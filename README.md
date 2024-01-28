# Thread-NextJs_Project


## Authentication

we are using ```Clerk``` for authentication

## Clerk Setup
- go to [Clerk](https://clerk.com/?utm_content=8_4_23&utm_medium=youtube&utm_source=js_mastery&utm_campaign=sponsorship) and create an account


- then go to ```Add Application``` and give an ```application name``` and select which fields you want to use for authentication and click ```Create Application```

- it will show the ```API Key```. copy it and paste it in ```.env.local``` file in the root folder
```env
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=pk_test_Y2FyaW5nLW1hbi0zMi5jbGVyay5hY2NvdW50cy5kZXYk
CLERK_SECRET_KEY=sk_test_EqoYqrdIWE3MbLzpzkjNaMz8onuEbn0uYkZhhFQETO

NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/
```

- then create following structure
```
threads
├── app
|    ├── (auth)
|           ├── sign-in
|           |   ├── [[...sign-in]]
|           |          ├── page.tsx
|           ├── sign-up 
|           |   ├── [[...sign-up]]
|           |          ├── page.tsx
|           ├── layout
├── middleware.ts
```




