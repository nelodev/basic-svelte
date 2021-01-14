<script>
    const skills = [
        {
            id: 1,
            name: 'React',
        },
        {
            id: 2,
            name: 'Tailwind CSS',
        },
        {
            id: 3,
            name: 'NodeJS',
        }
    ];
</script>

<style>
    .skills {
        display: flex;
        align-items: center;
        justify-content: center;
    }

    ul {
        margin: 0;
        padding: 0;
        list-style: none;
    }

    li {
        display: inline;
        margin: 0 0 0 0.4em;
    }
</style>

<div class="skills">
    <h3>Habilidades</h3>
    <ul>
        {#each skills as {name}, i}
            <li>{name}</li>
        {/each}
    </ul>
</div>