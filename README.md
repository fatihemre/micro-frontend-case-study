# Frontend Developer Case Study - Mikro Frontend Dashboard

## 📋 Proje Açıklaması

Bu case study ile basit bir dashboard uygulamasını mikro frontend mimarisi kullanarak geliştirmenizi bekliyoruz. Proje 3 ayrı mikro frontend'den oluşacak ve modern frontend geliştirme pratiklerini içerecektir.

## 🎯 Hedefler

- Mikro frontend mimarisini anlama ve uygulama
- Modern React/JavaScript geliştirme pratikleri
- Kod kalitesi ve standartları
- Git workflow ve conventional commits

## 🏗️ Proje Yapısı

Aşağıdaki mikro frontend yapısını oluşturmanız beklenmektedir:

```
dashboard-microfrontends/
├── packages/
│   ├── shell/                # Container App
│   ├── user-card/            # User Card Mikro Frontend
│   └── content-bar/          # Content Bar Mikro Frontend
├── docs/
│   └── SETUP.md              # Kurulum dokümantasyonu
├── package.json              # Root package.json
└── README.md                 # Bu dosya
```

### Shell (Container) App
- Ana layout ve routing
- Header/navigation menu
- Mikro frontend orchestration
- Module Federation host

### User Card Mikro Frontend
- Kullanıcı profil kartı (avatar, isim, email)
- Notification drawer/popup/bubble/card (açılır/kapanır/dismissible)
- Notification badge ve sayac
- Mock kullanıcı verisi

### Content Bar Mikro Frontend
- Sağ tarafta content listesi
- Card/list görünümü
- Mock content verisi
- Basit hover efektleri

## 🎨 Tasarım Gereksinimleri

### Layout
```
┌─────────────── Header Menu (Full Width) ───────────────┐
├──────────────┬─────────────────────────────────────────┤
│              │                                         │
│  User Card   │         Content Bar                     │
│              │                                         │
│              │                                         │
└──────────────┴─────────────────────────────────────────┘
```

### Responsive Davranış
- Desktop: Yan yana layout
- Mobile/Tablet: Stack layout (üst üste)

### UI Gereksinimleri
- Modern ve temiz tasarım
- Notification drawer animasyonu (opsiyonel)
- Hover efektleri (opsiyonel)
- Loading states (opsiyonel)

## 🛠️ Teknik Gereksinimler

### Teknoloji Stack
- **Framework**: React.js (18+)
- **Build Tool**: Vite veya Webpack 5
- **Mikro Frontend**: Module Federation
- **Styling**: Tailwind CSS veya Styled Components
- **State Management**: React Context veya Zustand
- **TypeScript**: Tercihen kullanın

### Kod Standartları
- ESLint + Prettier konfigürasyonu
- Conventional Commits kullanımı
- Anlamlı component ve dosya isimlendirme
- Clean code prensipleri

### Git Workflow
- Feature branch'ler ile geliştirme
- Conventional commit messages:
  ```
  feat: add notification drawer component
  fix: resolve responsive layout issue
  docs: update setup documentation
  style: apply consistent formatting
  refactor: optimize component structure
  ```

## 📦 Kurulum Talimatları

### 1. Repository'yi Fork Edin
1. Bu repository'yi GitHub'da fork edin
2. Fork edilmiş repository'yi **private** yapın
3. `fatihemre` GitHub hesabını repository'nize **contributor** olarak ekleyin

### 2. Development Workflow
```bash
# Feature branch oluşturun
git checkout -b feat/user-card-component

# Geliştirme yapın ve commit atın
git add .
git commit -m "feat: implement user card component with avatar"

# Push edin
git push origin feat/user-card-component
```

## 📚 Gerekli Dokümantasyon

Projenizde aşağıdaki dokümantasyonu hazırlamanız beklenmektedir:

### `/docs/SETUP.md`
- Proje kurulum adımları
- Development server başlatma
- Build alma süreçleri
- Deployment talimatları
- Troubleshooting

### Ana README.md Güncellemesi
- Proje açıklaması
- Teknoloji listesi
- Kullanım örnekleri
- Demo linkleri (tercihen)

## 🚀 Deployment (opsiyonel)

### Gereksinimler
- Her mikro frontend Vercel'e ayrı deploy edilmeli
- Shell app ana domain'de host edilmeli
- Environment variables kullanımı
- Production build optimizasyonları

### Beklenen URL Yapısı
```
https://dashboard-shell.vercel.app/          # Ana uygulama
https://user-card-mf.vercel.app/            # User Card MF
https://content-bar-mf.vercel.app/          # Content Bar MF
```

## 📋 Değerlendirme Kriterleri

### Teknik Uygulama (40%)
- Mikro frontend mimarisinin doğru implementasyonu
- Module Federation kullanımı
- Component yapısı ve kod kalitesi
- State management

### Kod Kalitesi (25%)
- Clean code prensipleri
- ESLint/Prettier uyumluluğu
- Conventional commits
- Code organization

### UI/UX (20%)
- Responsive tasarım
- Tasarım UX açısından değerlendirilecektir. Shadcn, flowbite gibi hazır kütüphaneler kullanılabilir.

### Dokümantasyon (15%)
- Setup guide kalitesi
- Code comments
- README güncellemesi
- Clear instructions

## 📅 Teslim Süresi

**3 gün** içinde tamamlanması beklenmektedir.

## 📞 Destek

Sorularınız için:
- Kendi reponuz üzerinden GitHub Issues kullanabilirsiniz.

## 🏁 Teslim

Proje tamamlandığında:
1. `fatihemre` kullanıcısının repository'ye erişimi olduğundan emin olun
2. Demo URL'lerini README'ye ekleyin (varsa)
3. Kurulum dokümantasyonunu test edin
4. E-posta ile bilgi verin

---

**Not**: Bu case study ile teknik yeteneklerinizin yanı sıra problem çözme becerilerinizi, kod organizasyonunuzu ve dokümantasyon kalitesini de değerlendiriyoruz. Temiz, sürdürülebilir ve iyi dokümante edilmiş kod yazmaya odaklanın.
