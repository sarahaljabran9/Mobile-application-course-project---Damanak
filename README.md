Damanak (ضمانك) — Receipt & Warranty Keeper
An Android app that keeps household receipts and warranties in one place, syncs them to the user's account, and sends reminders before a warranty expires.
CSC 402 — Mobile Application Programming · Term Project · Group 04 Imam Abdulrahman Bin Faisal University · College of Science and Humanities, Jubail
The problem
Warranties are often proven by paper receipts. Thermal receipts fade, receipts get lost, and users forget when their coverage ends. Repairs that should be covered end up being paid for.
If the records live only on one phone, a lost, broken or reset phone erases every warranty with it.
The solution
Damanak keeps a digital record of every product, its receipt and its warranty. It calculates each expiry date, shows each product's status at a glance, and sends reminders before coverage ends. Data is saved on the device first, so the app works offline, and is synced to the user's account so the record survives a lost or new phone.
Features
Feature Priority
Account and sync — sign up / sign in, records synced to the user's account Must
Add a product and capture its receipt with the camera Must
Automatic warranty status (active / expiring soon / expired) Must
Reminders at 30, 7 and 1 day before expiry Must
Home screen ordered by nearest expiry, with status indicators Must
Product details with the receipt and a service history log Must
Search, filter and categories Should
Receipt text extraction (OCR) Could
Tech stack
Language: Kotlin
UI: Jetpack Compose · Material 3
Architecture: UI / Domain / Data layers with Unidirectional Data Flow
Local storage: Room (single source of truth for the UI)
Accounts and cloud sync: Firebase Authentication · Cloud Firestore · Firebase Storage
Camera: CameraX
Background work: WorkManager (sync and expiry reminders)
State: ViewModel + StateFlow
Navigation: Navigation Compose
Minimum SDK: 24 · Target SDK: 34
Design and architecture (Milestone 2)
Clickable prototype: Figma (https://www.figma.com/design/YBJto06E71RQctkfAPajdx)
Screens: docs/wireframes/
Navigation map: docs/navigation-map.png
Architecture diagram: docs/architecture.png · docs/architecture.md
Style guide: docs/style-guide.md
Jetpack components: docs/tech-stack.md
AI use log: docs/ai-use-log.md
Project structure
