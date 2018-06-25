# next.js, fast as gatsby.js

## Headless CMS
- CMS w/o frontend
- Flexible choice for frontend

## Gatsby + Wordpress
- Need to learn GraphQL
- Slow dev lifecycle due to re-fetching all blog data at every dev server start

## Next.js static HTML export
- static route
```js
'/': {page: '/index'}
```
- dynamic route
```js
'/post/hello': {
  page: '/post',
  query: { // some query }
}
```
- saved as routes.json -> server-side render
- use getInitialProps() to identify how to render new components from pathMap

## Performance
- Not bad, but slow compare to gatsby.js
- Due to need to fetch all pages without actual usage
### Problem
- No data splitting + prefetching
- Cause by client routing
### Solution
- Imitate gatsby.js by saving data to .json files
- use getInitialProps() to load content from the .json files instead
### Faster!
- prefetch the content
- use `data-prefetch-link` to prefetch the data (aside from components that are already prefetched)

## Takeaways
- Learn from various tools -> take strong points to create stronger tools
- Give all efforts to the product!