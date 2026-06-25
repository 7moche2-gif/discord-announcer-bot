# Discord Announcer Bot

بوت ديسكورد يرسل كل رسالة تُكتب في روم محددة كـ DM خاص لجميع أعضاء السيرفر.

## المميزات

- /setroom — تحديد الروم المخصصة للإعلانات (للمشرفين فقط)
- /showroom — عرض الروم المحددة حالياً
- /clearroom — إلغاء تحديد الروم
- دعم (منشن) — يتحول لمنشن الشخص المُرسَل إليه
- دعم الايموجيات الخاصة بالسيرفر تلقائياً
- دعم المرفقات والصور
- ريأكشن ✅ على الرسالة الأصلية بعد الإرسال

## النشر على Railway

### 1. إعداد البوت على Discord
1. روح https://discord.com/developers/applications
2. New Application → Bot → Add Bot → انسخ الـ Token
3. فعّل Server Members Intent و Message Content Intent

### 2. دعوة البوت للسيرفر
OAuth2 → URL Generator:
- Scopes: bot, applications.commands
- Permissions: Read Messages, Send Messages, Add Reactions

### 3. النشر على Railway
1. railway.app → New Project → Deploy from GitHub repo
2. اختر discord-announcer-bot
3. أضف المتغيرات:
   - DISCORD_TOKEN = توكن البوت
   - GUILD_ID = ايدي سيرفرك

## طريقة الاستخدام

1. اكتب /setroom واختر الروم
2. أي رسالة تكتبها في تلك الروم تُرسل كـ DM لجميع الأعضاء

مثال على (منشن):
مرحباً (منشن)! عندنا اجتماع الليلة
