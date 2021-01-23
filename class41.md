# summery 
## Pre-rendering and Data Fetching
![image](https://sibelius.github.io/reactconf-taming-data-fetching/img/fetch.jpg)
## Pre-rendering.

### By default, Next.js pre-renders every page. This means that Next.js generates HTML for each page in advance, instead of having it all done by client-side JavaScript. Pre-rendering can result in better performance and SEO.Each generated HTML is associated with minimal JavaScript code necessary for that page. When a page is loaded by the browser, its JavaScript code runs and makes the page fully interactive. (This process is called hydration.)



## Check That Pre-rendering Is Happening
### You can check that pre-rendering is happening by taking the following steps:

### Disable JavaScript in your browser (here’s how in Chrome) and Try accessing this page (the final result of this tutorial). You should see that your app is rendered without JavaScript. That’s because Next.js has pre-rendered the app into static HTML, allowing you to see the app UI without running JavaScript.




## Dynamic Routes
![image2](https://nextjs.org/static/images/learn/dynamic-routes/page-path-external-data.png)
### How to Statically Generate Pages with Dynamic Routes
#### In our case, we want to create dynamic routes for blog posts:

#### We want each post to have the path /posts/<id>, where <id> is the name of the markdown file under the top-level posts directory.Since we have ssg-ssr.md and pre-rendering.md, we’d like the paths to be /posts/ssg-ssr and /posts/pre-rendering.


### Development v.s. Production
- In development (npm run dev or yarn dev), getStaticPaths runs on every request.
- In production, getStaticPaths runs at build time.


## Deploying Your Next.js App
![image3](https://scotch-res.cloudinary.com/image/upload/w_1050,q_auto:good,f_auto/v1600204990/ir2cpar6ccap8tguszkw.png)


### Before we deploy, let’s push our Next.js app to GitHub if you haven’t done so already. This will make deployment easier.

1. On your personal GitHub account, create a new repository called nextjs-blog.
2. The repository can be public or private. You do not need to initialize it with a README or other files.


3. If you haven’t initialized the git repository locally for your Next.js app, do so now.
4. Push the Next.js app to your GitHub repository.


### Deploy to Vercel
#### The easiest way to deploy Next.js to production is to use the Vercel platform developed by the creators of Next.js.Vercel is an all-in-one platform with Global CDN supporting static & JAMstack deployment and Serverless Functions. We believe Vercel is the optimal place to deploy Next.js apps.










