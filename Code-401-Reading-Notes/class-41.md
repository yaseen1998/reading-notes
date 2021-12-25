# class_41
## Dynamic Routes
 page path depends on external data. Next.js allows you to statically generate pages with paths that depend on external data. This enables dynamic URLs in Next.js.
 
 <img src = 'https://nextjs.org/static/images/learn/dynamic-routes/page-path-external-data.png'/>
 
 ### Implement getStaticPaths
 <img src='https://i.stack.imgur.com/RCmhz.png'/>
 mportant: The returned list is not just an array of strings — it must be an array of objects that look like the comment above. 
 <br>
 The post page is now using the getPostData function in getStaticProps to get the post data and return it as props.
 
 **If you come across an error, make sure your files have the correct code:**

* pages/posts/[id].js should look like this.
* lib/posts.js should look like this.
* (If it’s still not working) The remaining code should look like this.

### Render Markdown
To render markdown content, we’ll use the remark library. First, let’s install it:
```npm install remark remark-html```
```
import { remark } from 'remark'
import html from 'remark-html'
```
