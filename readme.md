## Deployment Guide

Follow these steps to deploy the site using GitHub and Vercel:

1. **GitHub Repository Setup**  
   - Create a new repository on GitHub (e.g., **Elevan-website**).  
   - Upload all the project files (the HTML, CSS, JS config files, etc.) to the repository. You can do this by dragging and dropping the files into the GitHub repo or using the GitHub Desktop app.  
   - Ensure the repository contains `index.html` at the root, as well as the `src/`, `dist/`, and configuration files.

2. **Vercel Deployment**  
   - Log in to [Vercel](https://vercel.com/) and click **New Project**.  
   - Import the GitHub repository you just created.  
   - For **Framework Preset**, choose **Other** (since this is a static HTML site).  
   - In the project **Settings**:  
     - Set the **Build Command** to `npm run build`. This will run Tailwind CSS and generate the `dist/output.css` file.  
     - Set the **Output Directory** to `.` (the root directory). This tells Vercel to deploy the files from the root of the repository (including the generated CSS in `dist/`).  
   - Click **Deploy**. Vercel will install dependencies and run the build process. Once completed, it will deploy the site.  
   - After a few moments, you will get a live URL for your site. Visit that URL to see the Elevan landing page in action.

**Note:** If Vercel’s build settings prompt for an output directory and does not accept `.` as a value, you can alternatively do the following: open your Vercel project’s **Settings**, navigate to **General → Build & Output Settings**, and specify the output directory as the root (leave it blank or use `./`). This will ensure Vercel deploys the root directory files after building.

Once deployed, your one-page Elevan website should be live and responsive on all devices. You can share the Vercel URL or set up a custom domain through Vercel’s dashboard if desired. Enjoy your new site!
