<script>
    import logo from "$lib/assets/logo.png"
    const nav = [
        {
            title: "г. Златоуст",
            href: "/zlat",
            isShow: true,
        },
        {
            title: "Саткинский МР",
            href: "/sat",
            isShow: true,
        },
        {
            title: "Ашинский район",
            href: "/aha",
            isShow: true,
        },
        {
            title: "Трёхгорный ГО",
            href: "/treh",
            isShow: true,
        },
        {
            title: "Катаав-Ивановский МР",
            href: "/kat",
            isShow: true,
        },
        {
            title: "Усть-Катавский ГО",
            href: "/ustkat",
            isShow: true,
        },
    ];
</script>

<nav>
    <div class="nav-container">
        <img src="{logo}" alt="trash">
        <a href="/" class="nav-logo" title="Back to Homepage">Trash map</a>
        <div class="nav-links">
            {#each nav as link}
                {#if link.isShow}
                    <a href={link.href} class="link">{link.title}</a>
                {/if}
            {/each}
        </div>
    </div>
</nav>