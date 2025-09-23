# Quinn's Website
---
- Built using Astro
- Served from AWS S3

## Deployment
- For development: `npm run dev`
- For deployment on AWS (must have AWS CLI installed and configured)
    - Automatically deploys on push to Github
    - Manual deployment:
        ```
        $ npm run build
        $ aws s3 sync dist/ s3://quinn-merkel --delete
        ```