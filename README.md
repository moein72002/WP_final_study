# WP_final_study

<p dir="RTL">
Kubernetes چیست؟
 <p/>
 <p dir="RTL">
 Kubernetes تکنولوژی مدیریت کانتینری است که در Google lab برای مدیریت اپلیکیشن های کانتینری در محیط های مختلف استفاده می شود. Kubernetes یک سیستم اوپن سورس است که به ایجاد و مدیریت کانتینر کردن اپلیکیشن ها و خودکار سازی استقرار، مقیاس گذاری و مدیریت برنامه های کانتینر شده است.
<p/>

<p dir="RTL">
Kubernetes یک ابزار مدیریت کانتینری open source است که توسط بنیاد محاسبات بومی ابری (CNCF) میزبانی شده است. Kubernetes همچنین به عنوان نسخه پیشرفته Borg شناخته می شود که در گوگل برای مدیریت فرآیندهای در حال اجرا و پردازش های دسته ای شناخته شده بود که قبلا توسط سیستم های جداگانه مورد استفاده قرار گرفت. کوبرنتیز توانایی خودکارسازی استقرار، مقیاس بندی اپلیکیشن و عملیات کانتینرهای اپلیکیشن در بین کلاستر ها را دارد. همچنین قادر به ساخت زیرساخت کانتینر را دارد. بسیاری از سرویس های ابری یک بستر یا زیرساخت مبتنی بر کوبرنتیز را به عنوان سرویس(PaaS یا IaaS) ارائه می دهند که در آن می توان کوبرنتیز را به عنوان یک سرویس ارائه دهنده پلتفرم مستقر کرد.
<p/>
<p dir="RTL">
ویژگی های Kubernetes:
 <p/>
 <p dir="RTL">
Service discovery and load balancing: برای استفاده از مکانیسم کشف سرویس ناآشنا، نیازی به اصلاح برنامه خود ندارید. کوبرنتیز به Pod آدرس IP اختصاصی خود و یک نام DNS را برای مجموعه ای از Pod می دهد و می تواند بین آنها تعادل برقرار کند.
<p/>
<p dir="RTL">
Automatic bin packing: کانتینر را بطور خودکار بر اساس نیاز به منابع و محدودیت های دیگر خود قرار می دهد، در حالی که در دسترس بودن را فریب نمی دهد. برای کار کردن در استفاده و صرفه جویی در منابع بیشتر، بارهای کاری مهم و بهترین تلاش را با هم ادغام میکند.
<p/>
<p dir="RTL">
Storage orchestration: به صورت خودکار سیستم ذخیره سازی مورد نظر خود را، از محل ذخیره محلی، ارائه دهنده ابر عمومی مانند GCP یا AWS یا سیستم ذخیره شبکه مانندNFS ،iSCSI ،Gluster ،Ceph ،Cinder یا Flocker به صورت خودکار سوار کنید.
<p/>
<p dir="RTL">
Automated rollouts and rollbacks: Kubernetes به تدریج تغییراتی در برنامه یا پیکربندی آن ارائه می دهد، ضمن نظارت بر سلامتی برنامه، برای اطمینان از این که همه موارد شما را همزمان از بین نمی برد. اگر چیزی پیش نیاید، کوبرنتیز تغییراتی را برای شما به وجود می آورد. از یک اکوسیستم رو به رشد از راه حل های استقرار استفاده کنید.
<p/>
<p dir="RTL">
Secret and configuration management: اسرار و پیکربندی برنامه را بدون بازسازی تصویر خود و بدون افشای اسرار در تنظیمات cluster خود، مستقر و به روز کنید.
<p/>
<p dir="RTL">
Batch execution: علاوه بر سرویس ها، Kubernetes می تواند بار کاری دسته ای و CI شما را مدیریت کند و در صورت تمایل کانتینر را که خراب می شوند جایگزین کنید.
<p/>
<p dir="RTL">
Horizontal scaling: برنامه خود را با یک دستور ساده، با رابط کاربری یا به طور خودکار بر اساس استفاده ازCPU، از بالا و پایین مقیاس بندی کنید.
<p/>
<p dir="RTL">
کاربردهای Kubernetes 
 <p/>
 <p dir="RTL">
