# Read: Class 41 React 4
### Next.js - Dynamic Routes 
- To download, install, and run the starter code. This command sets up a nextjs-blog directory.
	- $ npx create-next-app nextjs-blog --use-npm --example "https://github.com/vercel/next-learn/tree/master/basics/dynamic-routes-starter"

- when the page content depends on external data We use getStaticProps to fetch required data to render the index page.
- To create dynamic routes for blog posts: we create a page that is named **`[id].js`** under **`pages/posts`**.
	- Pages that begin square brackets '[' and end with ']' are dynamic routes in next.js
	- Write this code that will render a post page:

		import Layout from '../../components/layout'

		export default function Post() {
  		return <Layout>...</Layout>
		}

- Source from (https://nextjs.org/learn/basics/dynamic-routes/implement-getstaticpaths)
- Source from (https://nextjs.org/learn/basics/dynamic-routes/setup)https://nextjs.org/learn/basics/dynamic-routes/setup


### Next.js - Deployment
- Vercel is a serverless platform for static and hybrid applications built to integrate with your headless content, commerce, or database.

- Deploying nextJS to Vercel which is a platform built by NextJS creators
- Create an account on Vercel from (https://vercel.com/signup)
- You need a github account in order for you to be able to do that
- Push your code to github by these commands
	1. $ git remote add origin https://github.com/<username>/nextjs-blog.git
	2. $ git push -u origin main
- Source from (https://nextjs.org/learn/basics/deploying-nextjs-app)
