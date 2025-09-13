COMPANY: CODTECH IT SOLUTIONS

NAME: Aasim Kader

INTERN ID: CT04DY864

DOMAIN: FRONT END DEVELOPMENT

DURATION: 4 WEEEKS

MENTOR: NEELA SANTOSH

Description for E Learning platform :

front-end design for an E-Learning platform using only HTML, CSS, and JavaScript. It is a single-page application (SPA) where different sections like Home, Courses, Course Detail, and Profile are all part of the same file, but JavaScript dynamically switches between them. This makes the website lightweight, responsive, and easy to use without requiring multiple HTML files.

1. Navigation Bar

At the top of the page, there is a navigation bar (<nav>). It contains the platform name “E-Learning” and menu options:

Home

Courses

Course Detail

Profile

These links are not traditional page reloads. Instead, they call a JavaScript function showPage() which displays the selected section and hides the others. This approach gives the feel of a multi-page website while keeping everything inside one file.

2. Home Section

The Home section (<section id="home">) is the welcome page. It uses a hero banner with a title and a welcome message. This section introduces the platform, stating that learners can study at their own pace while tracking progress. It creates a good first impression for visitors and highlights the platform’s purpose.

3. Courses Section

The Courses section (<section id="courses">) displays a grid of courses using CSS Grid. Each course card (.course-card) contains:

A title (e.g., “HTML & CSS Basics”)

A short description

A Start Course button

A progress bar showing how much of the course is completed

The progress bar is updated dynamically with JavaScript. When lessons are completed, the width of the .progress bar increases accordingly. This gives users a clear visual representation of their learning progress.

4. Course Detail Section

The Course Detail section (<section id="course-detail">) contains:

A title

An embedded YouTube video (<iframe>) which acts as the lecture content

A list of lessons with checkboxes

Each lesson has a checkbox, and when a user checks it, the function trackProgress() stores the lesson as completed in localStorage (browser’s local storage). This way, even if the user refreshes or closes the browser, their progress remains saved. This simulates a real progress-tracking system.

5. Profile Section

The Profile section (<section id="profile">) shows the total number of lessons completed. It retrieves stored data from localStorage and displays the user’s progress. This helps learners quickly see their overall learning achievements.

6. Styling with CSS

The CSS is written inside the <style> tag. Key features:
Dark navigation bar for clear visibility
A hero section with a purple background for the home page
Course cards styled with white backgrounds, shadows, and rounded corners
Progress bars styled with grey background and purple filling
Responsive design using grid-template-columns so courses align neatly on all screen sizes
This ensures the platform is visually appealing and easy to use across devices.

7. JavaScript Functionality

The JavaScript (<script> at the bottom) handles the interactivity:
showPage(pageId) → switches between sections
trackProgress(lessonId) → saves completed lessons into localStorage
updateProfile() → updates the profile page with the number of lessons completed

OUTPUT :  



updateCourses() → updates progress bars in the courses section

These functions make the platform interactive and persistent, simulating a basic learning management system (LMS).
