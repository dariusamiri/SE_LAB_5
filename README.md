# سوال ۱
طبق مراحل گفته در مثال، گام به گام هر بخش را انجام دادیم. فقط در چند مورد به دلیل ارور هایی که داشت، تغییراتی داده شد که در ادامه آن را شرح داده ایم.


- به جای info.cukes از io.cucumber استفاده کردیم. info.cukes ارور هایی داشت که با تعویض آن با io.cucumber رفع شد.

<img width="1216" alt="Screenshot 1402-09-17 at 16 49 17" src="https://github.com/dariusamiri/SE_LAB_5/assets/59167222/e30fecdc-18d9-42c2-80d2-d80976d5c2af">

- در نتیجه import هایی که در فایل MyStepdefs.java داشتیم، نیز تغییر کرد و به جای cucumber.api.java از io.cucumber java استفاده کردیم برای import.


<img width="1252" alt="Screenshot 1402-09-17 at 16 50 43" src="https://github.com/dariusamiri/SE_LAB_5/assets/59167222/d4788eff-3d85-4c2b-a328-7f972ff92367">



- همچنین import های RunnerTest.java نیز تغییراتی داشت که در تصویر آن را مشاهده می‌کنید.

<img width="1252" alt="Screenshot 1402-09-17 at 16 51 45" src="https://github.com/dariusamiri/SE_LAB_5/assets/59167222/4e4565f7-468f-4ab2-8f77-6085aab8525f">


# سوال ۲

- تست دوم سناریو دوم یعنی حاصل جمع ۱- و ۶ به مشکل خورد.

- به دلیل اینکه در regex هایی که در کلاس MyStepdefs، برای تابع ورودی تعریف شده بود (+d\\ \\) اعداد مثبت فقط به عنوان ورودی در نظر گرفته شده بود.


<img width="706" alt="Screenshot 1402-09-17 at 18 36 59" src="https://github.com/dariusamiri/SE_LAB_5/assets/59167222/22e017bb-ee10-4276-a070-8cb127064210">

- با تغییر آن به (+d\\ \\?-) اعداد منفی نیز به عنوان ورودی، معتبر خواهند بود.


# سوال ۳

یک برنچ از main گرفتیم و نام آن را 3 گذاشتیم و مسئله خواسته شده را در این برنچ کدنویسی می‌کنیم.

- ابتدا سناریو خام را طراحی میکنیم.

<img width="1487" alt="Screenshot 1402-09-17 at 23 58 45" src="https://github.com/dariusamiri/SE_LAB_5/assets/59167222/8c0eafe2-8e40-45db-898f-d0a1b4c7a5c5">



- سپس در کلاس MyStepdefs تابع when را اضافه کردیم. برای این مسئله خواسته شده، از توابع Given و Then که پیشتر برای سناریو جمع، زده شده به صورت مشترک برای این سناریو نیز استفاده می‌کنیم. 

<img width="1271" alt="Screenshot 1402-09-17 at 23 45 46" src="https://github.com/dariusamiri/SE_LAB_5/assets/59167222/f3d691e1-3c65-448d-b82e-92e161b28f33">




- سپس به کلاس Calculator تابع sqdiv را اضافه می‌کنیم و الگوریتم آن را تعریف می‌کنیم که در واقع رادیکال، تقسیم دو عدد را محاسبه می‌کند.  java.lang.Math را نیز import کردیم تا از تایع sqrt آن استفاده کنیم.

 <img width="1271" alt="Screenshot 1402-09-17 at 23 46 03" src="https://github.com/dariusamiri/SE_LAB_5/assets/59167222/971cd3de-ae63-42f4-91eb-e3c1cc2fa471">


 - حال ران میکنیم و موفقیت آمیز است.

  <img width="1487" alt="Screenshot 1402-09-18 at 00 06 26" src="https://github.com/dariusamiri/SE_LAB_5/assets/59167222/6e6fab2a-bf6b-4fe5-8933-2ea0f262d47b">

  - در نهایت scenario outline را نیز تعریف میکنیم و تست میگیریم و موفقیت آمیز خواهند بود.

    <img width="1512" alt="Screenshot 1402-09-17 at 23 49 39" src="https://github.com/dariusamiri/SE_LAB_5/assets/59167222/ca321c82-8935-487d-841f-062d2f5d58f8">


