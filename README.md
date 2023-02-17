A minimal repo showing issue with loading JS in svelte:head component

to test:

1. npm install
2. npm run dev -- --open
3. go to /other
4. click link (it takes you to /)
5. Observe that `Stripe()` isn't available in onMount even though it is on SSR
