# Profile Card Component (Stage 1B - Frontend Wizards)

A responsive, accessible Profile Card built with **semantic HTML, modern CSS, and vanilla JavaScript**.  
This project was completed as part of the Stage 1B Frontend Wizards task.

---

## Live Demo

🔗 Live URL: [https://joshua-profilecard.netlify.app/]

---

## Features

- Semantic HTML structure (`article`, `header`, `section`, `nav`, `figure`)
- Fully responsive design (mobile → desktop)
- Accessible markup (WCAG AA compliant contrast, aria-live support)
- Dynamic epoch time display (milliseconds)
- Social links open in new tab securely
- Keyboard navigable UI
- Testable with required `data-testid` attributes

---

## Tech Stack

- HTML5
- CSS3 (Flexbox + Media Queries)
- Vanilla JavaScript (no frameworks)

---

## Project Structure

```
profile-card/
│── index.html
│── style.css 
│── script.js 
│── picture.jpg
│── README.md
```

---

## Core Components

| Element | data-testid |
|--------|-------------|
| Profile Card | test-profile-card |
| Name | test-user-name |
| Bio | test-user-bio |
| Avatar | test-user-avatar |
| Time (epoch ms) | test-user-time |
| Social Links | test-user-social-links |
| Hobbies | test-user-hobbies |
| Dislikes | test-user-dislikes |

---

## How to Run Locally

### 1. Clone the repository
```bash
git clone https://github.com/your-username/profile-card.git

```

### 2. Navigate into the folder
```bash
cd profile-card

```

### 3. Open in VS Code
```bash
code .

```

### 4. Run the project

You can use any of the following:

#### Option A: Live Server (Recommended)
- Install **Live Server** extension in VS Code  
- Right-click `index.html`  
- Click **"Open with Live Server"**

#### Option B: Direct Browser
- Double-click `index.html`  
- It will open directly in your browser  

---

## Manual Test Checklist

### Structure
- Profile card renders correctly  
- All required `data-testid` attributes exist  

### Accessibility
- Avatar has meaningful `alt` text  
- Links are keyboard accessible (Tab navigation works)  
- Focus state visible on links  
- Color contrast is readable (WCAG AA)  

### Functionality
- Epoch time updates in milliseconds  
- Social links open in new tab  
- Layout is responsive (mobile/tablet/desktop)  

### Responsiveness
- Mobile: stacked layout  
- Desktop: side-by-side layout  
- No overflow or broken layout on resize  

---

## Time Feature

The time is generated using:

```js
Date.now()

```
It updates every 1 second using:

```js
setInterval(updateTime, 1000);

```
---

## Security Best Practices
- External links use:
```html
target="_blank" rel="noopener noreferrer"

```
---

## Accessibility Notes
- Semantic HTML used throughout
- `aria-live="polite"` applied to time element
- Meaningful alt text for avatar image
- Keyboard navigable interactive elements

---

## Notes
- Avatar supports both local and remote image sources
- Design is mobile-first and scales to desktop
- Component is structured for easy extension (React migration-ready)

---

## Author

Mbamara Joshua — Jay Tech  
Frontend Developer | HNG Internship Stage 1b Submission

