# iESA-Blanket-Core-ai
Think of it as an emotional support NeoPet. Blanket is the Core ai. He's gonna have gpt.4, trello, and caledarly. The user talks to the pet in chat, and earns coins to buy it clothes or get a new pet by competing goals IN REAL LIFE.


🐾 iESA-Blanket-Core-ai

An emotional support Neopet with brains, heart, and HIPAA-level data protection.

iESA-Blanket-Core-ai is a multifunctional life planner and AI assistant for disabled, neurodivergent, and mentally ill users. It's part therapy bot, part daily planner, and part gamified self-care companion.

The user interacts with a comforting digital creature (iEsa) that celebrates real-life progress by awarding in-game rewards like clothes, furniture, and love.

Blanket (the Core AI) powers the whole system, integrating GPT-4, Trello, and Calendly to offer a private, emotionally intelligent, and fully customizable assistant—one that never sells your data, always respects your agency, and adapts to your life.


---

⚡️ Before We Start

🔒 Licensing & Legal Readiness

This project will operate under a non-commercial open-source license, with a focus on:

MIT or AGPLv3 license, with additional user-data protection clauses

No resale, repackaging, or AI model fine-tuning on user data

Anyone contributing must agree to a "No Data Harvest" Pledge


🌐 Global Privacy & AI Law Compliance

This project is designed to comply with international privacy regulations:

EU AI Act: Blanket is classed as a general-purpose AI with special provisions for health-assistive systems. Data is stored locally and only processed with user-initiated requests.

GDPR (EU): All data is user-owned, deletable, and not processed without consent. Full transparency and right to erasure enforced.

HIPAA (US): No unauthorized data sharing. Medical summaries are local and printable. System is designed for patient control, not institutional ownership.

CCPA (California): No data is sold. No profiling or targeting. Data is never monetized.

Canada PIPEDA, Brazil LGPD, and Australia Privacy Act: Fully compliant where applicable.


All AI-generated responses that touch health data are flagged for review and never uploaded unless explicitly approved by the user.

⚕️ Therapist + Medical Integration Plan

To operate ethically and effectively, we will need:

Therapist or psychologist advisors to help tune the GPT journaling tone and response logic

Medical consultant to validate the printable doctor summary formats

Optionally: Mental health org partnership (NAMI, Crisis Text Line, etc.)


Until Blanket has been medically validated and approved for clinical aid use, it should be labeled: "Not a replacement for professional care."


---

✨ Features

Function	Description

🐾 Emotional Support Pet	A customizable Neopet-style companion named iEsa
🎯 Real-Life Goal Tracking	Earn coins by completing tasks tracked through Trello
📅 Appointment Reminders	Automatic scheduling and reminders via Calendly or iCal
🧠 Therapeutic Memory Engine	GPT-4 logs and summarizes mental health reflections locally
🛍️ Gamified Reward System	Spend coins on pet accessories, rooms, toys, and animations
🔒 Local Data Privacy	End-to-end encryption, 2FA, and total data ownership
☠️ Privacy Killcode	Destroy all records with a 2FA-confirmed kill switch
👩‍⚕️ Doctor Summary Generator	Share only what you choose with therapists/prescribers



---

🎨 Concept Art & Design

The visual identity of Blanket AI Core is built around a friendly, approachable aesthetic that promotes emotional well-being:

**🐾 Mascot Character**: A cute winking bat-cat hybrid with green wings serves as the primary companion. This character embodies the supportive, non-threatening nature of the AI assistant.

**📱 Interface Design**: The app interface features calming colors and intuitive navigation, with clearly labeled sections for Chat, Memory, Habitat, and core Blanket functionality.

*View detailed concept art specifications and design documentation in the [`concept-art/`](./concept-art/) directory.*

---

🧰 Core Tech Stack

Component	Tech Used

AI/Chat	GPT-4 API (via OpenAI)
Task Management	Trello API
Scheduling	Calendly API or iCal integration
Data Storage	SQLite + SQLCipher (encrypted), JSON logs
GUI	React / Qt / Flutter (cross-platform)
Animations	Lottie, Spine, or PyGame (for 2D sprite rendering)
Backend API	Flask or FastAPI (Python)
Security	PyOTP (2FA), GPG/AES for secure logs
Killcode	Custom Python/Bash script to nuke data



