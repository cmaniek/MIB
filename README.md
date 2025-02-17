# MIB (Message in a Bottle)

MIB is an experimental real-time messaging project where users can send messages into a shared bottle. Every cycle, one message is randomly selected and displayed for 60 seconds before the process repeats.

## ✨ How It Works

1. Users connect to a WebSocket server.
2. During a time-limited period, users can submit messages through an input field.
3. When the timer reaches zero, a message is randomly selected and displayed for 60 seconds.
4. During this display time, users can submit new messages for the next cycle.
5. At the end of the 60 seconds, another message is selected, and all previous messages are erased.

## 🚀 Tech Stack

### Frontend:
- [Vite](https://vitejs.dev/)
- [react-use-websocket](https://github.com/robtaussig/react-use-websocket)

### Backend:
- [Fastify](https://www.fastify.io/)
- [fastify-websocket](https://github.com/fastify/fastify-websocket)

## 🛠 Installation & Setup

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/yourusername/mib.git
cd mib
```

### 2️⃣ Install Dependencies
#### Backend:
```bash
npm install
```

### 3️⃣ Start the Server
```bash
npm run start
```
The WebSocket server will run at: 
```
ws://localhost:3000/handleMessages
```

### 4️⃣ Setup & Run the Frontend
```bash
cd web
npm install
npm run start
```
This will launch the frontend on `http://localhost:5173/` (default Vite dev server port).

## 📜 License
This project is licensed under the MIT License.

## 💡 Future Improvements
- UI enhancements and animations.
- Onchain integration

---
Made by CManiek with ❤️ for experimentation and fun!

