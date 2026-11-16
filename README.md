# 🌤️ Azərbaycan Hava Proqnozu

Azərbaycanın **bütün 66 rayonu** və 8 böyük şəhəri üçün canlı hava məlumatı. Rayonun üzərinə toxunanda saatlıq və 7 günlük proqnoz, külək, təzyiq, UV və hava keyfiyyəti kimi ətraflı məlumat açılır.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)
![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-222?logo=github&logoColor=white)
![Asılılıq yoxdur](https://img.shields.io/badge/as%C4%B1l%C4%B1l%C4%B1q-yoxdur-brightgreen)

**Canlı demo:** https://mireli5656.github.io/az-hava-xeritesi/

## ✨ Xüsusiyyətlər

- **74 məkan:** 66 rayon və 8 şəhər (Bakı, Gəncə, Sumqayıt, Mingəçevir, Naxçıvan, Şirvan, Naftalan, Xankəndi)
- **Ölkə xülasəsi:** ən isti, ən soyuq, ən küləkli və ən çox yağıntı olan yer
- **Axtarış:** `ə, ı, ö, ü, ç, ş, ğ` hərfləri olmadan da işləyir (məsələn, `agdam` → Ağdam)
- **Çeşidləmə:** əlifba, ən isti, ən soyuq, yağış, külək
- **Detallı pəncərə:** rayona toxunanda açılır (aşağıdakı cədvələ baxın)
- **★ Sevimlilər:** seçdiyiniz rayonlar siyahının yuxarısında qalır
- **📍 Mənə yaxın:** məkanınıza ən yaxın rayonun hava məlumatını açır
- **Avtomatik yenilənmə:** hər 15 dəqiqədən bir; internet yoxdursa son saxlanan məlumat göstərilir
- **Mobil uyğun, qaranlıq rejim** (cihaz ayarına görə avtomatik), klaviatura fokusu və azaldılmış hərəkət dəstəyi

### Detallı pəncərədə nələr var

| Bölmə | Məzmun |
|---|---|
| Cari vəziyyət | Temperatur, hiss olunan temperatur, hava təsviri, günün min/max dəyəri |
| Ölçülər | Rütubət, külək (m/s və istiqamət), küləyin zərbəsi, təzyiq (mm c.süt.), buludluluq, yağıntı, yağış ehtimalı, UV indeksi |
| Günəş | Günçıxma və gün batma vaxtı |
| Hava keyfiyyəti | Avropa hava keyfiyyəti indeksi, PM2.5 və PM10 |
| 24 saat | Temperatur qrafiki və saatlıq proqnoz (temperatur, yağış ehtimalı) |
| 7 gün | Gündəlik proqnoz, temperatur aralığı və yağış ehtimalı |

### Xəbərdarlıq nişanları

| Nişan | Şərt |
|---|---|
| 🔥 Çox isti | günün maksimumu ≥ 35° |
| 🧊 Şaxta | günün minimumu ≤ 0° |
| 🌧️ Güclü yağıntı | günlük yağıntı ≥ 10 mm |
| 💨 Güclü külək | küləyin zərbəsi ≥ 15 m/s |
| 🕶️ Yüksək UV | UV indeksi ≥ 8 |

## 🚀 İstifadə

Layihə tək `index.html` faylından ibarətdir, build alətləri və ya əlavə paketlər tələb etmir.

**Lokal işə salmaq:** `index.html` faylını brauzerdə açın. Hava məlumatı yüklənməsi üçün internet lazımdır.

**GitHub Pages-də yerləşdirmək:**

1. Faylı (`index.html`) repozitoriyanın kökünə yükləyin
2. **Settings → Pages** bölməsinə keçin
3. **Source** olaraq `Deploy from a branch`, branch olaraq `main` və qovluq olaraq `/ (root)` seçin
4. **Save** düyməsinə basın, bir neçə dəqiqədən sonra səhifə `https://<istifadəçi>.github.io/<repo>/` ünvanında açılır

## 🌐 Məlumat mənbələri

Hava məlumatı [Open-Meteo](https://open-meteo.com/) xidmətindən alınır, API açarı tələb olunmur:

- Proqnoz: `api.open-meteo.com/v1/forecast`
- Hava keyfiyyəti: `air-quality-api.open-meteo.com/v1/air-quality`

Open-Meteo məlumatı [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) lisenziyası ilə təqdim olunur və pulsuz plan qeyri-kommersiya istifadə üçündür.

## 🔒 Gizlilik

- Məkanınız yalnız **📍** düyməsinə basanda və yalnız brauzerin icazəsi ilə istifadə olunur. Ən yaxın rayon cihazınızın özündə hesablanır, koordinatlarınız heç yerə göndərilmir.
- Brauzerin yaddaşında (`localStorage`) yalnız sevimli rayonlarınız və son hava məlumatı saxlanır.

## ⚠️ Məhdudiyyətlər

- Koordinatlar rayon mərkəzləri üzrədir, rayonun bütün ərazisini əks etdirmir. Dağlıq rayonlarda hündürlük fərqi səbəbindən real hava dəyişə bilər.
- Proqnoz model əsaslıdır və rəsmi hidrometeorologiya xəbərdarlıqlarını əvəz etmir.
- Hava məlumatı və hava keyfiyyəti ayrı sorğularla alınır, ikincisi alınmasa həmin bölmə sadəcə göstərilmir.

## 🧱 Texnologiyalar

Təmiz **HTML**, **CSS** və **JavaScript**: framework yoxdur, build yoxdur, asılılıq yoxdur.

## 📁 Struktur

```text
.
├── index.html   # səhifənin bütün kodu (HTML + CSS + JS)
└── README.md
```

## 👤 Müəllif

[@Mireli5656](https://github.com/Mireli5656)

## 🤖 Hazırlanma

Bu layihə və sənədləşdirmə **Claude Sonnet 5.5** ilə hazırlanıb.
