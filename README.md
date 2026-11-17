# ARC TECH AI — Starter Website

This is a simple static prototype. It is designed to be hosted free on GitHub Pages, Netlify, or Cloudflare Pages.

## Included
- Responsive dashboard
- Sample Hindi script template generator
- Scene-by-scene video prompt planner
- Browser text-to-speech preview (depends on device/browser Hindi voices)
- Google sign-in button placeholder

## Important limitations
- The script/story generators in this starter are templates, not connected generative AI.
- Image/video generation needs a third-party service or model. Free tiers have limits and can change.
- YouTube uploading requires Google OAuth consent setup and YouTube Data API configuration.
- Google Login is NOT active until Firebase is configured.

## Enable Google Login (Firebase)
1. Create a Firebase project at https://console.firebase.google.com/
2. Add a Web App and copy its Firebase config.
3. In Firebase Authentication > Sign-in method, enable Google.
4. Add your deployed website domain under Authentication > Settings > Authorized domains.
5. Replace the login placeholder in `index.html` with Firebase Authentication code and your project config.
6. Never publish private service-account keys or API secrets in frontend code.

## Publish for free
1. Create a GitHub repository.
2. Upload `index.html`.
3. In repository Settings > Pages, deploy from the main branch.
4. Open the Pages URL shown by GitHub.

For a real AI version, add a secure backend so API keys are not exposed in browser JavaScript.
