Run `pnpm run dev` then go to [localhost:3000](http://localhost:3000/) and observe this error:

```
Server running at http://localhost:3000
6:23:12 PM [vike][request(1)] HTTP request: /
6:23:15 PM [vite][request(1)] Error when evaluating SSR module /node_modules/.pnpm/@apollo+client@3.8.7_graphql@16.8.1_react-dom@18.2.0_react@18.2.0/node_modules/@apollo/client/react/hooks/internal/__use.js:
|- SyntaxError: The requested module 'react' does not provide an export named 'use'
    at Object.get (file:///home/romu/tmp/vite-regression-2023-nov-14/node_modules/.pnpm/vite@5.0.0-beta.19/node_modules/vite/dist/node/chunks/dep-uqAlfqPp.js:49006:23)
    at eval (/home/romu/tmp/vite-regression-2023-nov-14/node_modules/.pnpm/@apollo+client@3.8.7_graphql@16.8.1_react-dom@18.2.0_react@18.2.0/node_modules/@apollo/src/react/hooks/internal/__use.ts:18:29)
    at instantiateModule (file:///home/romu/tmp/vite-regression-2023-nov-14/node_modules/.pnpm/vite@5.0.0-beta.19/node_modules/vite/dist/node/chunks/dep-uqAlfqPp.js:48897:9)
┌──────────────────────────────────────────────────────────┐
│ Error isn't helpful? See https://vike.dev/errors#verbose │
└──────────────────────────────────────────────────────────┘
6:23:15 PM [vike][request(1)][Warning] No error page found, we recommend defining an error page, see https://vike.dev/error-page
6:23:15 PM [vike][request(1)] HTTP response / ERR
```
