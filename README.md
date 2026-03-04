# SBA-9: React Dashboard Application
**Author:** Jameka Haggins 

In this assessment, you will apply the skills you have developed throughout your React training to build a functional, real-world dashboard application. This project will test your understanding of React components, state management, TypeScript integration, form handling, and component composition.
---
## Reflection

Using TypeScript to create a "safety net" for the data, I defind a Task interface in types/index.ts, I ensured that every task had a title, priority, and status. This prevented  bugs where I might accidentally call a property the wrong name (something I have done a lot of in the past). Focusing on Component Composition, instead of one giant file, I broke the app into small pieces like TaskItem and TaskForm. This made the code easier to read and manage. I used useState to keep track of the list of tasks and useEffect to save everything to localStorage so the user doesn't lose their data when they refresh the page.

Managing the Filter state across different components was tricky. I needed the TaskList to know what the TaskFilter was doing.
The solutuion? I lifted the state up to the Dashboard component. By keeping the "filter" and "search" values in the parent, I could easily tell the list exactly which tasks to show. Another challenge was Health hurdles. Dealing with an ear infection while coding made it difficult to focus on complex logic.I broke the development into very small, 20-minute sessions and used clear TypeScript interfaces to help me remember where I left off without getting overwhelmed.

Finally State Management, The 'Brain' (Dashboard) holds all the info, and the 'Hands' (Form/List) just do what the brain tells them to do. Using the good ol' KISS Method.