کانتینر یک روش مناسب برای بسته بندی و اجرای برنامه های شما هستند. در یک محیط تولید، شما باید کانتینر را کنترل کنید که برنامه ها را اجرا می کنند و از عدم خرابی اطمینان می دهند. به عنوان مثال، اگر یک کانتینر خاموش شود، کانتینر دیگری لازم است که راه اندازی شود. آیا اگر این رفتار توسط یک سیستم انجام شود، آسان تر نخواهد بود؟
<p/>
<p dir="RTL">
اینگونه است که کوبرنتیز برای نجات می آید! Kubernetes فریمورکی را برای اجرای سیستمهای توزیع شده به صورت انعطاف پذیر در اختیار شما قرار می دهد. این امر به نیازهای شما در مقیاس بندی، عدم موفقیت، الگوهای استقرار و موارد دیگر اهمیت می دهد. به عنوان مثال، Kubernetes به راحتی می تواند استقرار را برای سیستم شما مدیریت کند.
<p/>
<p dir="RTL">
مقایسه کوبرنتیز با داکر
کوبرنتیز و داکر هر دو راه حل جامع de-facto برای مدیریت هوشمندانه برنامه های کانتینر شده و ارائه قابلیت های قدرتمند هستند و از این طریق برخی از سردرگمی ها پدید آمده است. Kubernetes اکنون بعضاً به عنوان كلاهبرداری برای كل محوطه های كانتینری مبتنی بر كوبرنتیز مورد استفاده قرار می گیرد. در واقعیت، آنها به طور مستقیم قابل مقایسه نیستند، ریشه های مختلفی دارند و برای چیزهای مختلف حل می شوند.
<p/>

<p dir="RTL">
Docker یک سکوی و ابزاری برای ساخت، توزیع و اجرای Docker container است. این ابزار کلاستر بندی بومی خود را ارائه می دهد که می تواند برای orkstrate و برنامه ریزی کانتینر روی کلاستر های دستگاه مورد استفاده قرار گیرد. Kubernetes یک سیستم ارکستراسیون کانتینر برای کانتینر Docker است که گسترده تر از Docker Swarm است و به منظور هماهنگی کلاستر node ها در مقیاس در تولید به شیوه ای کارآمد است. در حول مفهوم Podها کار می کند، که واحدهای برنامه ریزی (و می توانند یک یا چند کانتینر را در خود جای دهند) در اکوسیستم Kubernetes است و آنها برای تهیه در دسترس در بین node ها توزیع می شوند. می توان به راحتی ساخت Docker را روی یک کلاستر Kubernetes اجرا کرد، اما خود Kubernetes یک راه حل کامل نیست و منظور از آن افزونه های سفارشی است.
<p/>

<p dir="RTL">
Kubernetes و Docker هر دو اساساً دارای تکنولوژی متفاوت هستند اما در کنار هم بسیار خوب کار می کنند و مدیریت و استقرار کانتینر در یک معماری توزیع شده را تسهیل می کنند.
<p/>
<p dir="RTL">
اصطلاحات Kubernetes
 <p/>
 <p dir="RTL">
Cluster: یک کلاستر اساس موتور Kubernetes است. اجسام Kubernetes که برنامه های کانتینر شده شما را نشان می دهد همه در بالای یک کلاستر اجرا می شوند. این مجموعه ای از ماشین ها (فیزیکی یا مجازی) است که برنامه های شما مدیریت و اجرا می شوند. برای Kubernetes، تمام ماشین ها بسته به توپولوژی مورد استفاده، به عنوان یک کلاستر (یا مجموعه ای از کلاستر ها) اداره می شوند.
<p/>
<p dir="RTL">
Node: یک کلاستر معمولاً دارای یک یا چند node است، یعنی ماشین های کارگر که برنامه های کانتینر شده و سایر کارهای شما را اجرا می کنند. در Kubernetes Engine، کلاستر متشکل از حداقل یک استاد کلاستر و چند ماشین کارگر به نام node است. واحد ماشین منطقی (فیزیکی یا مجازی)، که بخشی از یک کلاستر بزرگتر است که بر روی آن می توانید برنامه های خود را اجرا کنید.
<p/>
<p dir="RTL">
Pod: یک گروه کانتینر که در کانتینر ها قرار دارد و محل نگهداری آنها Pod یا به سادگی Pod است. گروهی از کانتینر که در همان میزبان مستقر می شوند. به عنوان مثال، معقول است که فرآیندهای بانک اطلاعاتی و کانتینر داده تا حد ممکن نزدیک باشند - در حالت ایده آل، آنها باید در همان Pod باشند.
<p/>

