Link:
Pytorch YOLOv3 https://drive.google.com/drive/folders/1QNYmoJnxGLueFw-uHbpUSXz3g60m0Cg8?usp=drive_link

ExDark 暗影像資料集  https://drive.google.com/file/d/1FExoROsfs4o8KpFWqFQ3fx44Upz1fblG/view?usp=drive_link
Enhance_Dark增強影像資料集  https://drive.google.com/file/d/1PPgGczvZ2vghXWunFuyPXQHxKGXSVN4C/view?usp=drive_link
影像label  https://drive.google.com/file/d/1TVxBCiRhGRMQEKQay9nZumyUoNPdFpGy/view?usp=drive_link 
weight權重  https://drive.google.com/file/d/1ZaClZ5MjeLe_4C1lboxkx3Ecb9U8FDg3/view?usp=drive_link



1.操作說明
未增強和有增強的路徑我存在Google Cloud中，.ipynb的code檔案中，有幾個block是透過Google Colab下載下來，並且會儲存到/content/PyTorch-YOLOv3/checkpoint/
檔案名稱編號23，為第一次訓練影像未增強的，30則為第二次訓練有增強圖像的
在Colab執行須注意路徑的位置
如果使用第一個not enhanced的pth file，PyTorch-YOLOv3/data/custom/內部的名稱無須更動
如果使用第二個enhanced的pth file，PyTorch-YOLOv3/data/內部的名稱Enhace_ExDark 這個資料夾的filename需更改為images，原本的images則需先換成別的隨意名稱

2.文件夾說明
IAT_model這個資料夾是影像增強的model程式碼
PyTorch-YOLOv3 則是物件偵測的主要程式碼
detect_image 則是我用來測試偵測效果的圖片
Object_detection為主程式
兩個Training process 的文字文件為訓練時的mAP和AP記錄的資料


///*Implementation*///

The paths for both the unenhanced and enhanced images are stored in Google Cloud. In the .ipynb code files, several blocks are downloaded through Google Colab and saved to /content/PyTorch-YOLOv3/checkpoint/. File number 23 corresponds to the first training of unenhanced images, while 30 corresponds to the second training of enhanced images. When executing on Colab, attention should be paid to the path's location.

If using the first unenhanced .pth file, the filenames inside PyTorch-YOLOv3/data/custom/ do not need to be changed. If using the second enhanced .pth file, the folder name in PyTorch-YOLOv3/data/ named Enhace_ExDark should be changed to "images", and the original "images" folder should be renamed to any other arbitrary name.

///*File explanation*///

IAT_model: This folder contains the code for image enhancement models.

PyTorch-YOLOv3: This is the main folder for object detection code.

detect_image: Contains images used to test detection effectiveness.

Object_detection: The main program file.

Text documents for the two training processes: These documents contain recorded mAP and AP data during training.


reference: 
https://github.com/eriklindernoren/PyTorch-YOLOv3
https://github.com/cuiziteng/Illumination-Adaptive-Transformer