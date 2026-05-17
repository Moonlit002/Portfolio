# Ivan Alfeche's Portfolio

A modern, responsive portfolio website ready to be deployed.

## How to Customize

### 1. Avatar Photo
In `index.html`, replace the avatar image source (line 27) with your own photo URL:
```html
<img src="YOUR_PHOTO_URL_HERE" alt="Ivan Alfeche" class="avatar">
```

### 2. Projects Section
Each project card is wrapped in an `<a>` tag that links to your deployed project. To add your projects:

1. Replace `https://your-project-url-1.com` with your actual project URL
2. Update the project title, description, tags, and GitHub link
3. Repeat for each project

Example project card structure:
```html
<a href="YOUR_PROJECT_URL" target="_blank" class="project-card-link">
    <div class="project-card">
        <div class="project-image">
            <img src="PROJECT_IMAGE_URL" alt="Project Title">
        </div>
        <div class="project-content">
            <h3>Your Project Title</h3>
            <p class="project-description">Brief description of your project...</p>
            <div class="project-tags">
                <span class="tag">Technology1</span>
                <span class="tag">Technology2</span>
            </div>
            <div class="project-links">
                <a href="YOUR_PROJECT_URL" target="_blank" class="project-link" onclick="event.stopPropagation()">Live Demo</a>
                <a href="YOUR_GITHUB_URL" target="_blank" class="project-link" onclick="event.stopPropagation()">GitHub</a>
            </div>
        </div>
    </div>
</a>
```

### 3. Contact Information
Update the email, GitHub, and LinkedIn links in the contact section (lines 128-140).

## Deployment to Render

1. Initialize git repository:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   ```

2. Create a GitHub repository and push your code

3. Go to https://render.com and sign up/sign in

4. Click "New" → "Web Service"

5. Connect your GitHub account and select your repository

6. Configure:
   - Runtime: Node
   - Build Command: `npm install`
   - Start Command: `npm start`

7. Click "Create Web Service"

Your portfolio will be live in a few minutes!
