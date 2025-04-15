# 🔍 Pathfinding Visualizer using Flask + JavaScript

A web-based visualizer for popular pathfinding algorithms including **A\***, **AO\***, **Dijkstra**, **BFS**, and **DFS**. The project features a **Flask backend** with Python implementations of the algorithms and a **JavaScript frontend** to display the visualizations in a dynamic grid.

---

## 🚀 Features

- 🌐 Interactive grid for placing start, end, and wall nodes  
- 🔄 Supports the following algorithms:  
  - A* (A-star)  
  - AO* (AND-OR graph search)  
  - Dijkstra’s Algorithm  
  - Breadth-First Search (BFS)  
  - Depth-First Search (DFS)  
- 🧠 Python backend logic using Flask  
- 🖼️ Dynamic frontend with HTML, CSS, and JavaScript  
- 🔁 Multi-path option to find multiple solutions  

---

## 🗂️ Folder Structure

```
pathfinding-visualizer/
│
├── app.py                  # Flask backend server  
├── requirements.txt        # Python dependencies  
│
├── templates/
│   └── index.html          # Main frontend UI  
│
├── static/
│   ├── styles.css          # CSS for grid and UI  
│   └── script.js           # JavaScript logic and API calls  
```

---

## ⚙️ Installation and Usage

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/pathfinding-visualizer.git
cd pathfinding-visualizer
```

### 2. Install Python Dependencies

```bash
pip install -r requirements.txt
```

### 3. Start the Flask Server

```bash
python app.py
```

Flask server will run at: [http://127.0.0.1:5000](http://127.0.0.1:5000)

### 4. Open the App

Visit the URL in your browser:  
[http://127.0.0.1:5000](http://127.0.0.1:5000)

---

## 📡 API Overview

### `POST /find_path`

**Request Body:**

```json
{
  "graph": [[0, 0, 1, 0, ...]],
  "start": [x1, y1],
  "end": [x2, y2],
  "algorithm": "astar",  // Options: "astar", "aostar", "dijkstra", "bfs", "dfs"
  "multiPath": true
}
```

**Response:**

```json
{
  "path": [[x1, y1], [x2, y2], ...],
  "visited": [[a1, b1], [a2, b2], ...]
}
```

---

## 🛠️ Built With

- **Frontend:** HTML, CSS, JavaScript  
- **Backend:** Python, Flask  
- **Algorithms:** A*, AO*, Dijkstra, BFS, DFS  

---

## 🙌 Author

Developed by [Your Name]  
🔗 [Your GitHub](https://github.com/yourusername)

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
