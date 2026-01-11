🏠 Real Estate AI Assistant – Built with Vibe Coding (Bolt.new)

An experimental MVP built solo, for one goal — help people make smarter real estate decisions in Canada. No big teams. No traditional code. Just a working tool, made with curiosity, fast iteration, and a clear plan.

🔍 What It Does
This tool takes a **property address** and brings together all the info you would normally have to collect from 5 different tabs:

- Recent sold listings nearby
- Property comparison (sqft, year built, garage, basement)
- School ratings and walkability
- Transit access (TTC, GO)
- Closest grocery stores
- Auto-written offer justification email using OpenAI

All shown in one clean, simple view.

🧱 How It’s Built (Architecture)
This was a vibe-coded build — done using drag-and-drop tools and simple backend functions. Still, there’s structure behind it.

⚙️ Tech Stack
Frontend:
[Bolt.new](https://bolt.new) for the UI — no-code blocks, logic flows, and real-time preview

Backend / Logic:
- AWS Lambda (Python) to connect APIs and process input
- OpenAI for email generation

Data Sources:
- Google Maps API for nearby amenities (schools, transit, groceries)
- RapidAPI: Realty in CA for sold listings
- Fraser Institute school rankings (converted PDF to JSON manually, matched via fuzzy search)

Infra:
- API Gateway for secure HTTPS endpoint
- IAM for permission handling
- Hosted in `ca-central-1` (Canada region)

🧪 How It Works – End to End
1. User enters a property address
2. Address is geocoded → sold listings pulled via RapidAPI
3. Comparison table built for size, age, features
4. Google Maps API fetches nearby schools, transit, groceries
5. Schools matched to Fraser ratings (PDF → JSON → fuzzy search)
6. OpenAI writes the offer email using all collected info

🎯 Why This Project?

I work in project management. So I approached this like a mini project:

Scope: One address → full context
Timeline: 3 weekends
Constraints: No dev team, no fancy stack
Approach: Stay clear, move fast, skip the fluff

Instead of writing long plans, I just started building.

This is what vibe coding taught me — build first, refine later.

🛠 What’s Missing (For Now)
If I bring this forward again, here’s what I’d add:

- User login + saved comparisons
- Mobile-first layout
- PDF contract upload with clause detection
- Rental pricing or zoning overlays

🤝 Acknowledgements
- Fraser Institute Canada (school rating data)
- Bolt.new for helping speed up the UI build
- OpenAI, Google Maps, and RapidAPI for core functionality

Built by Neeraj in Canada.

🚧 Disclaimer

This is not a production app. It’s an MVP experiment. But it works — and it showed me how real-world problems can be tackled with simple tools and a builder mindset.
