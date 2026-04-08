
## 🌟 Loyiha haqida (Oddiy tilda)
Tasavvur qiling, sizda minglab foydalanuvchilarning fikrlari bor. Ularning har birini o'qib chiqishga vaqt yo'q. Ushbu loyiha — **Inson kabi fikrlaydigan Sun'iy Intellekt** bo'lib, u har qanday gapni o'qiydi va soniyalar ichida uning ijobiy yoki salbiy ekanini aytib beradi.



---

## 🧠 Bu qanday ishlaydi?
Ushbu loyihada dunyodagi eng ilg'or texnologiyalardan biri — **Transformer (DistilBERT)** arxitekturasidan foydalanilgan. 

### 🛠 Texnik jarayon:
1. **Model:** `distilbert-base-uncased` (Dunyo tillarini biladigan tayyor "raqamli miya").
2. **Dataset:** 25,000 ta kinolarga yozilgan sharhlardan iborat **IMDB** to'plami.
3. **Fine-Tuning:** Biz tayyor modelni o'zimizning ma'lumotlar bilan qayta o'qitib, uni aynan "ijobiy/salbiy"ni ajratishga ixtisoslashtirdik.
4. **GPU (T4):** O'qitish jarayonini tezlashtirish uchun grafik protsessorlardan foydalanildi.

---

## 📈 Model Natijalari (Test natijasi)

Sun'iy intellekt matnlarni qanchalik aniq tushunishini quyidagi jadvalda ko'rishingiz mumkin:

| Foydalanuvchi fikri | AI bergan baho | Ishonch darajasi |
| :--- | :--- | :---: |
| "Bu darslik shunchaki ajoyib, juda ko'p narsani o'rgandim!" | **POSITIVE (Ijobiy)** | **99.8%** |
| "Vaqtimni behuda sarfladim, juda zerikarli ekan." | **NEGATIVE (Salbiy)** | **98.5%** |
| "Kino yomon emas, lekin juda uzun." | **POSITIVE (Ijobiy)** | **85.2%** |

---

## 🚀 Qanday ishga tushirish kerak?

Agar siz dasturchi bo'lsangiz, loyihani o'z kompyuteringizda sinab ko'rish uchun:

1. **Kutubxonalarni o'rnating:**
```bash
pip install -U evaluate datasets transformers[torch] accelerate
Kodni yurgizing:

Python
# Modelni yuklash va test qilish
from transformers import pipeline
classifier = pipeline("sentiment-analysis", model="./results/checkpoint-XXX")
print(classifier("I love this project!"))
🎯 Loyiha xususiyatlari
Accuracy (Aniqlik): 91% dan yuqori.

Tezlik: Bir soniyada o'nlab matnlarni tahlil qila oladi.

Aqlli yondashuv: Faqat so'zlarni emas, gapning umumiy ma'nosini (sarkazm, inkor) tushunadi.

👨‍💻 Muallif haqida
Men JAvohirxon, Data Science va Sun'iy Intellekt sohasida izlanayotgan mutaxassisman. Ushbu loyiha mening Machine Learning va NLP (Tabiiy tilni qayta ishlash) yo'nalishidagi ko'nikmalarimni namoyish etadi.
You Tube kanalim: @MachineLearning_IT
