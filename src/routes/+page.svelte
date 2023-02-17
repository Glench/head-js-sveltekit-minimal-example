<script>
    import {onMount} from 'svelte';

    let message = '...'
    onMount(() => {
        if (Stripe) {
           message = 'Stripe() is available!' 
        }
    })
</script>
<svelte:head>
    <script src="https://js.stripe.com/v3/"></script>
</svelte:head>
<h1>{message}</h1>

<p>Above message should always be "Stripe() is available!"</p>

<a href="/other">other</a>
