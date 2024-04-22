
# WebProdigies Fuzzie App

## Introduction

WebProdigies Fuzzie App is a SaaS automation application designed to automate various tasks for individuals and organizations. It offers features such as sending messages to Discord servers, creating tasks in Notion, joining Slack channels, sending messages, organizing conversations, and uploading images to Google Drive. The application also includes authentication using Clerk, a modern and secure authentication service. It is built using Next.js 14, Tailwind CSS, Neon Postgres, and other technologies to provide a modern user experience with a clean UI.


## Technologies Used

- Frontend:
  - Next.js 14
  - Tailwind CSS
  - Clerk Authentication
  - UploadCare
  - Shadcn for components
  - Aceternity UI
  - React libraries (react-dom, react-hook-form, react-resizable-panels, reactflow, framer-motion)
- Backend:
  - Neon Postgres
  - Prisma ORM
  - Stripe for payment features
## Setup

- Clone the repository to your local machine.

- Install dependencies using `npm install`.

- Set up environment variables in a .env file. See the sample below:

```
# Clerk Authentication
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/dashboard
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/dashboard
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=<your_clerk_publishable_key>
CLERK_SECRET_KEY=<your_clerk_secret_key>

# Database
DATABASE_URL=<your_database_url>

# Application URLs
NEXT_PUBLIC_URL=https://localhost:3000
NEXT_PUBLIC_DOMAIN=localhost:3000
NEXT_PUBLIC_SCHEME=https://

# Google Authentication
NEXT_PUBLIC_GOOGLE_SCOPES=https://www.googleapis.com/auth/drive
NEXT_PUBLIC_OAUTH2_ENDPOINT=https://accounts.google.com/o/oauth2/v2/auth

# UploadCare
NEXT_PUBLIC_UPLOAD_CARE_CSS_SRC=https://cdn.jsdelivr.net/npm/@uploadcare/blocks@
NEXT_PUBLIC_UPLOAD_CARE_SRC_PACKAGE=/web/lr-file-uploader-regular.min.css

# Discord Integration
DISCORD_CLIENT_ID=<your_discord_client_id>
DISCORD_CLIENT_SECRET=<your_discord_client_secret>
DISCORD_TOKEN=<your_discord_token>
DISCORD_PUBLICK_KEY=<your_discord_public_key>
NEXT_PUBLIC_DISCORD_REDIRECT=https://discord.com/oauth2/authorize?client_id=<CLIENTID>&response_type=code&redirect_uri=https%3A%2F%2Flocalhost%3A3000%2Fapi%2Fauth%2Fcallback%2Fdiscord&scope=identify+guilds+connections+guilds.members.read+email+webhook.incoming

# Notion Integration
NOTION_API_SECRET=<your_notion_api_secret>
NOTION_CLIENT_ID=<your_notion_client_id>
NOTION_REDIRECT_URI=https://localhost:3000/api/auth/callback/notion
NEXT_PUBLIC_NOTION_AUTH_URL=https://api.notion.com/v1/oauth/authorize?client_id=<CLIENTID>&response_type=code&owner=user&redirect_uri=https%3A%2F%2Flocalhost%3A3000%2Fapi%2Fauth%2Fcallback%2Fnotion

# Slack Integration
SLACK_SIGNING_SECRET=<your_slack_signing_secret>
SLACK_BOT_TOKEN=<your_slack_bot_token>
SLACK_APP_TOKEN=<your_slack_app_token>
SLACK_CLIENT_ID=<your_slack_client_id>
SLACK_CLIENT_SECRET=<your_slack_client_secret>
SLACK_REDIRECT_URI=https://localhost:3000/api/auth/callback/slack
NEXT_PUBLIC_SLACK_REDIRECT=https://slack.com/oauth/v2/authorize?client_id=<CLIENTID>&scope=chat:write,channels:read,groups:read,mpim:read,im:read&user_scope=chat:write,channels:read,groups:read,mpim:read,im:read&redirect_uri=https%3A%2F%2Flocalhost%3A3000%2Fapi%2Fauth%2Fcallback%2Fslack

# Stripe
STRIPE_SECRET=<your_stripe_secret_key>

```

- Run the application using `npm run dev`.
- Access the application in your web browser at `https://localhost:3000`.


## Usage

- Register and log in using Clerk authentication.
- Explore various automation features such as sending messages, creating tasks, joining channels, and uploading images.
- Manage tasks and configurations from the dashboard.


## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!
## Deploy on vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.

## Acknowledgements

- This project was built to simplify and automate tasks for individuals and organizations.
- Special thanks to the creators and maintainers of the libraries and tools used in this project.

