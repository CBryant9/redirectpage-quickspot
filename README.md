# Quick Spot Redirect Page

A simple, elegant redirect page for Quick Spot customers after they complete their Stripe payment setup.

## Features

- Clean, modern design with smooth animations
- Responsive layout that works on all devices
- Clear step-by-step instructions for customers
- Optimized for Vercel deployment

## Deployment to Vercel

### Option 1: Deploy via Vercel CLI

1. Install Vercel CLI globally:
   ```bash
   npm install -g vercel
   ```

2. In the project directory, run:
   ```bash
   vercel
   ```

3. Follow the prompts to link your project to Vercel

4. Deploy to production:
   ```bash
   vercel --prod
   ```

### Option 2: Deploy via Vercel Dashboard

1. Go to [vercel.com](https://vercel.com) and sign in
2. Click "New Project"
3. Import your Git repository or drag and drop the project folder
4. Vercel will automatically detect it as a static site
5. Click "Deploy"

## Project Structure

```
├── index.html          # Main HTML file with embedded CSS
├── vercel.json         # Vercel configuration
├── package.json        # Project metadata
└── README.md          # This file
```

## Configuration

The `vercel.json` file is configured to:
- Serve the static HTML file
- Route all requests to `index.html` (for SPA-like behavior)
- Set appropriate cache headers for optimal performance

## Customization

To modify the content:
1. Edit `index.html`
2. Update the text, styling, or contact information as needed
3. Redeploy to Vercel

## Contact

For questions about this redirect page, contact: quickspot.help@gmail.com
