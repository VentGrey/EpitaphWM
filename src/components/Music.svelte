<script lang="ts">
    /* Assets import */
    import camel from "../assets/camel.jpg";
    import crimson from "../assets/kingcrimson.jpg";
    import linkin from "../assets/linkinpark.jpg";
    import opeth from "../assets/opeth.jpg";
    import steven from "../assets/stevenwilson.jpg";

    /* Icons import */
    import HeartFill from "svelte-bootstrap-icons/lib/HeartFill.svelte";
    import Spotify from "svelte-bootstrap-icons/lib/Spotify.svelte";
</script>

<section id="music" class="container text-light">
    <p class="display-5 fw-bold">Support these creators!</p>
    <p class="fw-light small">Epitaph is full of progressive rock / metal references. This is made solely as a tribute to the band(s) I love and listen to, the original idea + artwork concept and registered trademarks are property of the bands mentioned below and their registered trademark holders.</p>
    <p class="fw-light small">I cannot make good music. But I do know how to make "good" code. So, if you like this consider sponsoring this project or, consider helping the original artists ideas!</p>
</section>

<section class="container text-light">
    <p class="h2 fw-light">These music sources served as an inspiration for Epitaph's Development:</p>

    <div class="row text-center">
        <div class="col">
            <figure>
                <img height="150" width="150" class="rounded-3" src="{crimson}" alt="Portada del álbum 'In The Court Of The Crimson King'">
                <div class="d-grid my-2 gap-2">
                    <a rel="noreferrer" target="_blank" href="https://www.dgmlive.com/" class="btn btn-sm btn-dark">Support <HeartFill class="text-red"/></a>
                    <a rel="noreferrer" target="_blank" href="https://open.spotify.com/album/6tVg2Wl9hVKMpHYcAl2V2M?si=jMO4FQJyQD-rxSFPBvVjQw" class="btn btn-sm btn-dark">Listen legally <Spotify class="text-green"/> </a>
                </div>
            </figure>
        </div>
        <div class="col">
            <figure>
                <img height="150" width="150" class="rounded-3" src="{camel}" alt="Portada del álbum 'Mirage'">
                <div class="d-grid my-2 gap-2">
                    <a rel="noreferrer" target="_blank" href="https://www.camelproductions.com/" class="btn btn-sm btn-dark">Support <HeartFill class="text-red"/></a>
                    <a rel="noreferrer" target="_blank" href="https://open.spotify.com/album/4NLWM4hSjXnB1oA6HkIGjc?si=Ux1wzxQjT12DAxL4prx4tw" class="btn btn-sm btn-dark">Listen legally <Spotify class="text-green"/> </a>
                </div>
            </figure>
        </div>
        <div class="col">
            <figure>
                <img height="150" width="150" class="rounded-3" src="{linkin}" alt="Portada del álbum 'Meteora 20th Anniversay'">
                <div class="d-grid my-2 gap-2">
                    <a rel="noreferrer" target="_blank" href="https://www.linkinpark.com/meteora20" class="btn btn-sm btn-dark">Support <HeartFill class="text-red"/></a>
                    <a rel="noreferrer" target="_blank" href="https://open.spotify.com/album/7bN4OM5mtWq0UrAxdN6qMC?si=AI_NdlGkT22uJtTWzdtW0Q" class="btn btn-sm btn-dark">Listen legally <Spotify class="text-green"/> </a>
                </div>
            </figure>
        </div>
        <div class="col">
            <figure>
                <img height="150" width="150" class="rounded-3" src="{opeth}" alt="Portada del álbum 'Orchid'">
                <div class="d-grid my-2 gap-2">
                    <a rel="noreferrer" target="_blank" href="http://www.opeth.com/" class="btn btn-sm btn-dark">Support <HeartFill class="text-red"/></a>
                    <a rel="noreferrer" target="_blank" href="https://open.spotify.com/album/5fAXq1gQeCRjmlAwQQO40Q?si=9ad51f54873e493e" class="btn btn-sm btn-dark">Listen legally <Spotify class="text-green"/> </a>
                </div>
            </figure>
        </div>
        <div class="col">
            <figure>
                <img height="150" width="150" class="rounded-3" src="{steven}" alt="Portada del álbum 'The Raven That Refused To Sing'">
                <div class="d-grid my-2 gap-2">
                    <a rel="noreferrer" target="_blank" href="https://stevenwilsonhq.com/sw/" class="btn btn-sm btn-dark">Support <HeartFill class="text-red"/></a>
                    <a rel="noreferrer" target="_blank" href="https://open.spotify.com/album/2xJFvV7JzoYYMere5rqjVf?si=a8bc17b27d1943e2" class="btn btn-sm btn-dark">Listen legally <Spotify class="text-green"/> </a>
                </div>
            </figure>
        </div>
    </div>
</section>