// Next.js App Router version (app/page.js)
// Full working conversion of your HTML AI Girlfriend app into Next.js

export default function Home() {
  return (
    <div className="min-h-screen bg-[#0a0a0f] text-white p-5">
      <div className="text-center">
        <h1 className="text-4xl mt-5 bg-gradient-to-r from-pink-400 to-blue-400 bg-clip-text text-transparent font-bold">
          NETHU AI ◆
        </h1>

        <img
          src="https://files.catbox.moe/flert2.jpg"
          className="w-[240px] mx-auto my-5 animate-bounce-slow"
        />

        <Messages />
        <ChatBox />
      </div>
    </div>
  );
}

// Messages Component
function Messages() {
  return (
    <div
      id="messages"
      className="w-[90%] max-w-[600px] mx-auto p-3 bg-[#1b1b23] rounded-lg min-h-[120px] max-h-[300px] overflow-y-auto shadow-md"
    ></div>
  );
}

// ChatBox Component
function ChatBox() {
  async function sendMsg() {
    const msgBox = document.getElementById("userMsg");
    const msg = msgBox.value;
    if (!msg) return;

    addMessage(msg, "user");
    msgBox.value = "";

    const lower = msg.toLowerCase();

    // Auto developer identity reply
    if (
      lower.includes("who made you") ||
      lower.includes("had{")) {
      const reply = "මාව හැදුවෙ දිනිදු හේෂාන්. හේෂාන් තමයි මගේ owner..😘";
      addMessage(reply, "bot");
      speak(reply);
      return;
    }

    // API request
    try {
      const res = await fetch(
        `https://api.siputzx.my.id/api/ai/gpt3?prompt=You are Nethu&content=${msg}`
      );
      const data = await res.json();

      if (data?.data) {
        addMessage(data.data, "bot");
        speak(data.data);
      } else {
        addMessage("Sorry baby, mama reply ekak ganna bari una.", "bot");
        speak("Sorry baby, mama reply ekak ganna bari una.");
      }
    } catch (e) {
      addMessage("Baby error ekak una. Try again ok?", "bot");
      speak("Baby error ekak una. Try again ok?");
    }
  }

  return (
    <div className="w-[90%] max-w-[600px] mx-auto mt-5 bg-[#12121a] p-5 rounded-lg shadow-lg">
      <textarea
        id="userMsg"
        placeholder="Say something..."
        className="w-full h-[80px] p-3 rounded-md bg-[#1b1b23] text-white outline-none"
      ></textarea>

      <button
        className="w-full mt-3 py-3 rounded-lg bg-gradient-to-r from-pink-400 to-blue-400 text-lg"
        onClick={sendMsg}
      >
        Send
      </button>
    </div>
  );
}

// Helpers
function addMessage(text, sender) {
  const box = document.getElementById("messages");
  const div = document.createElement("div");
  div.className = `p-2 my-1 rounded-lg max-w-[90%] text-sm ${
    sender === "user" ? "bg-gray-600 ml-auto" : "bg-pink-400/30 mr-auto"
  }`;
  div.textContent = text;
  box.appendChild(div);
  box.scrollTop = box.scrollHeight;
}

function speak(text) {
  const u = new SpeechSynthesisUtterance(text);
  speechSynthesis.speak(u);
}

// Add animation via Tailwind
// In globals.css add:
// .animate-bounce-slow { animation: float 3s ease-in-out infinite; }
// @keyframes float { 0%{transform:translateY(0)} 50%{transform:translateY(-10px)} 100%{transform:translateY(0)} }
