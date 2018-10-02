# Photogrammetry

Software and tools to be used in the following sessions:
* Agisoft PhotoScan (Mac/Win)
* Altizure (Cloud/App)
* Autodesk ReCap Pro (Cloud/Win)
* MeshLab (Mac/Win)
* Meshmixer (Mac/Win)
* Meshroom (Win)

## Session 2A

參考資料
* TED 2007: [Demo of PhotoSynth](https://www.ted.com/talks/blaise_aguera_y_arcas_demos_photosynth) (codename: SeaDragon)
* [範例下載](https://drive.google.com/open?id=1fUwpXxOF5bZ7r-NL2cx3kXOfNyrwwxbk)

### Photo taking 拍照注意事項

Rule of thumb: clear and recognizable visual features

* Take a lot of photos from different angles for sufficient coverage of the subject
* Do not change the settings on the camera during shooting
* Steady subject, prevent moving objects
* No shiny, relective, transparent, pure color surface
* Prevent: blur, out of focus, high contrast images

拍攝大原則：拍攝對象的材質與視覺特徵清楚、易於辨識。

* 卯起來拍、拍很多照片、從各個角度拍！從不同視角獲取足夠的重疊度。
* 相機設定不要改變，最好是定焦、定光圈，愈清晰愈好。
* 物件本身必須靜止，避免周邊可動素材、畫面模糊。
* 避免：亮面、反射面、透明表面、純色表面
* 避免：模糊、失焦、高對比

其他注意事項：相片格式JPEG，解析度愈高愈好，內含的EXIF資料需包括相機參數與曝光設定。

### Modeling Process 建模流程

1. Import photos &rarr; retrieve camera parameters \
   匯入照片 &rarr; 同時取得相機參數
2. Photo alignment (matching) & feature extraction &rarr; Feature matching \
   從照片取得特徵點、照片與特徵點配對
3. Structure from Motion (SfM) \
   動作推斷結構 &rarr; 反推相機位置、建立空間與幾何結構資訊
4. Build dense point cloud \
   建立高密度點雲
5. Build mesh \
   建立網格模型
6. Build texture \
   建立材質貼圖

### Agisoft PhotoScan

* 單機使用。30天免費試用版(專業版)。
* PROS: 適合一般用途。
* CONS: 較慢，大型模型需仰賴高階顯卡增加運算能力；需每個步驟監督。

步驟(Menu > Workflow)：
1. Add Photos or Add Folder...
1. Align Photos...
1. Build Dense Cloud...
1. Build Mesh...
1. Build Texture...

### Altizure

* 雲端服務，免費建模，付費下載。
* PROS: 簡單、免費建模、建模品質佳、聰明、一鍵執行。
* CONS: 無法自訂建模參數。

步驟：
* 開啟新專案 > 匯入照片 > 開始建模

### Autodesk ReCap Pro

* 學生免費使用，每個專案至多100張照片。
* 內含 ReCap & ReCap Photo。
* 可編輯、修整 mesh 模型。

步驟：
1. 在 ReCap Photo 中，選擇新專案類型 > Drone or Object
1. 匯入照片 > 開始建模（一鍵執行）

### Meshroom

* Windows only. Open source.
* PROS: 可一鍵執行、亦可調整參數。建模品質佳。
* CONS: 沒有明顯缺點。

步驟：
1. 開啟新專案 > 匯入照片 > 開始建模

### Meshmixer (Mesh editor)

### MeshLab (Mesh editor)
