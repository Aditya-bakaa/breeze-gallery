
# 🍃 breeze-gallery

A responsive, high-performance image discovery application built with React and CSS Grid, leveraging the Unsplash API to deliver fluid image searching and dynamic gallery layouts.

---

## 🚀 Features

- **Asynchronous Search:** Real-time communication with the Unsplash API utilizing modern HTTP client structures.
- **Fluid Layout Engine:** Powered by a clean CSS Grid architecture using `auto-fill` and `minmax` patterns to provide perfect mobile-to-desktop responsiveness without structural layout breaks.
- **Robust Exception Handling:** Implements dedicated loading states and proactive network error tracking for an optimal user experience.
- **Secure Key Architecture:** Engineered with clean environment variable configurations to prevent security credential leaks on source control.

---

## 🛠️ Tech Stack

- **Frontend Framework:** React.js (Vite)
- **Styling Engine:** CSS3 (Flexbox, CSS Grid)
- **API Client:** Axios
- **Data Source:** Unsplash Developer API

---

## 📂 Project Architecture

```text
src/
├── components/
│   ├── SearchBar.jsx      # Handles search input logic and form submission
│   ├── ImageGrid.jsx      # The core CSS Grid wrapper engine
│   └── ImageCard.jsx      # Individual item wrapper handling hover effects
├── services/
│   └── unsplash.js        # Isolated API interaction layer (Separation of Concerns)
├── App.jsx                # Main controller handling dynamic React state
└── index.css              # Global styles & responsive grid variables

```

---

## ⚙️ Installation & Setup

Follow these steps to run the project locally:

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/Aditya-bakaa/breeze-gallery.git](https://github.com/Aditya-bakaa/breeze-gallery.git)
   cd breeze-gallery
   ```


2. **Install dependencies:**
```bash
npm install

```


3. **Configure Environment Variables:**
Create a `.env` file in the root directory and add your Unsplash Access Key:
```env
VITE_UNSPLASH_ACCESS_KEY=your_unsplash_access_key_here

```


4. **Launch the development server:**
```bash
npm run dev

```



---

## 📈 Engineering Highlights

* **Separation of Concerns:** Instead of performing fetch operations inside React lifecycle triggers, all network layers are completely decoupled into an isolated service client module.
* **Object-Fit Optimization:** Avoided image stretching and layout shifts across viewport transitions by establishing custom grid card containers bound to dynamic `object-fit: cover` properties.

```

```
