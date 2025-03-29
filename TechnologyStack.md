# 🛡️FAQ Collapsible Section  

## 🌐 Website Elements  
🔹 **FAQ Questions** → List of commonly asked cybersecurity questions.  
🔹 **Toggle Buttons** → Expand or collapse answers dynamically.  
🔹 **Icons (🕽️ ❌)** → Indicate open/close states visually.  
🔹 **Animations** → Smooth transitions when expanding/collapsing FAQs.  

## 🛠️ Technology Stack  

### 🖥️ Frontend Development  
- **HTML** → Defines the FAQ structure.  
- **CSS** → Styles the FAQ section and controls animations.  
- **JavaScript** → Adds interactive functionality.  

## 📆 Key Functionalities  

### **1️⃣ HTML Structure**  
```html
<div class="faq">
  <h3 class="faq-question">What is Cybersecurity?</h3>
  <p class="faq-text">Cybersecurity is the practice of protecting systems, networks, and data from cyber threats.</p>
  <button class="faq-toggle">
    <i class="fas fa-chevron-down"></i>
    <i class="fas fa-times"></i>
  </button>
</div>
```

**💡 Explanation:**  
- The `.faq` `div` represents an individual FAQ item.  
- The `.faq-text` contains the answer and is hidden by default.  
- The `.faq-toggle` button allows expanding/collapsing of the answer.  

---

### **2️⃣ CSS Styling & Animations**  
```css
.faq.active .faq-text {
  display: block;
}
```

**💡 Explanation:**  
- `.faq-text` is normally hidden.  
- When `.faq.active` is applied (via JavaScript), the text is displayed.  

---

### **3️⃣ JavaScript Interactivity**  
```js
document.querySelectorAll(".faq-toggle").forEach(toggle => {
    toggle.addEventListener("click", () => {
        toggle.parentNode.classList.toggle("active");
    });
});
```

**💡 Explanation:**  
- Selects all toggle buttons.  
- Adds a `click` event listener.  
- Toggles the `.active` class on the FAQ item, showing or hiding the answer.  

---

## 🎯 Learning Outcomes  
✅ Understanding **DOM manipulation** using JavaScript.  
✅ Implementing **collapsible UI elements** for better UX.  
✅ Applying **CSS animations and transitions**.  
✅ Managing **dynamic class toggling**.  

## 🔚 Conclusion  
This project is a simple yet effective way to create an interactive FAQ section for cybersecurity topics. It enhances **user engagement** while maintaining a clean and responsive layout.  

🚀 **Want to improve it? Contributions are welcome!**  
