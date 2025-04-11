# **AI Content Generator App - Documentation**  

## **📌 Overview**  
The **AI Content Generator App** is a web-based application that leverages artificial intelligence to generate various types of content, such as blog posts, marketing copy, social media captions, and more. Built with modern web technologies, it offers a fast, responsive, and user-friendly experience.  

---

## **🛠️ Tech Stack**  
| Technology | Purpose |  
|------------|---------|  
| **Vite** | Ultra-fast build tool for React & TypeScript |  
| **TypeScript** | Adds static typing for better code reliability |  
| **React** | Frontend framework for building dynamic UIs |  
| **shadcn-ui** | Reusable, accessible UI components |  
| **Tailwind CSS** | Utility-first CSS framework for styling |  

---

## **✨ Features**  
1. **AI-Powered Content Generation**  
   - Generate text based on user prompts (e.g., blog posts, ads, tweets).  
   - Supports different content tones (professional, casual, persuasive).  

2. **Responsive & Modern UI**  
   - Clean, minimalist design with **dark/light mode** support.  
   - Built with **shadcn-ui** components for consistency.  

3. **Fast Performance**  
   - Optimized with **Vite** for near-instant HMR (Hot Module Replacement).  

4. **Type Safety**  
   - Reduces bugs with **TypeScript**-enforced types.  

---

## **🚀 Installation & Setup**  
### **Prerequisites**  
- Node.js (v18+)  
- npm / yarn / pnpm  

### **Steps**  
1. **Clone the repository**  
   ```bash
   git clone https://github.com/yourusername/ai-content-generator.git
   cd ai-content-generator
   ```

2. **Install dependencies**  
   ```bash
   npm install  # or yarn / pnpm install
   ```

3. **Run the development server**  
   ```bash
   npm run dev
   ```

4. **Open in browser**  
   Visit `http://localhost:5173`  

---

## **📂 Project Structure**  
```bash
src/  
├── assets/           # Images, icons, etc.  
├── components/       # Reusable React components  
├── lib/              # Utility functions, API calls  
├── styles/           # Global CSS/Tailwind config  
├── App.tsx           # Main App component  
└── main.tsx          # Vite entry point  
```

---

## **🔌 API Integration**  
The app connects to an **AI API** (e.g., OpenAI GPT, Hugging Face) for content generation.  

### **Example API Call (using OpenAI)**  
```ts
import OpenAI from "openai";

const openai = new OpenAI({ apiKey: "YOUR_API_KEY" });

async function generateContent(prompt: string) {
  const response = await openai.chat.completions.create({
    model: "gpt-3.5-turbo",
    messages: [{ role: "user", content: prompt }],
  });
  return response.choices[0].message.content;
}
```

---

## **🎨 UI Components (shadcn-ui + Tailwind)**  
- **`<Button />`** – Interactive buttons with variants.  
- **`<Input />`** – Stylish input fields for prompts.  
- **`<Card />`** – Displays generated content.  
- **Dark/Light Mode** – Toggleable theme using `next-themes`.  

---

## **📜 License**  
MIT License – Free to use, modify, and distribute.  

---

### **💬 Feedback & Contributions**  
Feel free to open **issues** or **PRs** if you have suggestions!  

🚀 **Happy Coding!** 🚀  

