# Assignment & Exam Tracker Widget

### Issue  
Students manage various deadlines on multiple platforms (Canvas, Blackboard, Google Classroom, etc.), leading to stress and increasing the likelihood of overlooking crucial assignments or tests. Lacking a specific, organized space to monitor everything heightens stress and diminishes efficiency.  

### Answer  
This widget provides learners with an easy, unified perspective on forthcoming tasks and tests. Students can swiftly add tasks, view deadlines in an organized list, and monitor urgency with color-coding (e.g., red = approaching deadline, green = on the horizon).  

### Impact  
By combining deadlines into a single user-friendly display, the widget aids students in organizing their time, preventing last-minute studying, and keeping track of their assignments. Rather than being bogged down, they can concentrate more on acquiring knowledge.  

---

## Demo  
- **Live:** [Vercel Deployment Link](https://alfred-interview.vercel.app/)  
- **Repo:** [GitHub Repository](https://github.com/NoahDereje/alfredInterview)  

---

## Features  
- **Add tasks** with title, optional course, type (assignment/exam), and due date/time  
- **Color-coded urgency**  
  - Red = due within 24h  
  - Orange = due within 3 days  
  - Green = more than 3 days away  
  - Overdue = red text  
  - Done = gray + strikethrough  
- **Mark as done/undone** with a checkbox  
- **Delete tasks** individually  
- **Search and filter** by title, course, or type (assignment/exam)  
- **Automatic sorting** by soonest due date  
- **LocalStorage persistence** (tasks remain after refresh)  
- **Seed button** to quickly add example tasks for demo  
- **Clear Done button** to remove completed tasks in bulk  
- **Reset All button** to clear all tasks  
- **Mobile-friendly responsive layout**  
- **Accessible design** with aria-labels and keyboard (Enter key) support  

---

## Future Improvements  
- Calendar view to visualize deadlines by day/week  
- Reminders/notifications for upcoming deadlines  
- Recurring tasks for repeating assignments/quizzes  
- API integration with Canvas, Blackboard, Google Classroom  
- Export/import support (e.g., `.ics` calendar files)  
- Collaboration features for group projects or shared lists  
- User accounts for cloud sync across devices  
- Design polish: theming, dark/light mode, customizable urgency thresholds  

---

## How to Run Locally  
1. Clone this repo.  
2. Open `index.html` in any modern browser.  
   - No build tools required.  
   - Works offline thanks to LocalStorage.  

---

## Architecture & Decisions  
- Single-file implementation (HTML, CSS, JS) for clarity and speed.  
- LocalStorage used instead of a backend for simplicity.  
- Items sorted automatically by due date for production intuition.  
- Color-coded urgency thresholds chosen for clarity:  
  - ≤24h (red), ≤3d (orange), >3d (green).  
- Reset/Seed buttons included to make demoing simple.  

---

## Trade-offs  
- No real API integration (like canvas, google classroom, etc) due to time constraints.  
- No authentication or cross-device sync.  
- Calendar visualization omitted for simplicity.  

---

## Top 3 Strengths  
1. **Backend Architecture**
2. **API Integration**
3. **Problem Solving / Debugging**  
