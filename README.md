<h1 align="center">Next Auth v5 - Advanced Guide</h1>

#### Key Features:

- 🔐 Next-auth v5 (Auth.js)
- 🚀 Next.js 14 with server actions
- 🔑 Credentials Provider
- 🌐 OAuth Provider (Social login with Google & GitHub)
- 🔒 Forgot password functionality
- ✉️ Email verification
- 📱 Two factor verification
- 👥 User roles (Admin & User)
- 🔓 Login component (Opens in redirect or modal)
- 📝 Register component
- 🤔 Forgot password component
- ✅ Verification component
- ⚠️ Error component
- 🔘 Login button
- 🚪 Logout button
- 🚧 Role Gate
- 🔍 Exploring next.js middleware
- 📈 Extending & Exploring next-auth session
- 🔄 Exploring next-auth callbacks
- 👤 useCurrentUser hook
- 🛂 useRole hook
- 🧑 currentUser utility
- 👮 currentRole utility
- 🖥️ Example with server component
- 💻 Example with client component
- 👑 Render content for admins using RoleGate component
- 🛡️ Protect API Routes for admins only
- 🔐 Protect Server Actions for admins only
- 📧 Change email with new verification in Settings page
- 🔑 Change password with old password confirmation in Settings page
- 🔔 Enable/disable two-factor auth in Settings page
- 🔄 Change user role in Settings page (for development purposes only)

### Prerequisites

**Node version 18.7.x**

### Cloning the repository

```shell
git clone https://github.com/Shahriyar-Hosen/next-auth-v5-advanced-guide.git
```

### Install packages

###### npm

```shell
npm i
```

###### yarn

```shell
yarn add
```

###### pnpm

```shell
pnpm i
```

### Setup .env file

```env
# Database Url
DATABASE_URL="mongodb url"

# Next-Auth secret
AUTH_SECRET=next-auth-secret

# Github and Google id and secret
GITHUB_CLIENT_ID="Google id from google api console"
GITHUB_CLIENT_SECRET="Google secret from google api console"
GOOGLE_CLIENT_ID="Github id from Github -> Settings -> Developer Settings -> OAuth Apps"
GOOGLE_CLIENT_SECRET="Github secret from Github -> Settings -> Developer Settings -> OAuth Apps"

# resend (email provider) api key
RESEND_API_KEY="resend api key"

# base url
NEXT_PUBLIC_APP_URL="http://localhost:3000"
```

### Setup Prisma

```shell
npx prisma generate
npx prisma db push
```

### Start the app

```shell
npm run dev
```

## Available commands

Running commands with (npm or yarn or pnpm) `(npm or yarn or pnpm) run [command]`

| command | description                              |
| :------ | :--------------------------------------- |
| `dev`   | Starts a development instance of the app |
