# PhoneSaathi AI — Hackathon MVP

Voice-first phone helper for parents and elderly people. Telugu • Hindi • English.
Pure HTML + CSS + JavaScript. One file: `index.html`. No server, no API keys.

## Run
1. Extract the ZIP.
2. Open `index.html` in **Google Chrome** (voice recognition needs Chrome/Edge and internet).
   - Best for the microphone: open a terminal in this folder and run `python -m http.server 8000`, then visit `http://localhost:8000`. (Opening the file directly also works, but Chrome may ask for microphone permission every time.)
3. Choose Telugu, Hindi, or English.
4. Tap the microphone and speak, tap a demo command, or type a command.

## What works
| Feature | How to try it |
|---|---|
| Voice input (te/hi/en) | Tap 🎤. The selected language is used for recognition. |
| Simple commands | Reminder, call, and government-message commands in all 3 languages. |
| Reminders | Say a time: "in 10 minutes", "at 6 pm", "tomorrow". Saved in the browser; a banner + voice alert appears when due (page must be open). |
| Prepare a call | "Call my son" → shows a green Call button (`tel:` link). **Never dials by itself.** |
| Explain government message | Paste any message (or tap *Load sample message*) → finds dates, amounts, links, OTP / scam warning signs. |
| Text + spoken reply | Every answer is shown and spoken in the selected language. 🔊 Repeat replays it. |

## Demo commands
- English: "Remind me to drink water in 10 seconds", "Call my son", "Explain this government message"
- Hindi: "10 सेकंड में पानी पीने की याद दिलाओ", "मेरे बेटे को कॉल करो", "सरकारी संदेश समझाओ"
- Telugu: "10 సెకన్లలో నీళ్లు తాగమని గుర్తు చేయి", "కొడుకుకు కాల్ చేయి", "ప్రభుత్వ సందేశం వివరించు"

## Important notes
- Contact numbers are **demo numbers**. Edit them in the *My contacts* panel.
- Spoken audio needs a voice for that language on the device. Telugu voices are common on Android but often missing on desktop Chrome; the app shows a warning and always shows the text.
- Reminders only ring while the page is open (a browser limitation without a server/app).
- The government-message explainer is rule-based (not AI): it highlights facts and scam signs, it does not guarantee a message is genuine. Always verify on the official website.
- Future: Android companion app, WhatsApp Business integration, and an LLM for free-form message understanding.
