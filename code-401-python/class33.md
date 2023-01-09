# Data Fetching 

- Common data fetching practices such as the Fetch API or Axios library works well in React. They can be used to send and fetch data easily.

- But what about caching or data pagination? Or automatic revalidation or request deduplication? Fetch and Axios only can send or fetch data, then return its response, and that’s it.


---
## Beginner’s Guide to SWR: Data Fetching in React

SWR stands for stale-while-revalidate, a HTTP cache invalidation strategy popularized by HTTP RFC 5861. It basically means that it performs data fetching 

- SWR is created by Vercel and one of its advantages is that it is a fast and lightweight package. It is a layer built on top of Fetch API and therefore provides additional features on top of just data fetching. These features include caching, pagination, auto revalidation and more.

--------
- Built-in Cache + Real-Time Experience

When we use Fetch or Axios for data fetching in React, we usually need to show the user some loading message or spinner while data is being fetched. Using SWR’s strategy, the user sees the cached (stale) data first and requests are automatically being cached. Components will always be constantly updated with the most recent data, ensuring UI will always be fast and reactive.

- Auto Revalidation

SWR ensures that the user sees the most up-to-date data. So even with multiple tabs or windows, the data is always fresh and in sync when the window/tab is refocused.

Instead of just revalidating data on focus, SWR can also revalidate data on interval, to make sure multiple sessions will render the same components based on the data.

Finally, there’s revalidation on reconnect. In the event the user disconnects from the internet, SWR will automatically revalidates data once the user is online again.


- Pagination

One of the most useful features of SWR is that it supports pagination and infinite loading of data.

Instead of having to write your own logic with Fetch or Axios to paginate data or create an infinite loading UI for your app, SWR provides a simple Hook called useSWRInfinite to handle this for you.


