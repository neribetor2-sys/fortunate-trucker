Project: Apartment Furniture & Appliances Tracker 🏠
Core Purpose
A shared web application for a couple (Neri & Noa) to track furniture and appliance purchases for a new apartment. The goal is tracking ongoing expenses and progress, without debt calculation.

Tech Stack
Architecture: Single-file index.html (HTML5, CSS3, Vanilla JavaScript).

Storage: LocalStorage (Current) / Firebase-ready (Future).

Direction: RTL (Right-to-Left) for Hebrew support.

UI & Design Rules
Language: Entire UI must be in Hebrew (עברית).

Layout: Mobile-first, clean, modern cards using CSS variables for a "Teal/Mint" theme.

Visual Cues: Every item card MUST display two emojis:

Category Emoji: Based on the type of item.

Room Emoji: Based on where it belongs in the house.

Data Schema (Item Object)
id: Unique string.

title: Name of the item.

category: [ריהוט, מוצרי חשמל, טקסטיל, תאורה, אקססוריז, תחזוקה/גינון, כלי מטבח].

room: [חדר שינה, משרד, חדר אמבטיה ראשי, חדר אמבטיה שני, מסדרון, סלון, מרפסת, מטבח].

priority: [חייב להיות, נחמד לקבל].

status: [לקנייה, הוזמן, סופק].

estPrice / actualPrice: Numbers.

payer: [neri, noa, משותף].

dimensions: [Length, Width, Height].

imageUrl, storeLink, deliveryDate, notes.

Dashboard Requirements
Spending by Category: List with percentages of total actual spending.

Room Completion: Progress bars for each room showing '% Delivered' based on item count.

Total Stats: Items purchased vs. Total, Total spent so far, Projected costs for remaining items.

Simplification: Do NOT show "Savings" or "Must-have pending" sections unless requested.

Mapping Logic
Room Emojis

חדר שינה: 🛏️, משרד: 🖥️, חדר אמבטיה ראשי: 🛁, חדר אמבטיה שני: 🚿, מסדרון: 🚪, סלון: 🛋️, מרפסת: 🪴, מטבח: 🍳.

Category Emojis

ריהוט: 🛋️, מוצרי חשמל: ⚡, טקסטיל: 🧶, תאורה: 💡, אקססוריז: 🖼️, תחזוקה/גינון: 🛠️, כלי מטבח: 🍴.

Development Commands
The project is a static index.html. No npm install or npm run dev required.

Use Live Server in VS Code to preview.

To deploy: Use Vercel (drop the index.html file).
