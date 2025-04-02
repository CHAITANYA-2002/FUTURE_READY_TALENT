# Future Ready Talent Internship Project: Techie Pedia

Welcome to **Techie Pedia**, a technology blog platform developed as part of the [Future Ready Talent (FRT)](https://futurereadytalent.in/) virtual internship program by Microsoft, AICTE, NASSCOM, EY, GitHub, and Quess Corp. This project is a static web application designed to showcase tech-related articles on topics like artificial intelligence, machine learning, gadgets, and robotics. It demonstrates web development skills and the use of Microsoft Azure for deployment, fulfilling the FRT program’s objective of upskilling students in cloud technologies.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Deployment](#deployment)
- [Azure Services Used](#azure-services-used)
- [Demo](#demo)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

---

## Overview

**Techie Pedia** is a static web application built to provide a platform for technology enthusiasts to explore articles on innovative tech topics. The website features a responsive blog layout with a carousel banner, multiple blog sections, a sidebar with recent posts and categories, and a subscription form. It was developed during the Future Ready Talent internship to demonstrate proficiency in web development and Azure cloud deployment.

The project focuses on delivering a user-friendly experience with a clean design, interactive elements like a video popup and theme toggle, and deployment on Azure Static Web Apps using GitHub Actions for CI/CD.

---

## Features

- **Responsive Blog Layout**:
  - A carousel banner showcasing featured posts (e.g., "Artificial Intelligence," "Innovative Tech With Machine Learning").
  - Multiple blog sections (2-column, 3-column, and card-based) displaying articles on tech topics.
- **Sidebar**:
  - Recent posts with titles, dates, and images.
  - Categories (e.g., PC Components, Robotics, Tech News) with post counts.
  - About section with a brief description of Techie Pedia.
  - Ads section with a placeholder image.
  - Social media links (Facebook, Twitter, Instagram, Google Plus, YouTube).
- **Interactive Elements**:
  - Light/dark theme toggle in the header.
  - Search bar (placeholder functionality).
  - Video section with a popup to play a Pexels video.
  - Subscription form for email newsletters (placeholder).
- **Instagram Feed**: A grid of images linking to blog posts, styled as an Instagram feed.
- **Navigation**: Links to Home, About, and Contact pages.
- **Scroll-to-Top Button**: A button to return to the top of the page.

---

## Tech Stack

- **Frontend**:
  - HTML: For structuring the web pages.
  - CSS: For styling (`assets/css/style-starter.css`).
  - JavaScript: For interactivity (e.g., carousel, theme toggle, video popup).
- **Libraries/Frameworks**:
  - Bootstrap: For responsive design (`bootstrap.min.js`).
  - jQuery: For DOM manipulation (`jquery-3.3.1.min.js`).
  - Owl Carousel: For the banner slider (`owl.carousel.js`).
  - Magnific Popup: For the video popup (`jquery.magnific-popup.min.js`).
  - Font Awesome: For icons.
  - Google Fonts: Frank Ruhl Libre and Poppins for typography.
- **Cloud Services**:
  - Azure Static Web Apps: For hosting the web application.
- **Version Control**:
  - GitHub: For source code management.
  - GitHub Actions: For CI/CD pipeline to automate deployment to Azure.

---

## Project Structure

The repository is organized as follows:

```
FUTURE_READY_TALENT/
├── assets/                 # Static assets
│   ├── css/                # CSS files
│   │   └── style-starter.css
│   ├── js/                 # JavaScript files
│   │   ├── jquery-3.3.1.min.js
│   │   ├── owl.carousel.js
│   │   ├── jquery.magnific-popup.min.js
│   │   ├── theme-change.js
│   │   ├── bootstrap.min.js
│   │   └── (other JS files as needed)
│   └── images/             # Images for blog posts, ads, etc.
│       ├── banner-blog1..jpg
│       ├── banner-blog2..jpg
│       ├── blog1..jpg
│       ├── blog-s1..jpg
│       ├── testi1...jpg
│       ├── ads..jpg
│       └── (other images)
├── index.html              # Home page
├── about.html              # About page
├── contact.html            # Contact page
├── blog-single.html        # Single blog post page
├── .github/                # GitHub Actions workflows
│   └── workflows/
│       └── azure-static-web-apps.yml # Workflow for deploying to Azure
├── README.md               # Project documentation
└── .gitignore              # Files to ignore in version control
```

---

## Installation

Follow these steps to set up the project locally on your machine.

### Prerequisites
- Git
- A code editor (e.g., VS Code)
- A modern web browser (e.g., Chrome, Firefox)
- An Azure account (for deployment)

### Steps
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/CHAITANYA-2002/FUTURE_READY_TALENT.git
   cd FUTURE_READY_TALENT
   ```

2. **Run Locally**:
   - Since this is a static web app, you can open `index.html` directly in a browser:
     ```bash
     open index.html
     ```
   - Alternatively, use a local development server (e.g., VS Code’s Live Server extension) for a better experience:
     ```bash
     code .  # Open in VS Code
     # Use Live Server extension to launch the app
     ```

---

## Usage

1. **Explore the Blog**:
   - Open the app in a browser to access the home page (`index.html`).
   - Use the carousel banner to view featured posts (e.g., "Artificial Intelligence," "Top 10 Gadgets").
   - Browse blog sections to read articles on topics like laptops, smartphones, and robotics.
   - Check the sidebar for recent posts, categories, and social media links.
   - Toggle between light and dark themes using the switch in the header.

2. **Interact with Features**:
   - Click the play button in the video section to watch a Pexels video in a popup.
   - Use the subscription form to enter an email address (note: this is a placeholder; no backend is implemented).
   - Navigate to the About and Contact pages using the header links.

3. **Example Blog Post**:
   - Title: "Artificial Intelligence"
   - Author: Techie Pedia
   - Likes: 12
   - Comments: 9
   - Description: "Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet sed do eiusmod tempor incididunt ut labore et dolore magna aliqua."

---

## Deployment

The application is deployed on Azure Static Web Apps using GitHub Actions for CI/CD.

### Deployment Steps
1. **Set Up Azure Static Web Apps**:
   - In the Azure portal, create a new Static Web App.
   - Link your GitHub repository (`CHAITANYA-2002/FUTURE_READY_TALENT`) during setup.
   - Configure the app settings:
     - App location: `/`
     - Output location: `/`
     - API location: (leave blank, as there’s no backend)

2. **GitHub Actions Workflow**:
   - A workflow file (`.github/workflows/azure-static-web-apps.yml`) is likely included to automate deployment.
   - On each push to the `main` branch, the app is built and deployed to Azure.

3. **Access the Deployed App**:
   - After deployment, Azure provides a URL (e.g., `https://<app-name>.azurestaticapps.net`).
   - Note: The exact URL is not specified here as it depends on your deployment setup.

---

## Azure Services Used

This project leverages the following Azure service, as required by the Future Ready Talent program:

- **Azure Static Web Apps**: Hosts the web application, providing a scalable and secure hosting solution with integrated CI/CD via GitHub Actions.

---

## Demo

A live demo of the project may be available if deployed on Azure Static Web Apps. Check the repository for a deployed link or a demo video (if included).

- **Deployed App Link**: (Provide the Azure Static Web Apps URL if available, e.g., `https://lemon-stone-08a65af10.1.azurestaticapps.net/`.)
- **Demo Video**: (If a demo video is included in the repository, e.g., `demo.mp4`, mention it here.)

---

## Contributing

Contributions are welcome! If you’d like to contribute to this project, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Make your changes and commit them:
   ```bash
   git commit -m "Add your commit message"
   ```
4. Push to your branch:
   ```bash
   git push origin feature/your-feature-name
   ```
5. Create a pull request with a detailed description of your changes.

Please ensure your code follows standard web development practices (e.g., clean HTML/CSS/JS, responsive design) and includes appropriate documentation.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details (if included in the repository; otherwise, you may need to add one).

---

## Contact

For questions, suggestions, or collaboration opportunities, feel free to reach out:

- **GitHub**: [CHAITANYA-2002](https://github.com/CHAITANYA-2002)
- **Email**: (Add your email here if you’d like to share it)

Thank you for exploring my Future Ready Talent Internship Project! Techie Pedia reflects my skills in web development and Azure deployment, gained through the FRT program. I hope it serves as an inspiring example for others interested in building static web applications with cloud integration. Happy coding! 🚀