<p dir="RTL">
 Replication Controllers: یک مفهوم انتزاعی است که برای مدیریت چرخه عمر Podمورد استفاده قرار می گیرد. یکی از مهمترین کاربردهای کنترل کننده های تکرار، حفظ تعداد معینی Pod است. این کار همچنین مفید است اگر می خواهید تعداد خاصی از Podها را برای مقیاس گذاری فعال کنید، یا اطمینان حاصل کنید که حداقل یک Podوجود دارد. استفاده از کنترل کننده های تکرار برای تعریف چرخه عمر Pod، بهتر است به جای ایجاد Podبه طور مستقیم باشد.
<p/>
<p dir="RTL">
Selector: یک عبارت انتخاب کننده برای فیلتر کردن منابع خاص با برچسب ها مطابقت دارد. به عنوان مثال، شما ممکن است بخواهید تمام Pod هایی را که متعلق به یک سرویس خاص هستند جستجو کنید یا تمام کانتینر دارای یک مقدار خاص از برچسب لایه را به عنوان یک بانک اطلاعاتی پیدا کنید. می توانید از برچسب ها برای طبقه بندی منابع استفاده کنید و از انتخاب کنندگان برای یافتن آنها و استفاده از آنها برای اقدامات خاص استفاده کنید.
<p/>
<p dir="RTL">
Label: برچسب ها جفت های با ارزش اصلی هستند که به اشیاء مانند Pod ها وصل می شوند. از جفت های ارزش کلیدی می توان برای فیلتر، سازماندهی و انجام عملیات گسترده بر روی مجموعه ای از منابع استفاده کرد. به برچسب ها به عنوان یک نقش، گروه یا هر مکانیسم مشابه که به یک کانتینر یا منبع داده می شود فکر کنید. یک کانتینر می تواند نقش پایگاه داده داشته باشد، در حالی که دیگری می تواند یک توازن بار باشد.
<p/>
<p dir="RTL">
Replication Sets :Replica Sets تعیین می کند که تعداد ماکت های هر Pod در حال اجرا است. آنها همچنین مانیتور می کنند و اطمینان می دهند که تعداد Pod های لازم در حال اجراست، جای Pod هایی را که می میرند جایگزین می کنند. Replica Sets می تواند به عنوان جایگزینی برای کنترل کننده های Replication عمل کند.
<p/>
<p dir="RTL">
Annotation: حاشیه نویسی یک برچسب اما با ظرفیت داده بسیار بزرگتر است. به طور معمول، این داده ها توسط انسان قابل خواندن نیستند و از طریق فیلتر کردن آسان نیست. حاشیه نویسی فقط برای ذخیره داده هایی که ممکن است جستجو نشوند مفید است اما توسط منبع لازم است.
<p/>
<p dir="RTL">
Name: نامی است که یک منبع با آن مشخص می شود.
<p/>

<p dir="RTL">
Volume :Volume دایرکتوری است با داده هایی که برای یک کانتینر قابل دسترسی است. Volume با Pod هایی که آن را محصور می کند ، به پایان می رسد.
<p/>
<p dir="RTL">
Namespace :Namespace صلاحیت دیگری را برای نام یک منبع فراهم می کند. این امر به ویژه هنگامی مفید است که چندین تیم / پروژه از همان کلاستر استفاده کنند و احتمال برخورد نام نیز وجود دارد. می توانید از یک فضای نام به عنوان یک دیوار مجازی بین چندین کلاستر فکر کنید.
<p/>

