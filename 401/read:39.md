# Read: Class 39 React 3
- There are many important details to consider to build a complete react web application from scratch.
	1. Code has to be bundled using a bundler like webpack and transformed using a compiler like Babel.
	2. You need to do production optimizations such as code splitting.
	3. You might want to statically pre-render some pages for performance and SEO. You might also want to use server-side rendering or client-side rendering.
	4. You might have to write some server-side code to connect your React app to your data store.
	- A frame work solves all these problems
	- NextJS is a react framework that solves all the problems listed above.

- Use this command in your terminal to create a next application
	- $ npx create-next-app nextjs-blog --use-npm --example "https://github.com/vercel/next-learn/tree/master/basics/learn-starter"

	- Then cd inside the directory that has been made and run $ npm run dev or $ yarn dev
- After running the commands above you should see a starter nextjs page 1. Documentation 2. Learn 3. Examples 4. Deploy
- Open pages/index.js  and edit your code there.
- As soon as you save the file the browser automatically updates the page with the new text.

- Source from (https://nextjs.org/learn/basics/create-nextjs-app)
- Second Source (https://nextjs.org/learn/basics/create-nextjs-app/setup)
- Third Source (https://nextjs.org/learn/basics/create-nextjs-app/welcome-to-nextjs)
- Fourth Source (https://nextjs.org/learn/basics/create-nextjs-app/editing-the-page)