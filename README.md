# 樹木區域自動分類工具

用 DXF、GeoPackage 或 CSV 區域，將樹木座標（Tree No、X、Y）自動分到 Tree Group。可預覽地圖、搜尋組號或樹木編號，並匯出 CSV、KML、GPKG。檔案只在瀏覽器處理，不會上載到伺服器。

**網上使用：** [https://davychan188.github.io/tree-area-classifier/](https://davychan188.github.io/tree-area-classifier/)

建議用 **Chrome、Edge 或 Safari** 打開。iPad 亦可使用；搜尋欄已加大，方便觸控。

## 用法

1. 上傳樹木座標檔（CSV / TXT），或直接貼上 `Tree_No, X, Y`
2. 上傳一個或多個區域檔（DXF、GPKG 或 CSV）
3. 可先「預覽到地圖」，再按「開始分類」
4. 地圖上每個區域可直接顯示 TG 編號（例如 `TG774`）；可用「顯示 TG 編號」勾選顯示或隱藏
5. 用搜尋欄輸入 Tree Group（例如 `TG774`、`Group805`）或 Tree No（例如 `TG-T0078`、`0078`），地圖會標示並放大，結果表亦會篩選
6. 可複製或下載結果 CSV，亦可匯出 KML / GPKG / 多邊形 CSV

若 DXF 內含 Group 標籤（例如 Group867），結果欄會自動命名為 `Tree_Group`。多邊形 X 座標若多為負值且像香港格網（HK1980），會自動將 X 鏡射為正值。沒有被任何樹群多邊形包含的樹木會列為「未分類」。

分類使用檔案原始座標；地圖與 KML 才依所選座標系轉換。預設座標系為 HK1980 Grid（EPSG:2326）。

## 本機打開

也可以下載 `index.html`（或 `樹木區域自動分類工具.html`）雙擊打開，無需安裝。
