# YOLO Object Detection 📦🎯

مشروع للكشف عن الأجسام باستخدام النموذج الجاهز [YOLOv5s](https://github.com/ultralytics/yolov5)، حيث يتم تحليل بث مباشر من كاميرا الهاتف عبر شبكة الـ Wi-Fi أو USB Tethering باستخدام `IP Webcam`.

## 📷 مدخلات المشروع:
- كاميرا الهاتف عبر تطبيق [IP Webcam](https://play.google.com/store/apps/details?id=com.pas.webcam)
- أو كاميرا USB/Webcam عادية

## ⚙️ المتطلبات:
- Python 3.10
- OpenCV
- PyTorch
- torch.hub
- اتصال إنترنت لتحميل النموذج أول مرة

## 🚀 التشغيل:
1. تأكد أن هاتفك وجهازك على نفس الشبكة.
2. افتح تطبيق IP Webcam وفعّله.
3. شغّل الكود التالي:
```python
ip_webcam_url = "http://<YOUR_PHONE_IP>:8080/video"
cap = cv2.VideoCapture(ip_webcam_url)
استمتع برؤية الكائنات تتعرف عليها YOLO في الوقت الحقيقي.
🧠 مستقبل المشروع:

    جعله API عبر Flask

    دعم متعدد للكاميرات (USB + IP)

    استخدامه في الروبوتات أو الطائرات بدون طيار
تم تنفيذ المشروع بالكامل على بيئة Ubuntu باستخدام كرت شاشة NVIDIA RTX 3060 وتفعيل CUDA لتسريع الكشف.
