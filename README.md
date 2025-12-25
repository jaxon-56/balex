# Balex v1.0

**Async Python library for Bale Messenger bots** 🚀

نسخه ۱ Balex برای ارسال پیام و ست وب‌هوک طراحی شده است و کاملاً Async می‌باشد.  
.

---

## نصب

```bash
pip install balex

## نمونه کد
```bash
import asyncio
from balex.client import BaleClient

async def main():
    async with BaleClient("Token") as bot:
        await bot.send_message(1234666, "سلام از Balex v1.0 🚀")
        await bot.set_webhook("https://yourserver.com/balex_webhook")

asyncio.run(main())
