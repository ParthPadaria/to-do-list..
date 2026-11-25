# ✅ To-Do List

A clean, responsive to-do list built with plain HTML, CSS, and JavaScript. Add, complete, and delete tasks, filter them by status, and keep your list saved in the browser between visits.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

## ✨ Features

- Add tasks with the **Add** button or the **Enter** key
- Mark tasks as complete with a checkbox
- Delete individual tasks
- Filter by **All**, **Active**, or **Completed**
- Live counter showing how many tasks are left
- **Clear completed** button to remove finished tasks in one click
- Tasks are saved in `localStorage`, so they persist after a refresh
- Safe rendering with `textContent`, so typed HTML is never executed
- Responsive dark-themed layout
- No libraries or dependencies

## 📸 Preview

> Add a screenshot or GIF of your app here.
>
> `![To-Do List Preview](screenshot.png)`

## 🚀 Getting Started

### Option 1: Run locally

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/todo-list.git
   ```
2. Go into the project folder:
   ```bash
   cd todo-list
   ```
3. Open `index.html` in your browser.

### Option 2: Use GitHub Pages

1. Go to **Settings → Pages** in your repository.
2. Under **Source**, select the `main` branch and the `/ (root)` folder.
3. Save, and your app will be live at `https://your-username.github.io/todo-list/`.

## 📁 Project Structure

```
todo-list/
├── index.html    # Markup, styles, and script
└── README.md
```

## 🧠 How It Works

The app keeps a single source of truth: the `tasks` array. Every action follows the same pattern:

**change the data → save → re-render**

| Function | What it does |
|----------|--------------|
| `load()` | Reads saved tasks from `localStorage` |
| `save()` | Writes the `tasks` array to `localStorage` |
| `addTask()` | Adds a new task to the top of the list |
| `toggleTask(id)` | Flips a task between done and not done |
| `deleteTask(id)` | Removes a task by its `id` |
| `render()` | Rebuilds the list on screen based on the active filter |

Each task is stored as an object:

```js
{ id: 1700000000000, text: "Buy groceries", done: false }
```

## 🎨 Customization

**Change the theme colors** by editing these values in the CSS:

```css
background: #0f172a;   /* page background */
background: #1e293b;   /* card background */
background: #38bdf8;   /* accent color (buttons, active filter) */
```

## 👤 Author

**Parth**
