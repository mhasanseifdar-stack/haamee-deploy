# 🚀 راهنمای Deploy تمیز - Repository جدید

## 📦 فایل‌های این پوشه:

1. ✅ `server.js` - Backend
2. ✅ `package.json` - وابستگی‌ها
3. ✅ `liara.json` - تنظیمات لیارا
4. ✅ `.gitignore` - فایل‌های نادیده
5. ✅ `App.js` - Frontend (باید Build بشه)

---

## 🎯 مراحل:

### گام 1: Build کردن Frontend

```bash
# در پوشه frontend اصلی:
cd C:\Users\Administrator\Desktop\haamee-complete-system\frontend

# جایگزین App.js
copy App.js src\App.js

# Build
npm install
npm run build
```

پوشه `build` ساخته میشه.

---

### گام 2: کپی build به این پوشه

```bash
xcopy build ..\haamee-fresh\build\ /E /I
```

---

### گام 3: ساخت Repository جدید در GitHub

1. https://github.com → New Repository
2. نام: `haamee-deploy`
3. Public, بدون README
4. Create

---

### گام 4: Push به GitHub

```bash
cd haamee-fresh

git init
git add .
git commit -m "Initial deployment"
git remote add origin https://github.com/YOUR_USERNAME/haamee-deploy.git
git push -u origin main
```

---

### گام 5: اتصال به لیارا

1. لیارا → برنامه panel-haamee
2. استقرار → GitHub
3. قطع اتصال از repository قدیمی
4. اتصال به `haamee-deploy`
5. استقرار دستی

---

## ✅ تمام!

URL: https://panel-haamee.liara.run
