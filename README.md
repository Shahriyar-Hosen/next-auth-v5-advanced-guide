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

### Extract this system configuration

### 1. Install packages

##### npm | yarn | pnpm

```shell
npm i
```

#### 1.1 Install dependencies and devDependencies

##### dependencies

```shell
npm i next-auth@beta @auth/prisma-adapter resend uuid zod bcryptjs react-hook-form @hookform/resolvers next-themes react-icons react-spinners @radix-ui/react-icons
```

##### devDependencies

```shell
npm i -d @types/uuid @types/bcryptjs
```

#### 1.2 Install shadcn-ui

#### 1.3 Install shadcn-ui component

```shell
npx shadcn-ui@latest add button card switch form input select sonner dialog dropdown-menu badge avatar
```

### 2. all file and folder added

### 3. Setup .env file

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

### 4. Setup Prisma

```shell
npx prisma generate
npx prisma db push
```

### 5. Start the app

```shell
pnpm run dev
```

## Available commands

Running commands with pnpm `pnpm run [command]`

| command | description                              |
| :------ | :--------------------------------------- |
| `dev`   | Starts a development instance of the app |
