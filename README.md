# 🧑‍💻 PLP Hackathon Portfolio – July 2025

A collaborative, fully responsive, framework-free developer portfolio crafted by **Faraj Salim** and **Katy Safari** for the **Power Learn Project Hackathon – July 2025**.

## 🎨 Theme & Design

- **Color Palette:** Catppuccin Mocha
- **Visual Style:** Clean, soft shadows, rounded corners, card-style layout
- **Dark Mode:** Default and only mode
- **Typography:** System fonts for simplicity and speed
- **Layout:** Desktop-first, fully responsive via CSS media queries

---

## 📚 Sections

### 1. 👥 Meet the Team

Each team member is presented using a clean profile **card layout**:

- **Avatar**
- **Role**
- **Bio**
- **Interests**
- **Technology Badges:** Styled using [Shields.io](https://shields.io)

Cards are styled with:
- Flexbox layout
- Custom CSS classes per member (e.g. `.katy`, `.faraj`)
- Consistent padding and spacing
- Section heading: `Meet the Team`

---

### 2. 🎓 Education Timeline

The **Education** section uses **horizontal timelines**, with one timeline per person:

- Each timeline contains:
  - A connecting colored line (`.line`)
  - Timeline dots for each educational event (`.dot`)
  - Labels with:
    - Degree
    - Institution
    - Duration
- Fully responsive using percentage-based positioning
- Timeline per person:
  - **Faraj (green)**: 
    - BSc. Computer Science @ Mount Kenya University (Jan 2024 – Present)
    - Software Engineering @ PLP Africa (July 2025 – Present)
  - **Katy (mauve)**:
    - BSc. Computer Science @ Pwani University (Sep 2023 – Present)
    - Software Engineering @ PLP Africa (July 2025 – Present)

No JavaScript was used; positioning and alignment are handled purely using CSS `position: absolute` inside a relatively positioned container.

---

### 3. 📬 Contact Section

The contact section contains:

- **FAQ Accordion**
  - Pure HTML/CSS accordion using `<details>` and `<summary>` tags
  - Example questions: “How can I reach you?”, “Are you open to freelance?”
  - Each collapses and expands with no JS

- **Contact Form**
  - Submits using [Formspree](https://formspree.io/)
  - Fields:
    - Name (required)
    - Email (required)
    - Message (required)
  - `POST` method form submission to Formspree endpoint
  - Upon success, Formspree handles confirmation (no custom JS needed)

#### Example HTML:

```html
<form action="https://formspree.io/f/yourFormID" method="POST">
  <input type="text" name="name" placeholder="Your Name" required />
  <input type="email" name="email" placeholder="Your Email" required />
  <textarea name="message" placeholder="Your Message" required></textarea>
  <button type="submit">Send</button>
</form>
