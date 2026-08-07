TASHKENTGUIDE DMC — WORDPRESS (HOSTINGER + ELEMENTOR) O'RNATISH YO'RIQNOMASI
==============================================================================

Bu paketda saytingiz "parchalar" (snippet) ko'rinishida tayyorlangan — 
har bir bo'limni alohida joylaysiz va KEYINCHALIK ORALARIGA istalgan 
Elementor blokini qo'shish juda oson bo'ladi.

------------------------------------------------------------------
0-QADAM. SAHIFALARNI YARATING (slug muhim!)
------------------------------------------------------------------
WordPress → Pages → Add New. Quyidagi sahifalarni yarating va 
"slug" (URL) larini aynan shunday qiling (havolalar shunga moslangan):

  Home        → bosh sahifa (Settings → Reading → Homepage qilib belgilang)
  Tours       → slug: tours
  Concierge   → slug: concierge
  Partner     → slug: partner
  Blog        → slug: blog       (oddiy Page sifatida)
  About Us    → slug: about
  Contact     → slug: contact

------------------------------------------------------------------
1-QADAM. GLOBAL CSS NI BIR MARTA JOYLANG
------------------------------------------------------------------
Appearance (Tashqi ko'rinish) → Customize → Additional CSS
→ "global-styles.css" faylining BUTUN matnini paste qiling → Publish.

(Elementor Pro bo'lsa: Elementor → Site Settings → Custom CSS ham bo'ladi.)
Bu bir marta qilinadi — barcha snippetlar shu stillardan foydalanadi.

------------------------------------------------------------------
2-QADAM. HAR SAHIFANI ELEMENTORDA YIG'ING
------------------------------------------------------------------
Har bir sahifada: Edit with Elementor → chap pastdagi ⚙ (Settings) →
Page Layout: "Elementor Canvas" tanlang (tema header/footerisiz toza sahifa).

So'ng "HTML" widgetini sudrab keling va tegishli fayl ichidagini paste qiling:

HOME sahifasi (har biri ALOHIDA HTML widget — tartib bilan):
  home-sections/01-header-topbar-menyu.html
  home-sections/02-hero-slider.html
  home-sections/03-statistika.html
  home-sections/04-kategoriyalar.html
  home-sections/05-mashhur-turlar.html
  home-sections/06-tour-builder-band.html
  home-sections/07-tripadvisor-sharhlar.html
  home-sections/08-b2b-forma.html
  home-sections/09-footer.html

  ★ Keyinchalik yangi bo'lim qo'shmoqchi bo'lsangiz — shu widgetlar 
    ORASIGA istalgan Elementor section/widgetini tashlaysiz. 

BOSHQA sahifalar (3 ta widget: header + tarkib + footer):
  1) 01-header-topbar-menyu.html   (Home'dagi bilan bir xil)
  2) page-content/<sahifa>-sahifa-tarkibi.html
  3) 09-footer.html

------------------------------------------------------------------
3-QADAM. TEKSHIRING
------------------------------------------------------------------
Preview qiling: menyu, dropdown, slider, formalar ishlashi kerak.
Formalar hozircha "mailto" (email dasturini ochadi). Professional forma 
uchun keyin Elementor Form yoki WPForms bilan almashtiring — 
qabul qiluvchi: info@tashkentguide.com

------------------------------------------------------------------
QO'SHIMCHA MASLAHATLAR
------------------------------------------------------------------
• RASMLAR: hozir rasmlar Unsplash internetdan yuklanadi, logo va shaxsiy 
  rasmlar esa fayl ichiga joylangan (base64). Tezlik uchun keyinchalik: 
  Media Library'ga rasm yuklang → URL nusxalang → snippetdagi eski URL 
  o'rniga qo'ying. "images/" papkasida logolaringiz bor.
• KATTA SNIPPETLAR: 02-hero-slider.html va about tarkibi katta (shaxsiy 
  rasmlar fayl ichiga joylangani uchun). Yengillashtirish uchun: images/ 
  papkasidagi slider-*.jpg va about-portrait.jpg rasmlarini Media Library'ga 
  yuklang, so'ng snippetdagi "data:image/jpeg;base64,..." bilan boshlanuvchi 
  uzun matnni o'sha rasmning URL manziliga almashtiring.
• TRIPADVISOR: 07-tripadvisor-sharhlar.html ichida "TRIPADVISOR-EMBED" 
  izohi bor — real widget kodini tripadvisor.com/Widgets dan olib 
  o'sha joyga qo'ying.
• GOOGLE MAP: contact sahifasida "GOOGLE-MAP-EMBED" izohi bor — 
  Google Maps → Share → Embed a map → iframe kodini almashtiring.
• FAVICON: Appearance → Customize → Site Identity → images/logo-humo.png
• TEZKOR DEMO: full-pages/ papkasidagi 7 faylni Hostinger File Manager 
  orqali public_html/demo/ ga yuklasangiz, domeningiz/demo/index.html 
  da saytni WordPresssiz ham darhol ko'rsangiz bo'ladi.

Savol tug'ilsa — Claude'ga qaytib yozing, birga sozlaymiz!