<p dir="RTL">
Service: یک سرویس انتزاعی در بالای Pod است که یک آدرس IP اختصاصی و نام DNS را فراهم می کند که به وسیله آن می توان به Pod ها دسترسی پیدا کرد. این پیکربندی توازن بار بسیار ساده تر می شود و به Pod های Uniform scale کمک می کند.
<p/>
<p dir="RTL">
معماری Kubernetes
Kubernetes معماری اولیه / ماکت را دنبال می کند. اجزای Kubernetes را می توان به مواردی تقسیم کرد که یک node فردی را مدیریت می کنند و بخشی از صفحه کنترل هستند.
<p/>
<p dir="RTL">
پلن کنترلی Kubernetes (اولیه)
Kubernetes اولیه واحد کنترل اصلی کلاستر است و بار کاری آن را هدایت می کند و ارتباطات را در سراسر سیستم هدایت می کند. پلن کنترلی Kubernetes از اجزای مختلفی تشکیل شده است که هر یک فرایند خاص خود را دارند که می توانند هم در یک node اصلی واحد و هم در چندین اولیه که از کلاستر های در دسترس بالا پشتیبانی می کنند، اجرا شوند. اجزای مختلف پلن کنترلی Kubernetes به شرح زیر است:
<p/>
<p dir="RTL">
etcd: یک فروشگاه داده ثابت، سبک، توزیع شده و دارای ارزش کلیدی است که توسط CoreOS ایجاد شده است و داده های پیکربندی کلاستر را به طور قابل اعتماد ذخیره می کند و نمایانگر وضعیت کلی کلاستر در هر نقطه معین از زمان است. درست مانند Apache ZooKeeper سیستمی است که از ثبات بیش از دسترس بودن در صورت وجود پارتیشن شبکه حمایت می کند (به قضیه CAP مراجعه کنید). این قوام برای برنامه ریزی صحیح و خدمات عملی بسیار مهم است. سرور API Kubernetes از API ساعت etcd برای نظارت بر این کلاستر استفاده می کند و تغییرات مهم در پیکربندی را کنترل می کند و یا هر گونه واگرایی از وضعیت این کلاستر را باز می گرداند، به آنچه توسط اعزام کننده اعلام شده است. به عنوان نمونه، اگر مستقر اعلام کرد که سه نمونه از Pod خاص نیاز به دویدن دارد، این واقعیت در etcd ذخیره می شود. اگر مشخص شود که فقط دو نمونه در حال اجراست، این دلتا با مقایسه با داده های etcd شناسایی می شود و کوبرنتیز از این برنامه برای ایجاد یک نمونه اضافی از آن Pod استفاده می کند.
<p/>
<p dir="RTL">
سرور API: سرور API یک عنصر کلیدی است و API Kubernetes را با استفاده از JSON بر روی HTTP، که رابط داخلی و خارجی را نیز به Kubernetes ارائه می دهد، خدمت می کند. سرور API درخواست های REST را پردازش و تأیید می کند و وضعیت اشیاء API را در etcd به روز می کند، از این طریق به مشتریان امکان می دهد بارها و کانتینر کار را در node های کار پیکربندی کنند.
<p/>
<p dir="RTL">
Scheduler: Scheduler افزونه ای است که بر اساس در دسترس بودن منبع، کدام node را انتخاب نمی کند (یک موجود اصلی که توسط برنامه ریز مدیریت می شود) روی آن اجرا می شود. برنامه زمانبندی شده استفاده از منابع را در هر node دنبال می کند تا اطمینان حاصل کند که بار کاری بیش از منابع موجود برنامه ریزی نشده است. برای این منظور، برنامه ریز باید از الزامات منبع، در دسترس بودن منابع و سایر محدودیتها و دستورالعملهای ارائه شده توسط کاربر از قبیل کیفیت خدمات، الزامات وابستگی / ضد وابستگی، محل داده و etcd آگاه باشد. در اصل، نقش برنامه ریز مطابقت با "تأمین" منابع برای بار کاری "تقاضا" است.
<p/>
<p dir="RTL">
Controller manager: یک کنترل کننده حلقه تلفیقی است که حالت کلاستر واقعی را به سمت حالت کلاستر مورد نظر هدایت می کند و با ایجاد سرور API برای ایجاد، به روزرسانی و حذف منابعی که مدیریت می کند (Podها، نقاط پایانی سرویس) ارتباط برقرار می کند. مدیر کنترلر فرایندی است که مجموعه ای از کنترلرهای اصلی Kubernetes را مدیریت می کند. یک نوع کنترلر یک کنترل کننده Replication است که با اجرای تعداد مشخصی از نسخه های یک Pod در داخل کلاستر، همانند سازی و مقیاس گذاری را انجام می دهد. اگر node زیرین نیز نتواند Podهای جایگزینی را ایجاد کند. کنترل کننده های دیگر که بخشی از سیستم هسته ای Kubernetes هستند شامل یک کنترلر DaemonSet برای اجرای دقیقاً یک Podدر هر دستگاه (یا برخی از زیر مجموعه های دستگاه ها) و یک task controler برای اجرای Pod هایی که به اتمام می رسند. به عنوان مثال به عنوان بخشی از کار دسته ای مجموعه Podهایی که یک کنترل کننده مدیریت می کند توسط انتخاب کننده های برچسب تعیین می شود که جزئی از تعریف کنترلر است.
<p/>
<p dir="RTL">
StatefulSets
پرداختن به مقیاس برنامه های بدون تابعیت بسیار آسان است. یکی به سادگی تعداد بیشتری Podرا اضافه می کند، این کاری است که کوبرنتیز خیلی خوب انجام می دهد. اگر کار یک Podمجدداً راه اندازی شود، باید کارهایی با وضعیت بسیار سخت تر حفظ شود و اگر برنامه بالا یا پایین شود، ممکن است State مجدداً توزیع شود. بانک اطلاعاتی نمونه ای از بار کاری Stateful است. هنگام اجرا در حالت در دسترس بودن زیاد، بسیاری از بانکهای اطلاعاتی با مفهوم نمونه اولیه و نمونه های ثانویه همراه هستند. در این حالت، منظور از سفارش موارد مهم است. برنامه های کاربردی دیگر مانند کافکا داده ها را بین کارگزاران خود توزیع می کند - بنابراین یک کارگزار مانند دیگر نیست. در این حالت، مفهوم منحصر به فرد بودن مثال مهم است. StatefulSets کنترلرهایی هستند که توسط Kubernetes تهیه شده اند و خواص یکتایی و نظم را در بین موارد Pod اعمال می کنند و می توانند برای اجرای برنامه های حالت پذیر استفاده شوند.
<p/>
<p dir="RTL">
گره Kubernetes
Node که به عنوان Worker یا Minion نیز شناخته می شود، ماشینی است که کانتینرها (بار کاری) در آن مستقر می شوند. هر گره در این کلاستر برای برقراری ارتباط با اولیه برای پیکربندی شبکه این کانتینر باید یک زمان اجرا از کانتینر مانند Docker و همچنین مؤلفه های زیر را اجرا کند.
<p/>
<p dir="RTL">
Kubelet :Kubelet مسئول عملکرد هر گره است و از سالم بودن تمام کانتینر موجود در این گره می باشد. مراقبت از شروع، متوقف کردن و نگهداری کانتینر کاربردی که به وسیله پلنی کنترل به درون Pod ها ترتیب داده می شوند.
<p/>
<p dir="RTL">
Kubelet وضعیت یک Pod را کنترل می کند و اگر در حالت مورد نظر نباشد، Pod دوباره در همان گره مستقر می شود. وضعیت گره هر چند ثانیه از طریق پیام های ضربان قلب به اولیه منتقل می شود. هنگامی که Primary node fracture را تشخیص داد، کنترل کننده Replication این تغییر حالت را مشاهده می کند و Pod ها را روی سایر گره های سالم راه اندازی می کند.
<p/>
<p dir="RTL">
Kube-proxy: اجرای پروکسی شبکه و یک تعادل بار است و از انتزاع سرویس به همراه سایر عملکرد شبکه پشتیبانی می کند. این مسئول مسیریابی ترافیک به کانتینر مناسب را براساس IP و شماره پورت درخواست ورودی دریافت می کند.
<p/>
<p dir="RTL">
runtime کانتینر: یک کانتینر در داخل یک Pod قرار دارد. کانتینر پایین ترین سطح یک سرویس خرد است که برنامه در حال اجرا، کتابخانه ها و وابستگی های آنها را در خود جای داده است. کانتینرها می توانند از طریق یک آدرس IP خارجی در معرض دید جهانیان قرار بگیرند. Kubernetes از اولین نسخه خود از کانتینر Docker پشتیبانی می کند و در ژوئیه سال 2016 در موتور کانتینر اضافه شده است.
<p/>
<p dir="RTL">
Add-ons
Add-ons ها دقیقاً مانند هر برنامه دیگری که در داخل کلاستر قرار دارد کار می کنند. آنها از طریق Podو سرویس ها پیاده سازی می شوند و تنها با این تفاوت که با ویژگی های کلاستر Kubernetes پیاده سازی می شوند. Pod ها را می توان با استقرار، ReplicationControllers و etcd مدیریت کرد. افزودنیهای بسیاری وجود دارد و لیست در حال رشد است. برخی از مهمترین آنها:
<p/>
<p dir="RTL">
DNS: تمام کلاستر های Kubernetes باید دارای کلاستر DNS باشند. این یک ویژگی اجباری است Cluster DNS علاوه بر سایر سرورهای DNS موجود در محیط شما، یک سرور DNS است که سوابق DNS را برای خدمات Kubernetes ارائه می دهد. کانتینرهای شروع شده توسط Kubernetes بطور خودکار شامل این سرور DNS در جستجوی DNS می شوند.
<p/>
<p dir="RTL">
UI وب: این یک UI با هدف عمومی و مبتنی بر وب برای کلاستر های Kubernetes است. این برنامه به کاربران امکان می دهد برنامه های در حال اجرا در کلاستر و همچنین خود کلاستر را مدیریت و عیب یابی کنند.
<p/>
<p dir="RTL">
نظارت بر منابع کانتینر: تهیه یک برنامه کاربردی قابل اعتماد و قادر به مقیاس کردن آن در پاسخ به بارهای کاری، به معنای قادر به نظارت مداوم و مؤثر بر عملکرد بار کار است. نظارت بر منابع کانتینر این قابلیت را با ضبط معیارهای مربوط به کانتینر در یک پایگاه داده مرکزی فراهم می کند و UI را برای مرور آن داده ها فراهم می کند. cociation یک جزء در گره برده است که قابلیت نظارت متریک محدود را فراهم می کند.Complete pipelines اندازه گیری نیز وجود دارد، مانند پرومتئوس، که می تواند اکثر نیازهای نظارت را برآورده کند.
<p/>
<p dir="RTL">
ورود به سیستم در سطح کلاستر: گزارش های مربوط باید مستقل از گره ها، Pod ها یا کانتینر دارای انبار و چرخه زندگی جداگانه باشند. در غیر این صورت، خرابی گره یا Pod می تواند باعث از بین رفتن داده های رویداد شود. توانایی انجام این کار، ورود به سیستم در سطح کلاستر است و چنین مکانیسم هایی مسئول ذخیره نگارش کانتینر در یک فروشگاه مرکزی مرکزی با رابط جستجو / مرور هستند. Kubernetes هیچ راه حل ذخیره سازی بومی را برای داده های log فراهم نمی کند، اما می توان بسیاری از راه حل های ورود به سیستم موجود را در کلاستر Kubernetes ادغام کرد.
<p/>

Moein Madadi - 99102229 _ Erfan Asadi  - 99170359 _ Amir Aflatoonian - 99101151
