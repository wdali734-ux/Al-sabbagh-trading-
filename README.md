# 🎨 منصة الصباغ للتجارة الإلكترونية

## وصف المشروع

منصة تجارة إلكترونية متكاملة متخصصة في بيع الدهانات والمنتجات المرتبطة بها. تجمع بين واجهة ويب حديثة وتطبيق موبايل سهل الاستخدام مع نظام قوي في الخلفية.

## ✨ المميزات الأساسية

- 🛍️ **عرض المنتجات** - كاتالوج شامل للدهانات والمنتجات
- 🛒 **نظام الطلبات** - طلب المنتجات بسهولة
- 📱 **تطبيق موبايل** - تطبيق متقدم للعملاء
- 🌐 **واجهة ويب** - منصة ويب متجاوبة
- 🔒 **نظام آمن** - أمان عالي للبيانات والمعاملات
- 📊 **لوحة تحكم** - إدارة المنتجات والطلبات

## 🛠️ التكنولوجيات المستخدمة

### Backend
- **Node.js** - بيئة التشغيل
- **Express.js** - إطار العمل
- **MongoDB** - قاعدة البيانات
- **JWT** - المصادقة والتفويض

### Frontend
- **React.js** - واجهة الويب
- **React Native** - تطبيق الموبايل
- **Axios** - التواصل مع API

### أدوات التطوير
- **Git** - إدارة الإصدارات
- **GitHub** - المستودع
- **Nodemon** - تطوير سريع

## 📋 المتطلبات

- **Node.js** (v16 أو أعلى)
- **npm** أو **yarn**
- **MongoDB** (محلي أو سحابي)
- **Git**

## 🚀 البدء السريع

### 1️⃣ استنساخ المستودع

```bash
git clone https://github.com/wdali734-ux/Al-sabbagh-trading-.git
cd Al-sabbagh-trading-
```

### 2️⃣ تثبيت الحزم

```bash
npm install
```

### 3️⃣ إعداد متغيرات البيئة

```bash
cp .env.example .env
```

ثم عدّل ملف `.env` بمعلوماتك:

```env
PORT=5000
NODE_ENV=development
MONGODB_URI=mongodb://localhost:27017/al-sabbagh-trading
CORS_ORIGIN=http://localhost:3000
JWT_SECRET=your_secret_key_here
```

### 4️⃣ تشغيل الخادم

**وضع التطوير** (مع Reload تلقائي):
```bash
npm run dev
```

**وضع الإنتاج**:
```bash
npm start
```

الخادم سيعمل على: `http://localhost:5000`

## 📁 هيكل المشروع

```
Al-sabbagh-trading-/
│
├── server.js                 # نقطة البداية
├── package.json              # الحزم والتبعيات
├── .env.example              # متغيرات البيئة
├── .gitignore                # ملفات مخفية
│
├── routes/                   # مسارات API
│   ├── products.js          # منتجات
│   ├── orders.js            # طلبات
│   └── auth.js              # المصادقة
│
├── models/                   # نماذج قاعدة البيانات
│   ├── Product.js
│   ├── Order.js
│   └── User.js
│
├── controllers/              # معالجات الطلبات
│   ├── productController.js
│   ├── orderController.js
│   └── authController.js
│
├── middleware/               # وسائط
│   ├── auth.js              # التحقق من التفويض
│   └── errorHandler.js      # معالجة الأخطاء
│
└── README.md                 # هذا الملف
```

## 🔌 API Endpoints

### المنتجات
- `GET /api/products` - الحصول على جميع المنتجات
- `GET /api/products/:id` - الحصول على منتج معين
- `POST /api/products` - إضافة منتج جديد
- `PUT /api/products/:id` - تعديل منتج
- `DELETE /api/products/:id` - حذف منتج

### الطلبات
- `GET /api/orders` - جميع الطلبات
- `POST /api/orders` - إنشاء طلب جديد
- `PUT /api/orders/:id` - تحديث حالة الطلب
- `DELETE /api/orders/:id` - إلغاء طلب

### المصادقة
- `POST /api/auth/register` - تسجيل حساب جديد
- `POST /api/auth/login` - تسجيل الدخول
- `POST /api/auth/logout` - تسجيل الخروج

## 📝 خطوات التطوير

- [ ] إعداد قاعدة البيانات MongoDB
- [ ] تطوير models المنتجات والطلبات
- [ ] بناء API للمنتجات والطلبات
- [ ] نظام المصادقة والتفويض
- [ ] واجهة الويب (React)
- [ ] تطبيق الموبايل (React Native)
- [ ] الاختبارات والـ QA
- [ ] النشر والإطلاق

## 🤝 المساهمة

نرحب بمساهماتك! اتبع هذه الخطوات:

1. **Fork** المستودع
2. **أنشئ فرع** للميزة الجديدة:
   ```bash
   git checkout -b feature/amazing-feature
   ```
3. **Commit** التغييرات:
   ```bash
   git commit -m 'Add amazing feature'
   ```
4. **Push** إلى الفرع:
   ```bash
   git push origin feature/amazing-feature
   ```
5. **افتح Pull Request**

## 📄 الترخيص

هذا المشروع تحت رخصة MIT - انظر ملف [LICENSE](LICENSE) للتفاصيل

## 📞 التواصل والدعم

للأسئلة والدعم:
- 📧 البريد الإلكتروني: support@sabbagh-trading.com
- 🐛 افتح Issue في المستودع
- 💬 ناقش في Discussions

## 🎯 الأهداف المستقبلية

- ✅ نظام الدفع المتقدم
- ✅ تقييمات المنتجات والعملاء
- ✅ نظام التوصيل والشحن
- ✅ لوحة تحكم متقدمة للإدارة
- ✅ تطبيقات الجوال الأصلية

---

**آخر تحديث:** 2026-05-22

**صُنع بـ ❤️ بواسطة فريق الصباغ للتجارة**
