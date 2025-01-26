# DFirst Trader - Deriv OAuth2 Redirect Handler

This is a simple static site that handles the OAuth2 redirect flow for the DFirst Trader mobile app. When users authorize the app on Deriv, they are redirected to this page, which then redirects them back to the mobile app with the authorization token.

## Development

1. Install dependencies:
```bash
npm install
```

2. Start the development server:
```bash
npm start
```

## Deployment

This site is deployed on Render.com as a static site. To deploy:

1. Push changes to the repository
2. Connect the repository to Render.com
3. Create a new Static Site
4. Use the following settings:
   - Build Command: `npm install`
   - Publish Directory: `.`

## URL Structure

The redirect URL should be in the format:
```
https://[your-render-domain]/index.html?token1=[deriv-oauth-token]
``` 