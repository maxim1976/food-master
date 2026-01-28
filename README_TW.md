# 花蓮美食餐廳網站模板

## 快速開始

### 本地預覽
直接用瀏覽器打開 `index.html` 即可預覽網站。

### 主要特色

1. **完整繁體中文化** - 所有內容已轉換為繁體中文
2. **台灣在地化** - 電話、地址、營業時間符合台灣格式
3. **台灣料理菜單** - 牛肉麵、滷肉飯、珍珠奶茶等經典台灣美食
4. **LINE 社交整合** - 添加台灣最受歡迎的 LINE 圖標
5. **適合移動設備** - 響應式設計，完美支援手機瀏覽

### 網站架構

```
food-master/
├── index.html              # 主頁面 (已本地化為繁體中文)
├── assets/
│   ├── css/
│   │   ├── style.css      # 主樣式表 (已更新中文字體)
│   │   ├── responsive.css # 響應式樣式
│   │   └── ...
│   ├── js/
│   ├── images/
│   └── ...
├── TAIWAN_LOCALIZATION_NOTES.md  # 詳細本地化說明
└── README_TW.md                   # 本檔案
```

### 網站區塊

1. **導航選單** - 首頁、關於我們、特色、美食饗宴、菜單、外送服務、訂位專線
2. **主視覺區** - "道地台灣好味道"
3. **關於我們** - 餐廳介紹
4. **特色** - 獨家配方與傳承
5. **美食饗宴** - 8 道特色台灣料理展示
6. **菜單** - 完整菜單 (飲品、主餐、小吃)
7. **外送服務** - LINE、Uber Eats、foodpanda
8. **頁腳** - 聯絡資訊、營業時間、聯絡表單

### 客製化指南

#### 1. 更換餐廳資訊

在 `index.html` 中搜尋並替換以下資訊:

- **餐廳名稱**: `花蓮美食餐廳`
- **電話**: `03-8123-4567` (市話) 和 `0912-345-678` (手機)
- **地址**: `花蓮縣花蓮市中山路123號`
- **Email**: `info@hualien-food.com.tw`

#### 2. 修改菜單

找到 Portfolio Section 和 Menu Section，修改:
- 菜品名稱
- 價格 (NT$ 格式)
- 菜品描述

#### 3. 調整營業時間

在頁腳區域修改營業時間:
```html
<span class="date_day">週一至週五</span>
<span>11:30 - 14:00 (午餐)</span>
<span>17:30 - 21:00 (晚餐)</span>
```

#### 4. 更換圖片

圖片位置: `assets/images/`

需要替換的圖片:
- `logo.png` - 餐廳 Logo
- `bannerbg.jpg` - 主視覺背景
- `p1.png ~ p8.png` - 菜品圖片
- 其他背景圖片

建議圖片尺寸:
- Logo: 200x200px (透明背景 PNG)
- 主視覺: 1920x1080px
- 菜品圖片: 600x600px

#### 5. 修改配色

在 `assets/css/style.css` 中修改主色調:

```css
/* 主要色彩 */
#E7A331  /* 金黃色 - 主要強調色 */
#d6962c  /* 深金色 - 懸停效果 */
#000000  /* 黑色 - 背景 */
#ffffff  /* 白色 - 文字 */
```

### 字體說明

使用的中文字體順序:
1. **Noto Sans TC** - Google Fonts (線上字體)
2. **Microsoft JhengHei** - Windows 微軟正黑體
3. **PingFang TC** - macOS 蘋方-繁
4. **系統備用字體**

如果網路連接良好，會使用 Noto Sans TC。如果無法載入，會自動使用系統內建中文字體。

### 社交媒體連結

在 `index.html` 中找到社交媒體圖標區域，添加您的社交媒體連結:

```html
<a href="https://www.facebook.com/your-page"><i class="fa fa-facebook"></i></a>
<a href="https://line.me/R/ti/p/@your-id"><!-- LINE SVG --></a>
<a href="https://www.instagram.com/your-account"><i class="fa fa-instagram"></i></a>
```

### 外送平台整合

建議整合的台灣外送平台:
- **LINE 官方帳號** - 最受台灣用戶歡迎
- **Uber Eats** - https://www.ubereats.com/tw
- **foodpanda** - https://www.foodpanda.com.tw

### SEO 優化建議

1. 在 `<head>` 中添加更多 meta 標籤:
```html
<meta name="keywords" content="花蓮美食,台灣料理,牛肉麵,滷肉飯,花蓮餐廳">
<meta property="og:title" content="花蓮美食餐廳 - 正宗台灣料理">
<meta property="og:description" content="花蓮在地美食餐廳...">
<meta property="og:image" content="餐廳圖片網址">
```

2. 添加結構化資料 (Schema.org):
```json
{
  "@context": "https://schema.org",
  "@type": "Restaurant",
  "name": "花蓮美食餐廳",
  "address": {
    "@type": "PostalAddress",
    "streetAddress": "中山路123號",
    "addressLocality": "花蓮市",
    "addressRegion": "花蓮縣",
    "postalCode": "970"
  },
  "telephone": "+886-3-8123-4567",
  "servesCuisine": "台灣料理"
}
```

### 移動設備優化

網站已針對台灣高移動設備使用率優化:
- 觸控友好按鈕 (最小 44x44px)
- 響應式設計 (手機、平板、桌面)
- 快速載入優化
- 中文字體在小螢幕上清晰可讀

### 瀏覽器支援

- Chrome (推薦)
- Safari
- Firefox
- Edge
- 手機瀏覽器 (iOS Safari, Chrome Mobile)

### 部署建議

#### 1. GitHub Pages (免費)
```bash
# 將整個 food-master 資料夾推送到 GitHub
# 在 Settings > Pages 啟用 GitHub Pages
```

#### 2. Netlify (免費)
- 直接拖放 food-master 資料夾到 Netlify
- 自動獲得 HTTPS 網址

#### 3. 本地主機商
推薦台灣主機商:
- 中華電信 HiNet
- 遠傳電信
- Cloudmax

### 技術支援

如需詳細的本地化說明，請參考:
- `TAIWAN_LOCALIZATION_NOTES.md` - 完整本地化文件

### 授權

原始模板來自 Bootstrap Themes
台灣本地化改編: 2026

---

**提示**: 這是一個靜態網站模板。如需訂餐、會員系統等動態功能，需要額外的後端開發。

**推薦搭配**:
- LINE Bot (訂餐系統)
- Google Maps API (地圖整合)
- Google Analytics (流量分析)
- Facebook Pixel (廣告追蹤)
