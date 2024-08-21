# ImageGenerationFullAuto

# Package 組套
Install these package with pip:  [requests, json, time, hashlib, openpyxl, shutil] and [win11toast]
先用 pip 安裝這些套件： [requests, json, time, hashlib, openpyxl, shutil] and [win11toast]
For operative system before Windows 11, please find and delete every line that contains "toast"
作業系統版本比 Windows 11 舊的使用者，可以刪除所有包含 "toast" 的行 (ctrl+f 尋找)

# API 伺服器
Get an account on TensorArt (https://tensor.art/login), then get your API keys and App_ID at (https://tams.tensor.art/app)
先到 (https://tensor.art/login) 創帳號，然後在 (https://tams.tensor.art/app) 取得 API 金鑰和 App_ID

# image-to-image or prompt-to-image 圖生圖 或 文生圖 
If you want to generate image from image, set to  "True"; if set to "False", it would generate only from prompt
如果你想要從圖片生成圖片，請設為 "True"；如果設為 "False"，則會從提示詞生成圖片
(generate_from_image = True)


# Img source directory 圖片來源路徑(請從 C槽/D槽/E槽 開始)
(for example, C:\Image_Source)
Please put the source image in the directory with the same name as the row number (row-number-directory),
then put the row-number-directory under the storage-directory 
請將放置圖片的資料夾命名為 Excel檔案中存放提示詞那列的編號，然後將該資料夾放在 image_source_path這個資料夾裡面
(for example, C:\Image_Source\4, C:\Image_Source\4\image_001.jpg)

# About directory where you put your image: 關於來源圖片應該怎麼放：
for each image in the directory: 
this program will make a sub-directory with the same name as the image, and put the image into the sub-directory, 
then put generated image into that sub-directory
storage-directory內的每張圖片都會被這個程式建立一個子資料夾，子資料夾名稱同圖片名稱，
然後將圖片會被複製到子資料夾裡面，然後生成的圖片會存在子資料夾裡面
(for example, C:\Image_Source\4\image_001.jpg => C:\Image_Source\4\image_001\image_001.png [生成圖片會存在同一個資料夾裡面])
