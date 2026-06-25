# oa-page-classroom

橘子蘋果教學據點頁（`/classroom`）的自助 landing page prototype。

## 部署網址
https://orangeapple.co/classroom

## 維護方式
**只改一個地方**：`index.html` 內 `<script id="locations-data">` 的 JSON 陣列。

改完後：
- 畫面教室列表自動同步更新
- Google 看到的 LocalBusiness × N schema 自動同步更新
- 兩者永不脫鉤

## SEO/AEO/GEO 內建項目
- ✅ Title / meta description / canonical / robots
- ✅ Open Graph + Twitter Card
- ✅ JSON-LD: Organization + EducationalOrganization + BreadcrumbList + WebPage + ItemList + LocalBusiness × 44 + FAQPage + Article + Speakable
- ✅ 單一資料源 locations pattern
- ✅ Mobile responsive
- ✅ 縣市篩選 + 區域搜尋
- ✅ Google Maps 整合（每個教室）
- ✅ Click-to-call 電話連結
- ✅ Rails shell 注入點（`<oa-header>` / `<oa-footer>`）

## 上線前 checklist
跑 `/oa-webpage-preflight` 確認 SEO meta、schema、CTA 屬性齊全。

## 上線後驗證
- Google [Rich Results Test](https://search.google.com/test/rich-results)
- GSC 提交 URL 索引
- 確認 sitemap 包含 `/classroom/`
- Google Business Profile 同步檢查（每個實體教室）
