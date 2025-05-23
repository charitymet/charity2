# Academic Project Report Generator Prompt

Generate a comprehensive academic project report following the exact format and structure of a professional MCA mini project submission. Use the following information to personalize the document:

## Required Information to Collect:

### Student & Academic Details:
- **Student Name**: [Full Name]
- **Roll Number**: [Roll No.]
- **Semester**: [e.g., MCA Semester II]
- **Academic Year**: [e.g., 2024-2025]
- **Batch**: [e.g., 2024-2026]
- **Course**: [e.g., Masters of Computer Applications]
- **Institution Name**: [e.g., Institute of Computer Science]
- **University**: [e.g., University of Mumbai]
- **Course Code**: [e.g., MCAP21 MINI PROJECT 1B]

### Project Details:
- **Project Title**: [Complete project name]
- **Project Type**: [e.g., Web Application, Mobile App, Desktop Application, Algorithm Implementation, Data Analysis Tool, Game, etc.]
- **Live Application URL**: [If deployed - e.g., https://your-app.netlify.app, https://your-app.vercel.app, or "Not deployed/Local only"]
- **Technology Stack**: [List all technologies used - Frontend, Backend, Database (if applicable)]
- **Programming Languages**: [e.g., JavaScript, Python, Java, C++, etc.]
- **Frameworks/Libraries**: [e.g., React, Node.js, Express, Django, Flask, etc.]
- **Database**: [e.g., MongoDB, MySQL, PostgreSQL, File-based storage, or "Not Applicable - No database required"]
- **Data Storage Method**: [If no database: File system, Local storage, In-memory, Configuration files, etc.]
- **Deployment Platform**: [e.g., Netlify, Vercel, Heroku, GitHub Pages, or "Not deployed"]

### Faculty Information:
- **Project Guide Name**: [Prof./Dr. Name]
- **Principal Name**: [Dr./Prof. Name]
- **Institution Code/Name**: [Institution abbreviation]

### Project Scope & Features:
- **Target Audience**: [Who will use this application]
- **Main Functionality**: [List 5-7 key features]
- **Project Scope**: [What the project covers]
- **Core Modules**: [Main components/modules of the project]

### Technical Implementation:
- **Architecture**: [e.g., MERN Stack, 3-tier architecture]
- **Authentication Method**: [e.g., JWT, Session-based]
- **Security Features**: [e.g., Password encryption, Input validation]
- **Database Schema**: [Number and types of main entities OR "Not Applicable - No database used"]
- **Data Structure**: [If no database: How data is organized - file formats, data structures, configuration methods]

### Project Limitations:
- **Current Limitations**: [List 4-6 limitations]
- **Scope Constraints**: [What the project doesn't cover]

### Future Enhancements:
- **Planned Improvements**: [List 4-5 future features]
- **Scalability Plans**: [How it can be expanded]

## Document Structure to Generate:

### Title Page:
- Project Report on [Project Title]
- [Course Name] Mini Project
- [Semester]
- Submitted By: [Student Name]
- Roll No: [Roll Number]
- [Institution Name]
- [University Name]

### Acknowledgements Page:
Thank the Principal, Project Guide, and institution for their support and guidance.

### Certificate Pages (2-3 pages):
- Examination certificate template
- Approval certificate from Principal and Project Guide
- External examiner approval certificate

### Table of Contents:
1. Scope of Project
2. Project Description & Limitations
3. UML Diagrams
4. Database/Data Management (Skip if no database - replace with "System Architecture" or "Data Structures")
5. Screen Shots
6. Conclusion
7. Bibliography

### Chapter 1: Scope of Project
- Project overview and objectives
- Target audience description
- Detailed scope including main features
- Platform compatibility (desktop, mobile, etc.)

### Chapter 2: Project Description & Limitations
- Comprehensive project description
- Key functionalities explanation
- Technology stack breakdown (Frontend & Backend)
- Project limitations (6-8 limitations)
- Constraints and scope boundaries

### Chapter 3: UML Diagrams
- Use Case Diagram with description
- Class Diagram with relationships
- Sequence Diagram for key processes
- Brief explanation of each diagram's purpose and relevance

### Chapter 4: Database/Data Management
**For Database-based Projects:**
- Database choice justification
- Complete database schema (3-4 main entities minimum)
- Detailed field descriptions for each schema
- Entity relationships explanation

**For Non-Database Projects:**
- Data management approach explanation (e.g., "No database required - all data handled in-memory using React state")
- File structure or data organization method
- Configuration management (if applicable)
- Data flow and processing methods
- Input/Output data formats
- Memory management or data caching strategies
- Local storage methods (browser storage, file system, etc.)
- **Alternative data handling**: Session storage, local variables, component state management

### Screenshots Requirements:
- **8-10 application screenshots minimum** with descriptions:
  - Main/Home page or Landing page
  - Primary user interface screens
  - Key functionality demonstrations
  - Form/input screens
  - Preview/output screens
  - Admin/Management screens (if applicable)
  - User interaction flows
  - **Results/Generated output** (e.g., invoices, reports, calculations)
  - **Export/Download functionality** (if applicable)
  - Contact or About pages (if applicable)

### Screenshot Generation Options:
**Option 1: Manual Screenshots**
- Provide your own screenshots with descriptions
- Upload images and specify which screen each represents

**Option 2: Automated Screenshot Generation** (RECOMMENDED)
- If you provided a live URL above, request the AI agent to automatically capture screenshots
- The AI will visit your live application and take screenshots of:
  - Homepage/Landing page
  - Main application interface
  - Key functionality screens
  - User interaction flows
  - Different sections/pages of your app
- Include specific instructions for what to capture: [e.g., "Take screenshots of the invoice form, preview modal, and generated PDF"]

**Option 3: Hybrid Approach**
- Combine automated screenshots with specific manual screenshots for complex features

### Chapter 6: Conclusion
- Project overview summary
- Key achievements
- Technical implementation highlights
- Learning outcomes
- Limitations acknowledgment
- Future enhancement possibilities
- Final remarks on project value

### Chapter 7: Bibliography
- Relevant documentation links
- Tutorial/learning resources used
- Framework and library documentation
- Online resources and references

## Formatting Requirements:

- **Page Numbers**: Include page numbers on each page
- **Headers**: "Mini Project Report [Institution], [Course]" on each page
- **Professional Layout**: Clean, academic formatting
- **Consistent Styling**: Uniform fonts, spacing, and structure
- **Proper Citations**: Include all reference sources
- **Academic Tone**: Professional, technical writing style

## Project Type Examples:

### Database-Required Projects:
- E-commerce applications
- Content management systems
- User management systems
- Inventory management
- Social media platforms
- Booking systems

### Non-Database Projects:
- Algorithm implementations (sorting, searching, ML algorithms)
- Mathematical calculators or solvers
- Game applications (simple games, puzzles)
- Data visualization tools (using static datasets)
- Image/audio processing applications
- Desktop utilities or tools
- Static website generators
- Command-line tools
- Educational simulations
- **Invoice generators**
- **PDF generators**
- **Report generators**
- **Frontend-only web applications**
- **File processing tools**

## Document Formatting Examples:

### Title Formatting:
- Main project title should be in ***bold and italics*** 
- Student name in ***bold and italics***
- Section headings should be ***underlined and in bold italics***
- Use consistent formatting throughout the document

### Content Structure:
- Include bullet points and numbered lists where appropriate
- Use tables for structured data (like database schemas)
- Include proper spacing and professional layout
- Add page numbers and consistent headers

## Live Application Integration:

### If you have a deployed application:
1. **Provide the live URL** in the project details section above
2. **Request automated screenshot generation** using this prompt addition:

---
**AUTOMATED SCREENSHOT REQUEST:**
"Please visit my live application at [YOUR_URL] and capture screenshots for the project report. I need you to:

1. Take a screenshot of the homepage/main page
2. Navigate through the application and capture key functional screens
3. Screenshot any forms, input pages, or user interaction areas
4. Capture results/output pages (e.g., generated reports, invoices, calculations)
5. Take screenshots of any admin/management interfaces
6. Include any special features or unique functionality screens

For each screenshot, provide a professional description explaining what the screen shows and its purpose in the application.

Please organize these screenshots in Chapter 5 of the project report with appropriate captions and descriptions."
---

### Benefits of Live URL Integration:
- **Automated screenshot generation** saves time and effort
- **Consistent quality** across all screenshots
- **Complete application coverage** with systematic capture
- **Professional presentation** with proper descriptions
- **Real-time functionality demonstration**
- **Up-to-date interface** showing current application state

## Additional Instructions:

1. **For Database Projects**: Include detailed database schemas, entity relationships, and data management strategies
2. **For Non-Database Projects**: Focus on system architecture, data structures, algorithms, and processing methods. Clearly state "This project does not require a database" and explain alternative data handling methods
3. **For Live Applications**: If a URL is provided, prioritize automated screenshot generation for Chapter 5
4. **Follow exact formatting**: Use bold, italics, underlines, and bullets as shown in the examples
5. **Include comprehensive scope**: Cover all major features, limitations, and technical details
6. Maintain the exact same professional academic tone and structure
7. Ensure all technical details are accurate and relevant to the specified technology stack
8. Create realistic but appropriate project scope and limitations
9. Include proper academic formatting and page layout
10. Generate content that reflects genuine learning outcomes and technical understanding
11. Ensure all sections are comprehensive yet concise
12. Use appropriate technical terminology for the chosen technology stack
13. **Adapt Chapter 4 content** based on whether the project uses a database or not
14. **Include future enhancements section** in the conclusion
15. **Add educational value discussion** in the conclusion
16. **Screenshot Integration**: If live URL provided, use automated screenshot generation with professional descriptions

**Note**: Replace all bracketed placeholders with actual project-specific information to generate a personalized, professional academic project report that meets university standards.
