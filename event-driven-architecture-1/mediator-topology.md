# توپولوژی میانجی

```
توپولوژی واسطه برای رویدادهایی که دارای چندین مرحله هستند مفید است
و برای پردازش رویداد نیاز به سطحی از ارکستراسیون دارد. برای
به عنوان مثال، یک رویداد واحد برای انجام معامله سهام ممکن است به شما نیاز داشته باشد
ابتدا معامله را تأیید کنید، سپس مطابقت آن معامله سهام را بررسی کنید
برخلاف قوانین انطباق مختلف، معامله را به یک کارگزار واگذار کنید،
کمیسیون را به تاخیر انداخت و در نهایت معامله را با آن کارگزار انجام داد. همه
از این مراحل به سطحی از ارکستراسیون برای جلوگیری از
11
من ترتیب مراحل و اینکه کدام یک را می توان به صورت سریال انجام داد و
به موازات.
```

```
چهار نوع اصلی از اجزای معماری در داخل وجود دارد
توپولوژی میانجی: صف های رویداد، میانجی رویداد، کانال های رویداد،
و پردازنده های رویداد جریان رویداد با ارسال یک کلاینت شروع می شود
رویداد به صف رویداد، که برای انتقال رویداد به آن استفاده می شود
میانجی رویداد واسطه رویداد، رویداد اولیه و
آن رویداد را با ارسال رویدادهای ناهمزمان اضافی هماهنگ می کند
به کانال های رویداد برای اجرای هر مرحله از فرآیند. فرآیند رویداد -
ors که در کانال های رویداد گوش می دهند، رویداد را از کانال دریافت می کنند
میانجی رویداد و اجرای منطق تجاری خاص برای پردازش
رویداد. شکل 2-1 توپولوژی کلی میانجی را نشان می دهد
الگوی معماری رویداد محور
```

```
این معمول است که از یک دوجین تا چند صد نفر داشته باشید
صف های رویداد در معماری رویداد محور الگو انجام می دهد
اجرای جزء صف رویداد را مشخص نمی کند. آی تی
می تواند یک صف پیام، یک نقطه پایانی وب سرویس یا هر ترکیبی باشد
از آن
```

```
دو نوع رویداد در این الگو وجود دارد: یک رویداد اولیه و
یک رویداد پردازشی رویداد اولیه، رویداد اصلی دریافت شده توسط است
معماری رویداد محور
میانجی، در حالی که رویدادهای پردازش آنهایی هستند که
توسط میانجی تولید می شوند و توسط پردازش رویداد دریافت می شوند
اجزاء.
```

```
مؤلفه میانجی رویداد مسئول هماهنگی است
مراحل موجود در رویداد اولیه برای هر مرحله در آغاز
رویداد، واسطه رویداد یک رویداد پردازشی خاص را ارسال می کند
به یک کانال رویداد، که سپس دریافت و پردازش می شود
پردازنده رویداد ذکر این نکته ضروری است که میانجی رویداد
در واقع منطق تجاری لازم برای پردازش را انجام نمی دهد
رویداد اولیه؛ بلکه از مراحل مورد نیاز برای پردازش اولیه می داند
واقعه تیال
```

```
کانال های رویداد توسط واسطه رویداد به صورت ناهمزمان استفاده می شوند
رویدادهای پردازشی خاص مربوط به هر مرحله را در مرحله اولیه ارسال کنید
رویداد به پردازنده های رویداد. کانال‌های رویداد می‌توانند به صورت پیام‌رسان باشند
صف های حکیم یا موضوعات پیام، اگرچه موضوعات پیام بیشتر هستند
به طور گسترده ای با توپولوژی واسطه استفاده می شود به طوری که وقایع پردازش
می تواند توسط چندین پردازنده رویداد پردازش شود (هر کدام یک
وظیفه متفاوت بر اساس رویداد پردازش دریافت شده).
```

