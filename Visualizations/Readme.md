# 🔍 CHAOSS Augur Microtasks – D3.js Visualizations

Welcome to a collection of sleek, interactive **D3.js visualizations** crafted for [CHAOSS Augur](https://chaoss.community/augur) as part of my **Google Summer of Code (GSoC)** microtasks.

These visualizations are designed to offer clear, insightful, and aesthetically pleasing representations of project health, contributor behavior, and community dynamics — empowering open-source maintainers and contributors to make data-driven decisions with confidence.

---

## 🌟 Visualizations

### 1. 👨‍💻 Contributor Activity Line Chart  
**Type:** Time Series Line Chart  
**Purpose:** Track contributor commit frequency over time  
**Tech Stack:** `d3.js (v7)`

#### 📊 Features:
- Clean, responsive line chart displaying daily commit activity  
- Gradient stroke for a modern and vibrant look  
- Tooltip on hover with date and number of commits  
- Scalable to include multiple contributors or longer date ranges

#### 🧠 Use in CHAOSS Augur:
- Monitor individual or team contribution trends  
- Identify periods of high or low development activity  
- Detect burnout patterns or peak collaboration periods

  ![Screenshot 2025-04-05 113536](https://github.com/user-attachments/assets/88f8b5d6-96b1-4187-8471-cc9e7c8e3496)

---

### 2. 🧭 Force-Directed Contributor Network Graph  
**Type:** Dynamic Force-Directed Graph  
**Purpose:** Visualize relationships between contributors (e.g., co-authorship, PR interactions, shared files/modules)  
**Tech Stack:** `d3.forceSimulation`, `d3.drag`, `d3.forceLink`, `d3.forceManyBody` 

#### 🔧 Features:
- Nodes represent contributors  
- Edges (links) show collaborative relationships  
- Fully interactive: drag & reposition nodes  
- Smooth physics-based layout simulation

#### 🔍 Use in CHAOSS Augur:
- Reveal key contributor collaboration patterns  
- Identify tightly-knit subgroups or isolated contributors  
- Scale to large networks easily with optimized force layout

  ![Screenshot 2025-04-05 113559](https://github.com/user-attachments/assets/7b71b0d5-049a-48ff-8635-e7bcc0d7a6e4)

---

### 3. 🗂️ Issue Resolution Timeline  
**Type:** Horizontal Bar Chart (Gantt-style)  
**Purpose:** Visualize how long issues stayed open before being resolved  
**Tech Stack:** `d3.scaleTime`, `d3.scaleBand`, `d3.axisBottom` 

#### 🔧 Features:
- Each bar represents an issue’s open-to-close lifespan  
- Time-based x-axis for clear tracking  
- Helps analyze team responsiveness and backlog velocity

#### 🔍 Use in CHAOSS Augur:
- Understand average and outlier issue resolution times  
- Compare contributors or time periods for efficiency  
- Visualize project health by spotting unresolved issues

![Screenshot 2025-04-05 113632](https://github.com/user-attachments/assets/a7e0fbfd-b3e0-43e8-8413-8fc88ea61dc3)

---

### 4. 📆 Community Activity (Calendar Heatmap)  
**Type:** Calendar Heatmap  
**Purpose:** Visualize daily overall project activity (commits, PRs, issues, etc.) over a year  
**Tech Stack:** `d3.js`, `d3.timeFormat`, `d3.scaleSequential`

#### 🔧 Features:
- Displays daily activity levels using color intensity  
- Monthly grid layout like GitHub’s contribution graph  
- Intuitive overview of community engagement over time

#### 🔍 Use in CHAOSS Augur:
- Identify seasonal trends or contribution bursts  
- Spot silent periods or contributor burnout  
- Track engagement during events like hackathons or releases

![Screenshot 2025-04-05 113651](https://github.com/user-attachments/assets/83c8cf42-d82f-4694-9cf3-1b55aa41f3d6)

---

### 5. 🕸️ Project Radar (Radar Chart)  
**Type:** Radar Chart  
**Purpose:** Visualizes multidimensional metrics like activity, responsiveness, growth, etc.  
**Tech Stack:** `d3.lineRadial`, `d3.select`, `Math.cos/sin` for axis calculations 

#### 🔧 Features:
- Draws a polygon connecting values across multiple axes (dimensions)  
- Radial axis labels for each KPI  
- Smooth `lineRadial` path with color-filled shape  
- Easily customizable for more or fewer dimensions

#### 🧠 Use in CHAOSS Augur:
- Compare multiple repositories based on key performance indicators  
- Provide a snapshot of a project’s health across categories  
- Visualize team or community performance profiles

![Screenshot 2025-04-05 113710](https://github.com/user-attachments/assets/b008a3df-e7be-4a9d-94e8-69324c1abd32)

---

### 6. 🌍 Contributor Globe (3D Globe Visualization)  
**Type:** 3D Globe  
**Purpose:** Show geographical distribution of contributors or project activity  
**Tech Stack:** `globe.gl`, `Three.js`, `WebGL`

#### 🔧 Features:
- Interactive 3D Earth with auto-rotation  
- Highlights contributor locations using color-coded points  
- Zoom, pan, and tooltip interactivity  
- Support for custom tagging (e.g., city names or contributor handles)

#### 🌐 Demo Points:
- San Francisco (🟦 Cyan)  
- Berlin (🟧 Orange)  
- Delhi (🟩 Lime)

#### 🧠 Use in CHAOSS Augur:
- Showcase global contributor engagement  
- Display real-time activity origins  
- Great for community or marketing presentations

![Screenshot 2025-04-05 113743](https://github.com/user-attachments/assets/ba0e1e11-7df9-438e-b23d-e38f1ba748a4)

---

### 7. 📜 Changelog Stream (Timeline Visualization)  
**Type:** Horizontal Timeline  
**Purpose:** Visualizes project events like commits, pull requests, and issue updates  
**Tech Stack:** `d3.js (v7)` 

#### 🔧 Features:
- Clean horizontal timeline layout  
- Color-coded markers for event types:  
  - 🟦 Commit → Cyan  
  - 🟧 PR → Orange  
  - 🟩 Issue → Lime  
- Tooltips reveal event messages/details  
- Dark theme with smooth animations

#### 🧠 Use in CHAOSS Augur:
- Understand repository activity trends over time  
- Identify development bursts and idle periods  
- Combine with contributor data for richer insights

![Screenshot 2025-04-05 113803](https://github.com/user-attachments/assets/22a34ddb-28d3-4d82-a806-f1255050b089)

---

### 8. ⚡ Review Velocity Gauge  
**Type:** Gauge Chart  
**Purpose:** Visualize the speed of code reviews and PR handling  
**Tech Stack:** `d3.arc`, `d3.transition`, `d3.interpolate` 

#### 🔧 Features:
- Circular gauge with a pointer to show review velocity  
- Color gradients from red → yellow → green  
- Animates smoothly with dynamic values  
- Configurable min/max and labels

#### 🧠 Use in CHAOSS Augur:
- Monitor how quickly code is reviewed  
- Track team responsiveness and process bottlenecks  
- Compare review velocity across time or teams

  ![Screenshot 2025-04-05 113820](https://github.com/user-attachments/assets/2425e530-65d3-45da-943b-9ea31efe15be)
