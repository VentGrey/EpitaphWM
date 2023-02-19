<script lang="ts">
    const year: number = new Date().getFullYear();
    
    import GitHub from "svelte-bootstrap-icons/lib/Github.svelte";
    import Left from "svelte-bootstrap-icons/lib/SignTurnLeft.svelte";

    import logo from "./assets/icon.png";
</script>


<div class="container">
    <footer class="d-flex flex-wrap justify-content-between align-items-center py-3 my-4">
        <div class="col-md-4 d-flex align-items-center">
            <a href="/" class="mb-3 me-2 mb-md-0 text-muted text-decoration-none lh-1">
                <img height="32" width="32" src="{logo}" alt="La Esquina Gris logo">
            </a>
            <span class="mb-3 mb-md-0 text-light">© {year} <a class="text-light" href="https://ventgrey.github.io">VentGrey & La Esquina Gris</a></span>
        </div>
        
        <ul class="nav col-md-4 justify-content-end list-unstyled d-flex">
            <li class="ms-3"><a class="text-light" href="https://github.com/VentGrey/Epitaph"><GitHub height={48} width={48}/></a></li>
            <li class="ms-3"><a class="text-yellow" href="https://github.com/leftwm/leftwm"><Left height={48} width={48}/></a></li>
        </ul>
    </footer>

    <p class="fw-light text-light small">This site is 100% free of analytics or any tracking JavaScript.</p>
</div>