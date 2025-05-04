# 🚀 Hack Connect – Social fun for hackers during hackathons

**Hack Connect** is a web app designed to boost fun, connection, and creativity during hackathons. It transforms downtime and stress moments into opportunities to meet fellow hackers, complete quick challenges, and engage with the community — all while keeping the hackathon spirit alive.

> Project developed for **HackUPC 2025** 🧠💻


## 📱 What is Hack Connect?

Hack Connect is an interactive web platform that brings a playful and social layer to hackathon events. It allows participants to take short breaks, complete challenges, connect with others, and personalize their experience using AI tools.

Whether you want to take a break from debugging, meet like-minded hackers, or add a creative twist to your project, Hack Connect is the place to go.

## 🎯 What can you do with Hack Connect?

* 🧩 **Complete Fun Challenges**: Engage in short, creative challenges that earn you points and help you interact with others.
* 🏆 **Scoreboard**: Track your points and see who’s topping the leaderboard — a friendly competitive twist to keep things exciting!
* 💻 **Create Your Project**: Share what you're building with the community by registering your project in the app.
* 😄 **Generate Funny Avatars**: Upload a photo and get an AI-generated, diffusion-based fun avatar to spice up your profile.
* 🤖 **Let AI Name Your Project**: Use our name generator powered by LLMs to get creative, personalized project name suggestions.
* 🌐 **Connect with Like-Minded Hackers**: Discover people with shared programming languages, countries, or hobbies — perfect for networking and making friends.

## ⚙️ How does it work?

Hack Connect is built using modern web technologies and generative AI models to provide a seamless and engaging experience:

* **Backend**: FastAPI
* **Frontend**: React
* **Database**: PostgreSQL
* **AI Services**:

  * Diffusion models for avatar generation
  * LLM with GeminiAI for project name generation
* **Authentication**: Magic links via hackathon QR (no passwords!)

---

## 📦 How to install and run it

To run the app locally:

1. **Clone the repositories:**

```bash
git clone https://github.com/HackConnectTeam/frontend
git clone https://github.com/HackConnectTeam/backend
```

2. 🧠 **Set Up the Environment**.
   - Install Docker and Docker Compose.
   - Run a Cloudflare container to expose the application to the internet by tunelling:
     ```bash
     docker run --network host cloudflare/cloudflared:latest tunnel --no-autoupdate run --token
     eyJhIjoiNmMxN2NlMTM1ZDY4NTc0MGJmYmE4NjUxODAzNDA0NTciLCJ0IjoiYjQ3Mzc1OTYtZmU0MS00NDIwLWEyODQtY
     mFhYjczZGE4YTI4IiwicyI6Ill6RmpaamxoWlRrdE1qRmxNeTAwWkRjMUxUazVNak10WlRsbVkyVXdaVFJqWVdWbSJ9
     ```
   - Run these commands in the Frontend folder:
     ```bash
     npm install
     npm run dev
     ```
   - Create a `.env` file with the necessary environment variables. More information can be found in the [Environment Variables](#-environment-variables) section.
   - Run the Docker containers using Docker Compose:
     ```bash
     docker-compose up -f devops/docker-compose.yml up --build
     ```
3. 🚀 **Access the Application**.
   - Navigate to https://hackconnect.lamelas24.com and enjoy!

> ⚠️ Make sure required API keys are properly set.

---

## ❓ What works and what doesn’t?

✅ **What works:**

* Challenge system and scoreboard
* Avatar and project name generation via AI
* User profiles and matchmaking
* Project creation and sharing

🚧 **What doesn’t (yet):**

* 🖼️ Avatar display: Avatar generation works via the diffusion model, but the generated image is not yet displayed in the frontend.

* 🧑‍💻 GitHub language integration: We implemented a feature to automatically fetch programming languages from a user’s GitHub repositories, but it wasn’t fully tested during the hackathon.

* ✅ Challenge tracking: Users can complete challenges and gain points, but the list of completed challenges is not visible yet on their profiles.

---

## 🤔 Where to ask questions or report issues?

If you run into problems or have suggestions, feel free to:

* Open an issue on [Frontend Repo](https://github.com/HackConnectTeam/frontend/issues) or [Backend Repo](https://github.com/HackConnectTeam/backend/issues)
* Contact the team:

  * Pablo Boo Iglesias – pabloboocastrofeito@gmail.com
  * Antón Canzobre Martínez – antoncanzobremar@gmail.com
  * Alejandro Dopico Castro – alejandro.dopico2@udc.es
  * Alejandro García García – alejandro.garcia11@udc.es

---

## 🤝 How to contribute

We’d love to see this grow! To contribute:

1. Fork the repo.
2. Create a new branch: `git checkout -b feature/amazing-feature`
3. Commit your changes: `git commit -m "Add amazing feature"`
4. Push and open a Pull Request.

Feel free to reach out with ideas!

---

## 👥 Who built Hack Connect?

Hack Connect was developed during HackUPC 2025 by:

* Pablo Boo Iglesias
* Antón Canzobre Martínez
* Alejandro Dopico Castro
* Alejandro García García

---

## 📄 License

This project is licensed under the **MIT License**, which allows reuse, modification, and distribution with minimal restrictions.

---

## 🙌 Special Thanks

Thanks to the amazing **HackUPC 2025 organizers** for making this event possible, and to all the **mentors** for their help, insights, and support throughout the hackathon.
