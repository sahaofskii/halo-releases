# Halo

A simple VPN client for Windows, built on Xray and sing-box. Paste your subscription link, press connect, and Halo picks the best server for you.

<div dir="rtl">

یک کلاینت VPN ساده برای ویندوز، ساخته‌شده روی Xray و sing-box. لینک اشتراک را وارد کنید، دکمه‌ی اتصال را بزنید؛ Halo بهترین سرور را خودش انتخاب می‌کند.

</div>

## Download · دانلود

Get the newest version from **[Releases](../../releases/latest)**.

| File | For |
|---|---|
| `Halo-Setup-<version>.exe` | **Most people.** Installs Halo, updates itself from inside the app. |
| `Halo-Portable-<version>.zip` | No install: unzip and run `Halo.exe`. Settings stay in its own folder. |

<div dir="rtl">

| فایل | برای چه کسی |
|---|---|
| `Halo-Setup-<version>.exe` | **بیشتر کاربران.** Halo را نصب می‌کند و از داخل برنامه به‌روز می‌شود. |
| `Halo-Portable-<version>.zip` | بدون نصب: از حالت فشرده خارج کنید و `Halo.exe` را اجرا کنید. تنظیمات در پوشه‌ی خودش می‌ماند. |

</div>

Windows 10 (1809) or newer, 64-bit.

## Check the file · بررسی فایل

Each release has a `SHA256SUMS.txt`. In PowerShell:

```powershell
Get-FileHash .\Halo-Setup-<version>.exe -Algorithm SHA256
```

The hash must match the line for that file. Halo also checks every update it installs against its own signature.

<div dir="rtl">

هر انتشار یک فایل `SHA256SUMS.txt` دارد. خروجی دستور بالا باید با خط همان فایل یکی باشد. خود Halo هم هر به‌روزرسانی را قبل از نصب با امضای خودش بررسی می‌کند.

</div>

## License

Halo is free software under the GPL-3.0. It includes sing-box (GPL-3.0), Xray-core (MPL-2.0) and Wintun; their licenses are in the `licenses` folder of every download.
