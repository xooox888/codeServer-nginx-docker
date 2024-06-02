# codeServer-nginx-docker

## وصف المستودع

يحتوي هذا المستودع على إعدادات Docker لتشغيل خادم VSCode باستخدام Nginx مع دعم HTTPS. يمكن للمستخدمين إعداد بيئة تطوير متكاملة بسهولة باستخدام Docker Compose.

##  المتطلبات
- docker
- docker-compose

## المحتويات

| File | الوصف |
| ---- | -----|
| `Dockerfile.vscode`: | إنشاء VSCode server. |
|`Dockerfile.nginx`:| إنشاء nginx مع دعم التشفير HTTPs|
| `nginx/nginx.conf`: | ملف إعدادات nginx الأساسية.|
|`nginx/default.conf`: |ملف إعدادات إعادة التوجيه وخدمة HTTPs.|
|`docker-compose.yml`:| ملف Docker Compose لإدارة وتشغيل الحاويات.|

## كيفية الاستخدام


1. أنشئ مجلد جديد:
   ```bash
   mkdir new_folder
   cd new_folder
   ```

2. انسخ هذه الأوامر إلى التيرمينال لتحميل الملفات:
   ```bash
   git clone https://github.com/xooox888/codeServer-nginx-docker.git
   cd codeServer-nginx-docker
   ```
   
   
3. قم بتشغيل Docker Compose لتشغيل بيئة التطوير:

   ```bash
   docker-compose up
   ```
4. افتح متصفح الويب وانتقل إلى <https://localhost>
   


## ملاحظات
- تأكد من تحديث متغيرات البيئة مثل PASSWORD.
- يمكنك تخصيص الإعدادات الإضافية حسب الحاجة في ملفات Docker و Nginx.
