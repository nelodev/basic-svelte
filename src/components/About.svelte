<script>
    import Button from './Button.svelte';
    let someText = `Fullstack Developer at Finametrix`;
    let count = 0;
    let styles = { darkMode: false };

    function handleClick() {
        count += 1;
    }

    function toggleDarkMode() {
        styles.darkMode = !styles.darkMode;
        window.document.body.classList.toggle("dark-mode");
    }
</script>

<div class="about">

    {#if !styles.darkMode}
        <p>{someText}</p>
    {:else}
        <p>¡Hello dark mode!</p>
    {/if}


    <Button 
        text='Click' 
        {count}
        on:click={handleClick}
    />
    <Button 
        text={`Toggle ${styles.darkMode ? "light" : "dark"} mode`} 
        on:click={() => toggleDarkMode()} 
    />
</div>