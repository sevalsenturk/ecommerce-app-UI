# Full-Stack E-Commerce Project

Modern bir e-ticaret platformu. React 19, Node.js, Express.js ve MongoDB kullanılarak geliştirilmiştir.

## 🚀 Özellikler

### Kullanıcı Özellikleri
- ✅ Kullanıcı kaydı ve girişi
- ✅ Ürün listeleme ve detay görüntüleme
- ✅ Sepet yönetimi
- ✅ Kategori filtreleme
- ✅ Responsive tasarım

### Admin Özellikleri
- ✅ Kategori yönetimi (CRUD)
- ✅ Ürün yönetimi (CRUD)
- ✅ Kullanıcı yönetimi
- ✅ Admin paneli

## 🛠️ Teknolojiler

### Backend
- **Node.js** - JavaScript runtime
- **Express.js** - Web framework
- **MongoDB** - NoSQL veritabanı
- **Mongoose** - MongoDB ODM
- **JWT** - Authentication
- **bcryptjs** - Password hashing
- **CORS** - Cross-origin resource sharing

### Frontend
- **React 19** - UI library
- **Vite** - Build tool
- **Ant Design** - UI components
- **React Router** - Routing
- **React Slick** - Carousel/slider
- **Context API** - State management

## 📦 Kurulum

### Gereksinimler
- Node.js (v18+)
- MongoDB
- npm veya yarn

### Backend Kurulumu

1. Backend klasörüne gidin:
```bash
cd backend
```

2. Bağımlılıkları yükleyin:
```bash
npm install
```

3. Environment dosyasını oluşturun:
```bash
cp env.example .env
```

4. `.env` dosyasını düzenleyin:
```env
MONGO_URI=mongodb://localhost:27017/ecommerce
JWT_SECRET=your_secret_key_here
JWT_EXPIRE=7d
PORT=5000
FRONTEND_URL=http://localhost:5173
```

5. Sunucuyu başlatın:
```bash
npm start
```

### Frontend Kurulumu

1. Frontend klasörüne gidin:
```bash
cd frontend
```

2. Bağımlılıkları yükleyin:
```bash
npm install
```

3. Environment dosyasını oluşturun:
```bash
cp env.example .env
```

4. `.env` dosyasını düzenleyin:
```env
VITE_API_BASE_URL=http://localhost:5000
```

5. Geliştirme sunucusunu başlatın:
```bash
npm run dev
```

## 🌐 API Endpoints

### Authentication
- `POST /api/auth/register` - Kullanıcı kaydı
- `POST /api/auth/login` - Kullanıcı girişi

### Categories
- `GET /api/categories` - Tüm kategorileri getir
- `POST /api/categories` - Yeni kategori oluştur
- `PUT /api/categories/:id` - Kategori güncelle
- `DELETE /api/categories/:id` - Kategori sil

### Products
- `GET /api/products` - Tüm ürünleri getir
- `GET /api/products/:id` - Ürün detayını getir
- `POST /api/products` - Yeni ürün oluştur
- `PUT /api/products/:id` - Ürün güncelle
- `DELETE /api/products/:id` - Ürün sil

## 📁 Proje Yapısı

```
full-stack-e-commerce/
├── backend/
│   ├── models/          # MongoDB modelleri
│   ├── routes/          # API rotaları
│   ├── middleware/      # Middleware'ler
│   ├── server.js        # Ana sunucu dosyası
│   └── package.json
├── frontend/
│   ├── src/
│   │   ├── components/  # React bileşenleri
│   │   ├── pages/       # Sayfa bileşenleri
│   │   ├── layouts/     # Layout bileşenleri
│   │   ├── context/     # Context providers
│   │   └── config/      # Konfigürasyon dosyaları
│   └── package.json
└── README.md
```

## 🔧 Geliştirme

### Backend Geliştirme
- `npm run dev` - Nodemon ile geliştirme
- `npm start` - Production başlatma

### Frontend Geliştirme
- `npm run dev` - Vite dev server
- `npm run build` - Production build
- `npm run preview` - Build önizleme

## 🚨 Güvenlik

- JWT token authentication
- Password hashing (bcryptjs)
- CORS yapılandırması
- Input validation
- Error handling

## 📝 Lisans

Bu proje MIT lisansı altında lisanslanmıştır.

## 🤝 Katkıda Bulunma

1. Fork yapın
2. Feature branch oluşturun (`git checkout -b feature/amazing-feature`)
3. Commit yapın (`git commit -m 'Add amazing feature'`)
4. Push yapın (`git push origin feature/amazing-feature`)
5. Pull Request oluşturun

## 📞 İletişim

Proje hakkında sorularınız için issue açabilirsiniz. 