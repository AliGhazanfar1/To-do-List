# 📝 To-Do List

A simple and responsive **To-Do List web application** built using **HTML, CSS, and JavaScript**.
The application allows users to add tasks, mark tasks as completed, delete tasks, and automatically save tasks using **Local Storage**.

## 🚀 Features

* ➕ Add new tasks
* ✅ Mark tasks as completed
* ❌ Delete tasks
* 💾 Tasks are saved using Local Storage
* 🔄 Tasks remain available after refreshing the page
* 📱 Responsive and clean user interface
* 🎨 Gradient background with a simple modern design

## 🛠️ Technologies Used

* **HTML5** – Structure of the application
* **CSS3** – Styling and responsive layout
* **JavaScript** – Application logic and DOM manipulation
* **Local Storage** – Saving tasks in the browser

## 📂 Project Structure

```text
To-Do-List/
│
├── images/
│   ├── checked.png
│   ├── unchecked.png
│   └── icon.png
│
├── index.html
├── style.css
└── script.js
```

## ⚙️ How It Works

### 1. Add a Task

Enter a task in the input field and click the **Add** button.

JavaScript creates a new `<li>` element and adds it to the task list.

### 2. Complete a Task

Click on a task to mark it as completed.

The `checked` CSS class is added or removed using:

```javascript
e.target.classList.toggle("checked");
```

This changes the task appearance and displays the checked icon.

### 3. Delete a Task

Click the **×** button next to a task to remove it.

```javascript
e.target.parentElement.remove();
```

### 4. Save Tasks

The application stores the current task list in the browser's Local Storage:

```javascript
localStorage.setItem("data", listContainer.innerHTML);
```

When the page loads, the saved tasks are retrieved:

```javascript
listContainer.innerHTML = localStorage.getItem("data");
```

This allows tasks to remain even after refreshing the page.

## 💡 Key JavaScript Concepts Used

* DOM Manipulation
* `createElement()`
* `appendChild()`
* `classList.toggle()`
* Event Listeners
* Event Delegation
* `localStorage`
* `setItem()` and `getItem()`
* `innerHTML`

## ▶️ How to Run

1. Clone the repository:

```bash
git clone https://github.com/your-username/To-Do-List.git
```

2. Open the project folder.

3. Open `index.html` in your browser.

No additional installation or dependencies are required.

## 📸 Project Preview

Add a screenshot of your To-Do List here:

```text
![To-Do List Preview](images/preview.png)
```

## 🔮 Future Improvements

* Add task editing functionality
* Add task categories
* Add due dates and reminders
* Add dark mode
* Add task filtering
* Add animations
* Improve mobile responsiveness

## 👨‍💻 Author

**Ali Ghazanfar**

Built as a frontend JavaScript project to practice **DOM manipulation, event handling, and browser Local Storage**.
