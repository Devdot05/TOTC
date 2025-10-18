<script>
    let count = $state(0)
    $effect(() => {
        console.log('count:', count);
    })
    let username = $state('Guess')
    $effect(() => {
        document.title = `welcome ${username}`
    })

    let seconds = $state(0)
    $effect(() => {
         const timer = setInterval(() => {
             seconds += 1
         }, 1000)
         return () => clearInterval(timer)
    })
</script>

<p>{count}</p>
<button onclick={() => count++}>increase</button>
<p>{username}</p>
<input type="text" bind:value={username} />
<div>seconds pass: {seconds}</div>
