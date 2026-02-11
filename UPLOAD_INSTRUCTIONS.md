# 📤 تعليمات رفع المشروع إلى GitHub

## الطريقة 1: باستخدام سطر الأوامر (Terminal)

### 1. تثبيت Git (إذا لم يكن مثبتاً)
```bash
# Windows: حمّل من
https://git-scm.com/download/win

# Mac: (عادة مثبت مسبقاً)
git --version

# Linux:
sudo apt-get install git
```

### 2. إعداد Git (أول مرة فقط)
```bash
git config --global user.name "اسمك"
git config --global user.email "بريدك@example.com"
```

### 3. الانتقال إلى مجلد المشروع
```bash
cd path/to/nafs-project
```

### 4. ربط المشروع بـ GitHub
```bash
# تهيئة Git
git init

# إضافة جميع الملفات
git add .

# أول Commit
git commit -m "Initial commit: نظام تحليل نافس المتقدم"

# ربط المستودع
git remote add origin https://github.com/abo-mohsen/nafs-g.git

# رفع الملفات
git push -u origin main
```

### ملاحظة: إذا طُلب منك تسجيل الدخول
```bash
# استخدم Personal Access Token بدلاً من كلمة المرور
# للحصول عليه:
# 1. اذهب إلى: https://github.com/settings/tokens
# 2. Generate new token (classic)
# 3. اختر scopes: repo
# 4. انسخ الـ token واستخدمه كـ password
```

---

## الطريقة 2: باستخدام GitHub Desktop (أسهل)

### 1. تحميل GitHub Desktop
https://desktop.github.com/

### 2. تسجيل الدخول
- افتح GitHub Desktop
- اضغط "Sign in to GitHub.com"
- سجّل دخولك

### 3. إضافة المشروع
- File → Add Local Repository
- اختر مجلد `nafs-project`
- اضغط "Create Repository"

### 4. الرفع
- Commit to main (أدخل رسالة)
- Publish repository
- اختر `nafs-g` كاسم المستودع
- اضغط "Publish repository"

---

## الطريقة 3: رفع مباشر من موقع GitHub

### 1. اذهب إلى المستودع
https://github.com/abo-mohsen/nafs-g

### 2. رفع الملفات
- اضغط "Add file" → "Upload files"
- اسحب الملفات:
  - `index.html`
  - `README.md`
  - `.gitignore`
  - `قاعدة_بيانات_المدارس_نموذجية.xlsx`
- اضغط "Commit changes"

---

## 🎯 التحقق من النجاح

بعد الرفع، تأكد من:
1. الملفات ظاهرة في https://github.com/abo-mohsen/nafs-g
2. README.md يظهر في الصفحة الرئيسية
3. يمكنك فتح الموقع مباشرة عبر GitHub Pages

---

## 🌐 تفعيل GitHub Pages (لفتح الموقع مباشرة)

### 1. اذهب إلى المستودع
https://github.com/abo-mohsen/nafs-g

### 2. Settings → Pages
- Source: Deploy from a branch
- Branch: main
- Folder: / (root)
- Save

### 3. انتظر دقيقة
الموقع سيكون متاح على:
```
https://abo-mohsen.github.io/nafs-g/
```

---

## 🔄 التحديثات المستقبلية

عند إجراء تعديلات على الملفات:

### باستخدام Terminal:
```bash
git add .
git commit -m "وصف التحديث"
git push
```

### باستخدام GitHub Desktop:
1. Commit to main
2. Push origin

---

## ⚠️ مشاكل شائعة وحلولها

### المشكلة: error: failed to push
**الحل:**
```bash
git pull origin main --rebase
git push
```

### المشكلة: Authentication failed
**الحل:**
استخدم Personal Access Token بدلاً من كلمة المرور

### المشكلة: المستودع غير موجود
**الحل:**
```bash
# تأكد من إنشاء المستودع في GitHub أولاً
# أو استخدم:
git remote set-url origin https://github.com/abo-mohsen/nafs-g.git
```

---

## 📞 الدعم

إذا واجهت أي مشكلة، تواصل معي أو افتح Issue في GitHub