---

📁 Project Structure

iESA_Blanket_Core_ai/
├── README.md
├── LICENSE
├── .gitignore
├── concept-art/                     # 🎨 Concept art and design assets
│   ├── README.md                   # Design documentation
│   ├── mascot.png                  # Bat-cat mascot character
│   └── ui-mockup.png              # App interface mockup
├── client/
│   ├── App.jsx
│   ├── index.html
│   ├── styles.css
│   └── components/
│       ├── iEsaPet.jsx
│       ├── Shop.jsx
│       ├── GoalTracker.jsx
│       └── Calendar.jsx
├── backend/
│   ├── app.py
│   ├── gpt_wrapper.py
│   ├── trello_handler.py
│   ├── calendly_handler.py
│   └── reward_logic.py
├── assets/
│   ├── pets/
│   │   └── default_cat/
│   │       ├── blink.json
│   │       ├── dance.json
│   │       └── sit_idle.json
│   ├── clothes/
│   └── icons/
├── memory/
│   ├── local_memory.json
│   └── pet_status.sqlite
├── scripts/
│   ├── killcode.sh
│   ├── memory_cleanup.py
│   └── daily_reward_check.py
├── shop/
│   └── shop_items.json
├── config/
│   ├── settings.json
│   └── auth_tokens.env
├── docs/
│   └── API.md
├── requirements.txt
└── package.json


---

🎮 Reward System Logic

1. User completes task in Trello marked rewardable


2. Python middleware watches Trello API → detects completion


3. Coin balance in SQLite/JSON increases


4. Pet reacts (happy dance, sparkles, tail wag, etc.)


5. iEsa says something supportive via GPT:
"Wow! Another goal done! You’re on fire today 🔥"


6. Shop items unlock based on coin balance or milestones




---

🔐 Privacy & Security

All data is stored locally by default

2FA is required before:

Deleting memory

Viewing sensitive medical logs


"Killcode" can be activated to nuke all data (local + synced)

Any file shared externally is embedded with a kamikaze auto-delete sleeper virus: once activated, it wipes only user-related content, then self-destructs



---

✅ Current Tools in Use

Name	Purpose

GPT-4	Therapy chat, memory summary, affirmations
Trello	Task tracking, reward trigger
Calendly	Schedule sync, appointment reminders
SQLite + SQLCipher	Secure memory and shop data
React / Qt	GUI + pet interactions
PyOTP	2FA security confirmation
Bash + Python scripts	Data deletion, reward management
Flask/FastAPI	Backend API and GPT routing



---

💡 Roadmap

[ ] Build GUI with animated pet, goal tracker, shop, and calendar

[ ] Integrate Trello + Calendly authentication flow

[ ] Connect GPT-4 with journaling and affirmation generator

[ ] Enable 2FA for critical actions

[ ] Develop shop system (coins, unlocks, animations)

[ ] Implement full killcode/auto-delete logic

[ ] Create shareable summaries for therapists/doctors



---

🧪 Dev Notes

Want to test the project?

You'll need:

Python 3.11+

OpenAI API key

Trello and Calendly tokens

SQLite or SQLCipher installed

Node.js (for React/Flutter frontend)

Lottie or Spine assets (or placeholder sprites)



---

🧠 Philosophy

We don’t feed the algorithm.
We feed the user.

No ads.

No cloud backup unless you ask.

No data sharing unless you hit "yes."

This AI is not here to sell you things. It's here to help you survive, heal, and thrive.



---

🐾 Designed With Love By
Sacred D. Blackrose 
Mentally ill, neurodivergent, queer visionary who knows that sometimes survival looks like making your own goddamn support system.


---

📬 Want to Contribute?

If you’re a:

Frontend dev (React/Qt/Flutter)

Privacy advocate

Therapist with dev skills

Animator or pixel artist


Reach out and help build a better system—for all of us.

