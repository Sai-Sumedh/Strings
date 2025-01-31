
# **Strings**

AI System for Tailored Real-time Interactive Narrative Generation and Scriptwriting

---

## **Overview**

Strings is a web application that assists writers in generating dynamic character dialogue, offering two distinct modes:

### **Normal Mode**
- Quick scene setup
- Basic character descriptions
- Straightforward dialogue generation
- Ideal for rapid story development

### **Fine-Grain Mode**
- Detailed character control
- Emotional state management
- Relationship dynamics
- Response length customization
- Advanced dialogue generation for nuanced storytelling

---

## **Technology Stack**
- **Next.js 14**
- **Tailwind CSS**
- **Framer Motion**
- **shadcn/ui**
- **OpenAI API**

---

## **Features**
- Real-time dialogue generation
- Character state management
- Scene context preservation
- Plot development tracking
- Responsive and modern UI design
- Smooth animations
- Custom fonts and styling for enhanced readability

---

## **Getting Started**

Follow these steps to get the application up and running:

### **1. Clone the Repository**
```bash
git clone https://github.com/treydenc/string.git
cd prompt-engineer
```

### **2. Install Dependencies**
```bash
npm install
```

### **3. Set Up Environment Variables**
Create a `.env.local` file in the project root with the following content:
```env
OPENAI_API_KEY=your_api_key_here
```

### **4. Run the Development Server**
```bash
npm run dev
```

The app will be available at `http://localhost:3000`.

---

## **Project Structure**
```plaintext
src/
├── app/
│   ├── (with-header)/     # Pages with header
│   │   ├── page.js        # Landing page
│   │   └── layout.js      # Layout with header
│   ├── (without-header)/  # Pages without header
│   │   ├── fine-grain/    # Fine-grain mode
│   │   │   └── page.js
│   │   ├── normal/        # Normal mode
│   │   │   └── page.js
│   │   └── layout.js      # Layout without header
│   ├── api/               # API routes
│   │   ├── generateDialogue/ # OpenAI Function
│   │   └── generateScene/    # OpenAI Function
│   ├── layout.js          # Root layout
│   └── globals.css        # Global styles
├── components/
│   ├── Header.js          # Site header
│   ├── CharacterPanel.js  # Character management panel
│   └── ui/                # shadcn/ui components
├── services/
│   ├── dialogueAPI.js     # API integration for OpenAI
│   └── sceneAPI.js        # API integration for OpenAI
├── data/
│   └── default.js         # Default configurations
└── lib/
    └── utils.js           # Utility functions
.env.local
```
---

## **Usage**

1. **Select a Mode**: Choose between **Normal Mode** or **Fine-Grain Mode**.
2. **Enter Character Descriptions**: Provide details about your characters.
3. **Set the Scene**: Establish the scene context for the dialogue.
4. **Define Plot Development**: Add relevant plot points.
5. **Generate Dialogue**: Use the AI to create tailored character dialogue.
6. **Refine and Iterate**: Adjust settings to fine-tune the generated content.

---

## **Contributing**
Contributions are welcome! Please submit a pull request or open an issue on GitHub to propose improvements or report bugs.

---

## **License**
This project is licensed under the [MIT License](LICENSE).
