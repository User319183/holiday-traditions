## **Student Design Brief**

Complete this design brief with your partner **before** you begin coding. This document defines your idea, design intent, and technical plan. In professional web projects, this type of brief guides development decisions and keeps the project focused. (*Download and Save this file in your project repository)*

**Project Title**

Working title for your website.

* Snowflake Designer Lab \- Cultural Winter Patterns

### **Design Challenge Summary**

In 2 to 3 sentences, describe the website you plan to create and the experience you want users to have. Focus on the concept, tone, and purpose of the site rather than specific features.

* An interactive web application where users create symmetrical snowflake designs by drawing with automatic symmetry reflection and stamping cultural patterns from 12 global winter traditions. The experience celebrates cultural diversity while providing a creative, meditative design tool with a polished winter aesthetic featuring animated snowfall, aurora effects, and ambient music.

### **Team Roles**

Briefly describe how responsibilities will be shared between partners. (Who is doing what)

* Sathvik Sridar (Lead): Project lead and primary developer. Managed overall project direction, implemented the core drawing canvas with a symmetry system, integrated Vue.js pattern library, handled deployment to GitHub Pages, and coordinated team efforts.  
* Joseph Friedman: Cultural research and content development. Researched the 12 winter traditions to ensure authentic and respectful representation, wrote pattern descriptions and cultural significance text, and assisted with testing across different browsers.  
* Ethan Chang: UI/UX design and quality assurance. Contributed to the visual design, including color schemes and layout decisions, created the winter-themed aesthetic, tested responsive design on mobile devices, and provided feedback on user experience improvements.

### **Design Goals**

List **4 to 6 specific goals** that will guide your design and development decisions.

1. Create an intuitive drawing experience with real-time symmetry reflection (4-fold, 6-fold, 8-fold)  
2. Celebrate cultural diversity by featuring authentic winter tradition patterns from 12 global cultures.  
3. Implement persistent storage to enable users to save and revisit their snowflake gallery.  
4. Design an immersive winter atmosphere with animated snow, aurora effects, and ambient music.  
5. Ensure full accessibility through keyboard navigation and reduced-motion support.  
6. Build a responsive experience that works seamlessly on desktop and mobile devices.

### **Content and Data Plan**

Describe the type of content your site will display and how it will be structured.

Include:

* What information will be stored in JSON  
* What fields each data item will include

*Example: Each item includes name, description, category, date or season, image, and tags.*

What information is stored in JSON: Cultural pattern data for 12 winter traditions

Each data item includes:

* id \- Unique identifier  
* name \- Pattern name (e.g., "Rangoli Circle")  
* culture \- Culture of origin (e.g., "Indian")  
* holiday \- Associated celebration (e.g., "Diwali")  
* description \- Cultural significance and meaning  
* category \- Pattern type (geometric, floral, symbolic)  
* svgPath \- Vector path data for rendering  
* colors \- Traditional color palette

### **Vue Interactivity Plan**

List at least **two interactive features** you plan to build using Vue and explain how they will improve the user experience. *Examples: ( Search, filter, sort, toggles, favorites, saved items)*

1. Pattern Search & Filter: Users can search patterns by name, culture, or holiday, and filter by category. This helps users quickly find patterns relevant to their heritage or interests, making the library of 12 traditions easy to navigate.  
2. Interactive Pattern Cards: Hovering reveals cultural information with smooth animations. Clicking a pattern stamps it onto the canvas. This creates an educational experience where users learn about traditions while designing.

### **New Concept Exploration**

Identify **one new concept** you will explore in this project and explain how it will be integrated into your site.

* LocalStorage API for Data Persistence  
* The site uses the browser's LocalStorage API to save user data locally without requiring a backend database. This includes:  
* Saved snowflake designs with thumbnails and metadata  
* User preferences (dark/light mode, audio settings)  
* Gallery management (save, rename, delete designs)  
* This was integrated by creating a storage utility module that handles serialization/deserialization of canvas data to base64 images, with functions for CRUD operations on the gallery.

### **AI Integration Plan**

Describe **3 specific ways** AI will support your work on this project.

For each, include:

* What you will ask AI to help with  
* How you will review, edit, and adapt the results

AI should support your thinking, not replace it.

Canvas Symmetry Algorithm

1. What I asked: Help implement real-time symmetry reflection for drawing on HTML5 Canvas with configurable fold counts  
2. How I reviewed: Tested each symmetry mode (4/6/8-fold) manually, adjusted rotation calculations, and refined the line smoothing algorithm for better visual results.

CSS Animations & Visual Effects

3. What I asked: Creating performant snowfall animation, aurora borealis effects, and glassmorphism UI styling  
4. How I reviewed: Tested animations across browsers, adjusted timing/opacity for subtlety, ensured reduced-motion support was working, and tuned colors for both light and dark modes.

Responsive Design Implementation

5. What I asked: Implementing fluid typography and spacing using CSS clamp() functions for smooth scaling  
6. How I reviewed: Tested on multiple viewport sizes, adjusted breakpoints and clamp values, fixed overflow issues, and ensured touch targets remained accessible on mobile

### **Success Criteria**

List **3 indicators** that will help you evaluate whether your project was successful.

1. Functional Drawing System: Users can successfully create, save, and export snowflake designs with working symmetry modes and pattern stamps  
2. Cultural Authenticity: All 12 cultural patterns are accurately represented with respectful, researched descriptions that educate users about winter traditions  
3. Technical Requirements Met: Site includes Vue.js integration, JSON data storage, LocalStorage persistence, responsive design, and accessibility features as specified in the rubric
