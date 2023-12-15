<script>
    import { onMount } from 'svelte';
    let balance;
    onMount(async () => {
        const response = await fetch(
            "https://bitcointxoko.com/api/v1/wallet",
            {
                method: 'GET',
                headers: {
                    'x-api-key': "fe69e5485e09418d94811fd585f66615",
                },
            },
        );
        const data = await response.json();
        balance = Math.trunc((data.balance) / 1000);
    });
</script>

<div class="p-4 font-bold tech text-3xl text-highlight">
    {#if balance}
        <p>Saldo: <span class="hover:text-amber-400 hover:underline hover:decoration-dashed">{balance}</span> sats</p>
    {:else}
        <p class="animate-pulse">cargando...</p>
    {/if}
</div>