```
اجزای پردازشگر رویداد شامل کسب و کار برنامه است
منطق لازم برای پردازش رویداد پردازش. پردازنده های رویداد هستند
ترکیب معماری مستقل، مستقل و به شدت جدا شده
شبکه هایی که وظیفه خاصی را در برنامه یا سیستم انجام می دهند.
در حالی که دانه بندی جزء رویداد-پردازنده می تواند متفاوت باشد
از ریزدانه (به عنوان مثال، محاسبه مالیات بر فروش بر روی یک سفارش) تا درشت دانه (به عنوان مثال، رسیدگی به ادعای بیمه)، مهم است که
توجه داشته باشید که به طور کلی، هر جزء رویداد-پردازنده باید
یک کار تجاری واحد را تشکیل دهید و به سایر پردازشگرهای رویداد متکی نباشید
وظیفه خاص خود را کامل کند
```

```
میانجی رویداد را می توان به روش های مختلفی اجرا کرد. به عنوان یک
معمار، شما باید هر یک از این پیاده سازی ها را درک کنید
گزینه هایی برای اطمینان از اینکه راه حلی که برای رسانه رویداد انتخاب می کنید
tor با نیازها و نیازهای شما مطابقت دارد.
```

```
ساده ترین و رایج ترین پیاده سازی رویداد رسانه ای
ator از طریق هاب های یکپارچه سازی منبع باز مانند Spring Integra- است.
tion، Apache Camel یا Mule ESB. رویداد در این منبع باز جریان دارد
هاب های یکپارچه سازی معمولاً از طریق کد جاوا یا a پیاده سازی می شوند
DSL (زبان مخصوص دامنه). برای میانجیگری پیچیده تر
و ارکستراسیون، می توانید از BPEL (اجرای فرآیند تجاری) استفاده کنید
زبان) همراه با یک موتور BPEL مانند منبع باز
آپاچی ODE. BPEL یک زبان استاندارد XML مانند است که توصیف می کند
داده ها و مراحل مورد نیاز برای پردازش یک رویداد اولیه. برای خیلی
برنامه های بزرگ که نیاز به ارکستراسیون بسیار پیچیده تری دارند
(از جمله مراحل مربوط به تعاملات انسانی)، می توانید اجرا کنید
میانجی رویداد با استفاده از مدیر فرآیند کسب و کار (BPM) مانند
به عنوان jBPM.
```

```
درک نیازهای شما و تطبیق آنها با رویداد صحیح
پیاده سازی واسطه برای موفقیت هر معماری رویداد محور با استفاده از این توپولوژی حیاتی است. استفاده از یک منبع باز
گرشن هاب برای انجام مدیریت فرآیندهای تجاری بسیار پیچیده
ارکستراسیون دستوری برای شکست است، درست مانند اجرای BPM
راه حل برای اجرای منطق مسیریابی ساده
```

```
برای نشان دادن نحوه عملکرد توپولوژی واسطه، فرض کنید شما هستید
از طریق یک شرکت بیمه بیمه شده و تصمیم به نقل مکان می گیرید. که در
در این مورد، رویداد اولیه ممکن است چیزی شبیه جابجایی نامیده شود
رویداد. مراحل مربوط به پردازش یک رویداد جابجایی عبارتند از
همانطور که در شکل 2-2 نشان داده شده است. برای هر
مرحله اولیه رویداد، واسطه رویداد یک رویداد پردازشی ایجاد می کند (به عنوان مثال،
تغییر آدرس، نقل قول مجدد محاسبه، و غیره)، آن رویداد پردازش را به
کانال رویداد و منتظر می ماند تا رویداد پردازش توسط پردازش شود
پردازشگر رویداد مربوطه (به عنوان مثال، فرآیند مشتری، نقل قول
فرآیند و غیره). این روند تا تمام مراحل اولیه ادامه می یابد
رویداد نهایی پردازش شده است. تک نوار بالای نقل قول recalc
و به روز رسانی مراحل ادعا در میانجی رویداد نشان می دهد که این
مراحل را می توان همزمان اجرا کرد.
```
