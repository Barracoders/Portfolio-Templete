# Barracoders Portfolio Template

Welcome to the Barracoders Portfolio Template! This template is designed to help you easily create a personal portfolio even if you have little or no experience with HTML and CSS. Follow the instructions below to set up and customize your portfolio.

## Features

- **Responsive Design**: The template adapts to all screen sizes (mobile, tablet, desktop).
- **Navigation Bar**: Includes a simple navigation bar to link to different sections of the portfolio.
- **Profile Section**: Space for your profile picture, a short bio, and social media links.
- **Projects Section**: Display your projects with titles, descriptions, images, and links to GitHub or live demos.

---

## How to Use This Template

### Step 1: Download the Template

1. Download the files from this repository (`index.html`, `style.css`).
2. Open the files in a code editor (such as [VSCode](https://code.visualstudio.com/)).

### Step 2: Customize Your Portfolio

#### 1. **Edit the Navigation Bar**
   In the `index.html` file, look for the `<nav>` section:
   
   ```html
   <nav>
      <ul>
         <li><a href="#about">About</a></li>
         <li><a href="#projects">Projects</a></li>
         <li><a href="#contact">Contact</a></li>
      </ul>
   </nav>
```
Add more links if needed by copying the `<li>` tags.
Update the link names or IDs if you want to rename the sections.
#### 2. Add Your Profile Picture
In the index.html file, find the section with the placeholder for your profile picture:


```html 
<img src="placeholder.svg" alt="Profile Picture">

```
Replace `placeholder.svg` with the file name of your profile picture.
Ensure the image file is saved in the same folder as index.html.
#### 3. Update the About Me Section
Below the image, you’ll see a space for your bio:

```html

<p>Hi, I'm [Your Name], a web developer passionate about creating interactive and responsive web applications...</p>
```
Replace the placeholder text with a short description about yourself.
Keep it brief and highlight your interests, skills, or goals.
#### 4. Add Social Media Links
You can add or remove links to your social profiles in the .profile-links section:

```html

<a href="https://github.com/yourusername" target="_blank">GitHub</a>
<a href="https://linkedin.com/in/yourusername" target="_blank">LinkedIn</a>
```
Replace the href with links to your actual social media profiles.
You can add more links by copying the `<a>` tag.
#### 5. Add Your Projects
In the `#projects` section, you’ll see a template for displaying your projects:

```html
<div class="project-card">
   <img src="project-image1.jpg" alt="Project 1">
   <h2>Project Title 1</h2>
   <p>This is a description of the project...</p>
   <a href="https://github.com/yourusername/project1" target="_blank">View on GitHub</a>
   <a href="https://your-project-link.com" target="_blank">Live Demo</a>
</div>
```
**Project Image:** Replace `placeholder.svg` with the name of an image file representing your project.

**Project Title:** Replace Project Title 1 with the title of your project.

**Description:** Replace the placeholder text with a short description of your project.

**Links:** Add links to your GitHub repository and live demo, or remove the Live Demo link if not applicable.

To add more projects, simply copy the `<div class="project-card">...</div>` block and paste it below the last project.

#### 6. Customize the Footer
At the bottom of the index.html file, you'll find a footer:

```html
<footer>
  <p>&copy; 2024 Your Name. All rights reserved.</p>
</footer>
```
Replace Your Name with your name or leave it as is.
## Responsive Design
The projects will automatically adjust based on the device screen size:

1 column on phones

2 columns on tablets

3 columns on desktops

There’s no need to manually configure this. The CSS file takes care of it.

## How to Edit Styles
If you want to change the colors, fonts, or layout, you can edit the styles.css file.

#### 1. Change Colors
Find the color values in the CSS file (for example, `#007BFF` for blue).

Replace them with any hex code of your choice.
#### 2. Change Fonts
The default font is set to `Arial`, `sans-serif`. You can replace this with a Google font if you want. Example:
```css
body {
  font-family: 'Roboto', sans-serif;
}
```
To use a Google font, add this to the `<head>` section of `index.html`:
```html

<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
```
#### 3. Change Layout
The layout for the project cards is managed by a CSS grid. You can adjust how many projects show per row by editing the grid styles in the `styles.css` file:
```css

@media (min-width: 768px) {
  .projects-grid {
    grid-template-columns: repeat(2, 1fr); /* 2 columns for tablets */
  }
}

@media (min-width: 1024px) {
  .projects-grid {
    grid-template-columns: repeat(3, 1fr); /* 3 columns for desktop */
  }
}
```
Change the number in `repeat(3, 1fr)` to customize the number of columns.

## How to Host Your Portfolio
#### Barracoders Website:

Send the files to the Barracoders Website team and they will upload them to `{yourname}.barracoders.com` for free
#### GitHub Pages:

You can easily host your portfolio for free using GitHub Pages. Follow their instructions to upload your files and publish the site.
#### Netlify:

Netlify offers free hosting with an easy drag-and-drop interface or GitHub integration.
## Need Help?
If you run into any issues or have questions about customizing your portfolio, feel free to ask for help during meetings. We’re here to support each other!
