# سوال ۱
طبق مراحل گفته در مثال، گام به گام هر بخش را انجام دادیم. فقط در چند مورد به دلیل ارور هایی که داشت، تغییراتی داده شد که در ادامه آن را شرح داده ایم.


- به جای info.cukes از io.cucumber استفاده کردیم. info.cukes ارور هایی داشت که با تعویض آن با io.cucumber رفع شد.

<img width="1216" alt="Screenshot 1402-09-17 at 16 49 17" src="https://github.com/dariusamiri/SE_LAB_5/assets/59167222/e30fecdc-18d9-42c2-80d2-d80976d5c2af">

- در نتیجه import هایی که در فایل MyStepdefs.java داشتیم، نیز تغییر کرد و به جای cucumber.api.java از io.cucumber java استفاده کردیم برای import.


<img width="1252" alt="Screenshot 1402-09-17 at 16 50 43" src="https://github.com/dariusamiri/SE_LAB_5/assets/59167222/d4788eff-3d85-4c2b-a328-7f972ff92367">



- همچنین import های RunnerTest.java نیز تغییراتی داشت که در تصویر آن را مشاهده می‌کنید.

<img width="1252" alt="Screenshot 1402-09-17 at 16 51 45" src="https://github.com/dariusamiri/SE_LAB_5/assets/59167222/4e4565f7-468f-4ab2-8f77-6085aab8525f">


# سوال ۲

- تست دوم سناریو دوم یعنی حاصل جمع -۱ و ۶ به مشکل خورد.
  
- به دلیل اینکه در regex هایی که در کلاس MyStepdefs&، برای تابع ورودی تعریف شده بود (\\d+) اعداد مثبت فقط به عنوان ورودی در نظر گرفته شده بود.
  
- با تغییر آن به (-?\\d+) اعداد منفی نیز به عنوان ورودی، معتبر خواهند بود.


<img width="706" alt="Screenshot 1402-09-17 at 18 36 59" src="https://github.com/dariusamiri/SE_LAB_5/assets/59167222/22e017bb-ee10-4276-a070-8cb127064210">





