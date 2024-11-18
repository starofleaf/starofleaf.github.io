
# 2024 Duke GDDI Portfolio Template

## Overview

Welcome to the 2024 Duke GDDI Portfolio Template! This repository provides a simple, configurable, and professional portfolio template for students. The template is built as a static site and uses GitHub Pages—a free, easy-to-set-up hosting solution—making it ideal for engineers and developers to showcase their work.

### Why Use GitHub Pages?

- **Free Hosting**: No cost for hosting your site.
- **Easy to Deploy**: Simply push your code to the repository, and your site will be live.
- **Professional Presence**: GitHub Pages is a trusted hosting option widely used by engineers and developers.
- **Version Control**: Built-in version control with GitHub makes tracking changes and collaboration seamless.

## Repository Structure

- `index.html` - The main HTML file of the website. **Tip**: You only need to change the `<title>` tag for custom page titles.
- `config.json` - The primary configuration file for customizing content.
- `assets/` - Built-in assets for the site (icons, etc.). **Do not modify** unless you have a specific need to change built-in assets.
- `projects/` - Folder to store project-related images, videos, and other files.
- `photo.jpg` - Your profile picture (replace with your own).
- `RESUME_JAMESYONG_2024_DUKE_GDDI.pdf` - Placeholder for your resume (replace with your own).
- Various favicon and web manifest files for compatibility.

## Quick Start Guide

### Step 1: Create a GitHub Repository

To correctly deploy your site using GitHub Pages, **create a repository with the name `yourusername.github.io`** (replace `yourusername` with your GitHub username).

### Step 2: Clone the Repository

Clone this repository to your local machine:

```bash
git clone git@github.com:jamesyong-42/2024-duke-gddi-portfolio-template.git
```

### Step 3: Customize Your Content

#### 1. Edit the `config.json` File

The `config.json` file contains customizable content for your portfolio. Here is an explanation of each section:

- **Basic Information**
  ```json
  "basic": {
    "name": "Your Name",
    "email": "your-email@example.com",
    "linkedin": "https://www.linkedin.com/in/yourprofile/",
    "resume": "RESUME_YOURNAME_2024.pdf"
  }
  ```
  - **`name`**: Your full name.
  - **`email`**: Your email address for contact.
  - **`linkedin`**: Link to your LinkedIn profile.
  - **`resume`**: Path to your resume file (upload your resume in this repository).

- **Home Content**
  ```json
  "home": {
    "heroSentence": "A brief tagline about yourself",
    "projects": [ ... ]
  }
  ```
  - **`heroSentence`**: A short phrase that summarizes your professional focus.
  - **`projects`**: List of project entries (explained further below).

- **Skills**
  ```json
  "skills": [
    {
      "group": "Technical Skills",
      "skills": ["C++, Python, JavaScript"]
    },
    ...
  ]
  ```

- **Bio**
  ```json
  "bio": "Write a brief biography about yourself.",
  "bioPic": "/photo.jpg"
  ```
  - **`bio`**: Your biography text.
  - **`bioPic`**: Path to your profile picture (e.g., `photo.jpg`).

#### 2. Add Projects

Each project should have the following structure in the `projects` array:

```json
{
  "name": "Project Title",
  "year": "Year",
  "keywords": ["Keyword1", "Keyword2"],
  "shortDesc": "A brief description of the project.",
  "coverImage": "/projects/project-folder/cover.jpg",
  "roles": ["Your Role"],
  "highlights": [
    "Key highlight 1",
    "Key highlight 2"
  ],
  "detail": [
    {
      "type": "paragraph",
      "value": "Detailed description."
    },
    {
      "type": "image",
      "value": "/projects/project-folder/image.jpg"
    },
    {
      "type": "video-muted",
      "value": "/projects/project-folder/video.mp4"
    }
  ]
}
```


#### 3. Upload Files

- **Resume**: Replace `RESUME_JAMESYONG_2024_DUKE_GDDI.pdf` with your own resume.
- **Profile Picture**: Replace `photo.jpg` with your image.
- **Project Media**: Add images and videos in the `projects/` folder for each project.

### Step 4: Deploy with GitHub Pages

1. Go to your GitHub repository.
2. Navigate to **Settings** > **Pages**.
3. Under **Source**, select `main` branch and click **Save**.
4. Your site will be live at `https://yourusername.github.io`.

## Additional Notes

- Make sure all paths in `config.json` are correct for your files.
- Avoid making changes to files in the `assets/` directory unless necessary.
- Test your site locally by opening `index.html` or using a local server before pushing changes.

---

This guide should help you set up and deploy your professional portfolio with minimal effort while providing the flexibility to showcase your unique skills and projects. Happy coding!
