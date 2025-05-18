
---

# 🎬 Gemini Movie Recommendation System

یک سیستم توصیه‌گر فیلم ساخته‌شده با استفاده از مدل هوش مصنوعی Google Gemini و رابط کاربری Gradio.
کاربر نام یک فیلم مورد علاقه‌اش را وارد می‌کند و سیستم ۱۰ فیلم مشابه پیشنهاد می‌دهد.

## 🧠 تکنولوژی‌های استفاده‌شده

* [Google Generative AI (Gemini API)](https://ai.google.dev/)
* [Gradio](https://www.gradio.app/) برای رابط گرافیکی ساده و تعاملی


## 📦 نصب و اجرای پروژه

### 1. نصب پیش‌نیازها:

```bash
pip install gradio google-generativeai
```

### 2. اضافه‌کردن API Key

یک API Key از Google AI دریافت کنید و جایگزین این قسمت در کد کنید:

```python
genai.configure(api_key="YOUR_API_KEY")
```



### 3. اجرای برنامه:

```bash
python app.py
```

## 🖥️ نحوه استفاده

1. برنامه را اجرا کنید. مرورگر باز می‌شود.
2. در کادر، نام یک فیلم مورد علاقه خود را وارد کنید.
3. سیستم ۱۰ فیلم مشابه آن را پیشنهاد خواهد داد.






---

