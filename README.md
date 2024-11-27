
## برنامه v2rayNG برای گوشی
- این برنامه باید از گوگل پلی نصب شود. [لینک نصب از گوگل پلی](https://play.google.com/store/apps/details?id=com.v2ray.ang)
- در صورتی که به هر دلیل دسترسی به گوگل پلی مقدور نبود، می‌توان آن را مستقیم دانلود و نصب کرد. اما باید هر چند وقت یکبار آپدیت شود.
    - [دریافت مستقیم آخرین نسخه](https://github.com/2dust/v2rayNG/releases/download/1.9.16/v2rayNG_1.9.16_arm64-v8a.apk)  
    - [آخرین نسخه‌های منتشر شده](https://github.com/2dust/v2rayNG/releases)
    - پیشنهاد می‌شود در صورت نصب برنامه از قبل، یکبار آن را حذف و دوباره نصب کنید تا تنظیمات اشتباه حذف گردد.


### روش تنظیم برنامه برای گوشی
- ابتدا محتویات کانفیگ را به طور کامل کپی کنید، سپس وارد برنامه شده و دکمه بعلاوه در بالا را بزنید. سپس گزینه Import config from clipboard را بزنید. در صورت نیاز این کار را تکرار کنید.
- برای اتصال به هر کانفیگ آن را انتخاب کرده و دکمه اتصال را بزنید.
- ![image](https://github.com/user-attachments/assets/4115fd84-1e60-46e4-953e-1a45eb873d7e)



### تنظیمات تکمیلی
- برای اتصال همزمان به سایت‌های داخلی، این بخش بعدا بروز می‌شود.



## برنامه v2rayN برای کامپیوتر
- آخرین نسخه از این برنامه را دریافت کنید: [لینک دریافت مستقیم](https://github.com/2dust/v2rayN/releases/download/7.1.3/v2rayN-windows-64-With-Core.zip)
- [آخرین نسخه‌های منتشر شده](https://github.com/2dust/v2rayN/releases)
- آن را از حالت فشرده خارج کرده و پوشه را در یک مکان دائمی ذخیره کنید.
- برنامه را اجرا کرده سپس محتویات هر کدام از کانفیگ‌ها را کپی و با زدن کلید ctrl+v در داخل برنامه پیست کنید.
- برای فعال کردن هر کانفیگ آن را انتخاب کرده و کلید enter‌ را بزنید تا به رنگ آبی در بیاید.
- یکبار دکمه آپدیت را بزنید و صبر کنید تا برنامه به طور کامل به‌روز شود. این کار را هر چندوقت یکبار تکرار کنید.


### تنظیمات تکمیلی
- برای اتصال همزمان به سایت‌های داخلی، ابتدا محتویات زیر را بطور کامل کپی کنید. سپس وارد بخش تنظیمات شوید و بعد Routing setting را بزنید. سپس دکمه Advanced function و بعد گزینه Add را بزنید. حالا گزینه Import rules from clipboard را بزنید تا تنظیمات وارد شود. حالا از بخش بالا و در قسمت Remarks نام Iran Rules را وارد و دکمه تایید را بزنید. سپس تنظیم وارد شده را انتخاب و دکمه enter را بزنید تا به رنگ آبی در آمده و فعال شود.
- ![image](https://github.com/user-attachments/assets/ad360543-b182-4e3a-8254-c1531a28a00c)


```
[
  {
    "Port": "",
    "OutboundTag": "direct",
    "Ip": [
      "geoip:private"
    ],
    "Domain": [
      "geosite:private"
    ],
    "Process": [],
    "Enabled": true,
    "Remarks": "Bypass Local IP/Domain"
  },
  {
    "Port": "",
    "OutboundTag": "direct",
    "Ip": [],
    "Domain": [],
    "Protocol": [
      "bittorrent"
    ],
    "Process": [],
    "Enabled": true,
    "Remarks": "Bypass Bittorrent"
  },
  {
    "Port": "",
    "OutboundTag": "direct",
    "Ip": [
      "117.50.60.30",
      "52.80.60.30"
    ],
    "Domain": [],
    "Process": [],
    "Enabled": true,
    "Remarks": "Bypass Special IPs(Sample)"
  },
  {
    "Port": "",
    "OutboundTag": "block",
    "Ip": [],
    "Domain": [
      "geosite:category-ads-all"
    ],
    "Process": [],
    "Enabled": true,
    "Remarks": "Block Ads"
  },
  {
    "Port": "",
    "OutboundTag": "direct",
    "Ip": [],
    "Domain": [
      "domain:doh.pub",
      "domain:onedns.net"
    ],
    "Process": [],
    "Enabled": true,
    "Remarks": "Bypass Iran/ISP Public DNS"
  },
  {
    "Port": "",
    "OutboundTag": "direct",
    "Ip": [
      "geoip:ir"
    ],
    "Domain": [
	  "geosite:category-ir",
      "regexp:.+.ir$"
    ],
    "Process": [],
    "Enabled": true,
    "Remarks": "Bypass Iran IP/Domains"
  },
  {
    "Port": "443",
    "Network": "udp",
    "OutboundTag": "block",
    "Ip": [],
    "Domain": [],
    "Process": [],
    "Enabled": false,
    "Remarks": "Block UDP 443(Disabled)"
  },
  {
    "Port": "0-65535",
    "OutboundTag": "proxy",
    "Ip": [],
    "Domain": [],
    "Process": [],
    "Enabled": true,
    "Remarks": "Final Agent"
  }
]
  ```
  


