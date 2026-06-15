# Personal Portfolio Website — Mansoor Ali

A high-performance, responsive single-page web application engineered to professionally showcase my experience, technical milestones, and verified credentials as a Web & Systems Developer. 

Built with a modern minimal terminal-inspired interface theme, this codebase features fluid layouts, bespoke client-side animations, image modals, and an automated carousel layout designed completely from scratch using native web technologies—zero heavy component frameworks or bloated third-party dependencies required.
## 🔗 Live Deployment

For a live, interactive preview of the portfolio, visit:
👉 **[mansooraliportfolio.netlify.app](https://mansooraliportfolio.netlify.app)**

## 🚀 Live Preview & Core Highlights

* **Production Identity:** Showcases **2+ years of working experience** delivering custom business solutions, e-commerce applications, and high-performance backend systems.
* **Performance-Optimized UI:** Achieves lightning-fast page speed and smooth asset delivery using modern HTML5, clean CSS custom properties (`:root`), and optimized standard script logic.
* **Responsive Multi-Tier Layouts:** Engineered a unique horizontal scrolling nav-link array mechanism for modern mobile viewports. **Eliminates traditional burger menus entirely**, ensuring instantly accessible user routes across touch and desktop platforms alike.
* **Custom Client Engine Architecture:** Includes an asynchronous client-side content slider, state-driven insight modules, and high-fidelity credential overlays natively managed via vanilla JavaScript optimization vectors.

---

## 🛠️ Core Technology Matrix

| System Domain | Technologies & Infrastructure Used |
| :--- | :--- |
| **Front-End Architecture** | HyperText Markup Language (HTML5), Cascading Style Sheets (CSS3), Semantic Layout Patterns |
| **Bespoke Script Execution** | Asynchronous Native JavaScript (Vanilla ES6+ DOM Engine) |
| **Design Tokens & Fonts** | Google Fonts Integration (`Plus Jakarta Sans`, `JetBrains Mono`), FontAwesome Icon Core |
| **Performance Enhancements** | Native CSS `backdrop-filter` Blurring, Fluid Layout Flexbox/Grid Systems, Clean Structural Lifecycle Hooks |

---

## 📂 Structural Code Highlights

### 1. Zero-Dependency Asynchronous Carousel Engine
Rather than importing heavy layout packages, the verified credentials pipeline leverages an explicit, window-aware translation engine built in native ES6 Javascript. It self-adjusts layout views based on responsive breakpoints dynamically:

```javascript
const updateSliderPosition = () => {
    const cardsPerView = window.innerWidth <= 768 ? 1 : 2;
    const totalNodes = cards.length;

    if (currentIndex > totalNodes - cardsPerView) {
        currentIndex = 0;
    }

    if (cards[currentIndex]) {
        const widthFactor = cards[currentIndex].getBoundingClientRect().width;
        const offset = currentIndex * (widthFactor + 30); // Maintains layout safety gap rules
        track.style.transform = `translateX(-${offset}px)`;
    }
};
