# AIBhai 🤖🇮🇳 — Level-3 Personal AI Agent for Android

AIBhai ek **offline-first voice assistant** hai jo power/home button long-press pe khulta hai,
Hindi, Hinglish, English, Haryanvi aur Bhojpuri samajhta hai, aur phone pe **asli kaam** karta hai —
sirf chat nahi.

## Level-3 Agent (chatbot nahi)
| Capability | AIBhai mein |
|---|---|
| Missing data pe rukna | File/folder/time na bolo to poochta hai, guess nahi karta |
| Human approval | Bulk file move, unsure call → pehle plan dikhata hai, "Haan" pe hi karta hai |
| Verify results | File move ke baad disk pe check karta hai → `✓ VERIFIED` |
| Action log | Har command ka record: kya suna, kaunsa skill, result, status |
| Error handling + Undo | Galti pakadta hai, file actions wapas kar sakta hai |
| Learning | "Sikhao" se apne words sikhao (Haryanvi/Bhojpuri bhi) |

## 🌐 Online + 📴 Offline (hybrid)
Internet ho to online features, na ho to apne aap offline: on-device speech, Google offline voice, saare phone/file/study kaam. News/update jaise internet wale kaam **queue** mein jaate hain aur internet aate hi khud ho jaate hain. Offline mein pichli saved news & attendance dikhti hai.

## Features
- 📬 **Important messages** — "Bhai aaj kaun se message aaye?" (WhatsApp/SMS/Gmail/Classroom ko score karke important batata hai, OTP chhupata hai)
- 📝 **Aaj ke kaam** — "Aaj mujhe assignment aur gym karna hai" → "Aaj kya karna hai?" → "Assignment ho gaya"
- 🗂️ **Files** — "Communication wali PDF ko English folder mein daalo", "Downloads organize karo", "WhatsApp ke notes collect karo", Undo
- 📊 **Attendance** — "Aaj Maths attend kiya", "Attendance batao" (75% ke liye kitni class chahiye)
- 🎓 **College portal** — "Maths ki attendance kitni hai?" / "Overall attendance batao" → AIBhai portal (Okie Dokie) kholke % padhta hai aur bolke batata hai
- ⏰ **Alarm / Timer / Reminder** — "Kal subah saade 6 baje alarm", "10 minute baad yaad dilana ki chai"
- 📞 **Call / WhatsApp** — "Papa ko call karo", "Rahul ko WhatsApp pe bolo main aa raha hoon"
- 🧮 **Engineering calc** — stress (F/A), Ohm's law, EV range (kWh, Wh/km), km/h→m/s, maths
- 🔦 Torch, 🔊 volume, 📳 class mode, 🔋 battery, 🕐 time/date, apps kholna (Vivo Notes bhi)
- ☀️ **Briefing** — "Good morning" → time, battery, messages, kaam, attendance alerts, reminders
- 📰 **News** — "Aaj ki news kya hai?" → EV & Mechanical updates sabse pehle, phir India + Tech (free Google News, no key). Roz 8 AM notification
- 📕 **Galti Diary** — "Aaj ki galti: der se utha" → top performers ke tareeke + aapka "Solution: …" + pledge, repeat count & clean-streak, roz subah yaad
- 🤖 **Phone control (Accessibility)** — "Screen pe kya hai", "Subscribe pe tap karo", "Scroll karo", "Back jao", "Screenshot lo", "Phone lock karo", kisi bhi app mein type; bank/UPI apps mein kabhi auto-tap nahi
- ⚙️ **Koi bhi setting** — "Display settings kholo", "Battery settings kholo"…
- 📲 **Self-updating** — naye install hue apps khud pehchanta hai; GitHub pe naya version aate hi khud download karke install karwata hai
- 🎙️ **Voices** — Adam & Nidhi: phone ki Google voice (free, unlimited, offline). Optional ElevenLabs premium
- 🌐 Jis language mein poocho, usi mein jawab (Hinglish ↔ English)
- 🖥️ Optional **PC Brain** — Ollama on your PC over Wi-Fi for open questions

## Install (phone se)
1. `Releases` → latest → **AIBhai.apk** download → Install (Unknown apps allow karo)
2. App kholo → **Settings** → saari permissions **Allow**
3. Vivo: Settings → Apps → Default apps → **Digital assistant app → AIBhai**
4. Power button long-press → AIBhai 🎉

## Build
Har push pe GitHub Actions khud APK banata hai (`.github/workflows/build.yml`). Local: `./gradlew assembleDebug`.

Stack: Kotlin · Jetpack Compose · Android SpeechRecognizer · TextToSpeech · ElevenLabs · VoiceInteractionService · NotificationListenerService
