# Prim's Algorithm Simulation

This is a web-based visual simulator for **Prim's Algorithm**, a greedy algorithm used to find the **Minimum Spanning Tree (MST)** of a connected, undirected, and weighted graph.

The simulation allows users to:
- Create custom graphs by placing nodes and adding edges
- Visualize the step-by-step execution of Prim's algorithm
- Understand how MSTs are formed through interactive visuals

---

## 🌐 Live Demo

https://drive.google.com/file/d/1ju4f_phZZ2z70uw_2lbIxyhU6lQAsC8c/view?usp=drive_link 

---

## 🛠️ Features

- Node placement via canvas click
- Custom edge creation with weight input
- Interactive algorithm step-by-step execution
- Visual edge coloring to indicate algorithm decisions:
  - 🟢 Green: Accepted MST edges
  - 🟠 Orange: Currently considered edges
  - 🔴 Red: Rejected edges
  - ⚪ Gray: Unused edges

---

## 📷 Screenshot

![image](https://github.com/user-attachments/assets/dde1decf-290c-45c6-84c7-a5d6db62d5e8)
![image](https://github.com/user-attachments/assets/4b14c54f-e611-4144-9480-ce8bd2b973d2)
![image](https://github.com/user-attachments/assets/6fd7ff58-c324-4e2c-9b4b-449900d301c2)
![image](https://github.com/user-attachments/assets/4aa0b53e-1da4-4163-94ab-33f23d16106b)
![image](https://github.com/user-attachments/assets/9ef5c72f-4f81-442d-b53e-e79bce796f7d)

---

## ❓ How to Use

1. **Setup Phase**
   - Enter the number of nodes (2–20) and click **Setup Graph**

2. **Node Placement**
   - Click on the canvas to place nodes (same number as specified)

3. **Edge Creation**
   - Click on two nodes (they turn red when selected)
   - Enter a weight and click **Add Edge**
   - Repeat for as many edges as needed

4. **Run the Algorithm**
   - Click **Run Prim's Algorithm**
   - Click **Next Step** to progress through each step

5. **Reset**
   - Use **Reset** to start over at any time

---

## 📘 Algorithm Explanation

**Prim's Algorithm** works by:

1. Starting with a single arbitrary node
2. Repeatedly adding the **minimum-weight edge** that connects a visited node to an unvisited node
3. Continuing until all nodes are included in the spanning tree

### Steps in this simulator:

- Initialize a **priority queue (min-heap)** with all edges connected to the starting node
- Select the smallest edge that connects to an unvisited node
- Add the edge to the MST and mark the node as visited
- Add all new edges from the newly added node to the queue
- Repeat until all nodes are visited or the priority queue is empty

---

## 🕔 Time and Space Complexity

### Time Complexity

- Using a min-heap (priority queue) and an adjacency list:
- `V` = Number of vertices (nodes)
- `E` = Number of edges
- Each insertion and deletion in the heap takes `log V` time

### Space Complexity

- Adjacency list: `O(V + E)`
- Other arrays (visited, keys, parent): `O(V)`
- Priority queue (min-heap): up to `O(V)`

**Overall Space:** `O(V + E)`

---

## 📁 Files

- `index.html` – Main simulation file containing HTML, CSS, and JavaScript
- Uses HTML5 Canvas for drawing
- Fully contained (no external libraries)

---

## 🧑‍💻 Author

Developed by **[Vedansh Pandey]**, **[Vedant Kolhe]**, and **[Vedant Desai]**
For educational and demonstration purposes.

---

## 📄 License

This project is open-source and free to use under the MIT License.
