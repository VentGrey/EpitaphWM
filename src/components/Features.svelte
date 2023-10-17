<script lang="ts">
    /* Import icons */
    import Palette from "svelte-bootstrap-icons/lib/Palette.svelte";
    import Battery from "svelte-bootstrap-icons/lib/BatteryCharging.svelte";
    import Boxes from "svelte-bootstrap-icons/lib/Boxes.svelte";
    import ArrowRight from "svelte-bootstrap-icons/lib/ArrowRight.svelte";
    import Book from "svelte-bootstrap-icons/lib/Book.svelte";
    import Bar from "svelte-bootstrap-icons/lib/WindowDesktop.svelte";
    import Update from "svelte-bootstrap-icons/lib/ArrowRepeat.svelte";
</script>

<style>
    .text-bg-blue {
        background-color: #89b4fa;
    }

    .text-bg-yellow {
        background-color: #f9e2af;
    }

    .text-bg-purple {
        background-color: #cba6f7;
    }

    .text-bg-green {
      background-color: #a6e3a1;
    }

    .text-bg-pink {
      background-color: #f5c2e7;
    }

    .text-bg-red {
      background-color: #f38ba8;
    }
</style>

<div id="content" class="container px-4 py-5 text-light">
    <h2 class="pb-2 fw-bold display-4">Features</h2>
    <p class="lead">Epitaph comes with a handful of features for you to enjoy using it first-time. These are the most important ones:</p>
    <div class="row g-4 py-5 row-cols-1 row-cols-lg-3">
      <div class="col">
        <div class="d-inline-flex align-items-center justify-content-center text-bg-blue rounded-circle text-dark fs-2 mb-3">
          <Palette class="p-2" width=1.5em height=1.5em/>
        </div>
        <h3 class="fs-2">Catppucchin Palette</h3>
        <p>Catppucchin has one of the best pastel-color palettes out there. The mocha variant is specially gentle on the eyes, while also giving a colorful experience.</p>
        <a href="https://github.com/sponsors/catppuccin" class="d-inline-flex align-items-center text-light fw-bold text-decoration-none">
          Support Catppucchin <ArrowRight class="mx-1"/>
        </a>
      </div>
      <div class="col">
        <div class="d-inline-flex align-items-center justify-content-center text-bg-yellow rounded-circle text-dark fs-2 mb-3">
          <Battery class="p-2" width="1.5em" height="1.5em"/>
        </div>
        <h3 class="fs-2">Tiny Power Manager</h3>
        <p>Epitaph comes with a tiny power manager written in Rust. It's DE/WM agnostic and it tries to be as light as possible to help you manage your battery life.</p>
        <a rel="noreferrer" target="_blank" href="https://github.com/VentGrey/Epitaph/wiki/Goodie:-battery-notify" class="d-inline-flex align-items-center text-light fw-bold text-decoration-none">
          Learn More <ArrowRight class="mx-1"/>
        </a>
      </div>
      <div class="col">
        <div class="d-inline-flex align-items-center justify-content-center text-bg-purple rounded-circle text-dark fs-2 mb-3">
          <Boxes class="p-2" width="1.5em" height="1.5em"/>
        </div>
        <h3 class="fs-2">Solid starting point</h3>
        <p>If you don't want to follow the "Epitaph way", you can always use this theme as a starting point to build your own desktop. I heavily encourage you to do so.</p>
        <a rel="noreferrer" target="_blank" href="https://github.com/VentGrey/Epitaph/wiki/Freezing-your-installation" class="d-inline-flex align-items-center text-light fw-bold text-decoration-none">
          Freeze your installation <ArrowRight class="mx-1"/>
        </a>
      </div>


      <div class="col">
        <div class="d-inline-flex align-items-center justify-content-center text-bg-green rounded-circle text-dark fs-2 mb-3">
          <Book class="p-2" width="1.5em" height="1.5em"/>
        </div>
        <h3 class="fs-2">Extensive Documentation</h3>
        <p>Be not afraid. Epitaph comes with a lot of help and coumentation. If you ever get lost or don't know how to start, the wiki has you covered!</p>
        <a rel="noreferrer" target="_blank" href="https://github.com/VentGrey/Epitaph/wiki" class="d-inline-flex align-items-center text-light fw-bold text-decoration-none">
          Read the wiki <ArrowRight class="mx-1"/>
        </a>
      </div>


      <div class="col">
        <div class="d-inline-flex align-items-center justify-content-center text-bg-pink rounded-circle text-dark fs-2 mb-3">
          <Bar class="p-2" width="1.5em" height="1.5em"/>
        </div>
        <h3 class="fs-2">Beautiful Polybar</h3>
        <p>Polybar is already configured for you! Customize your badge, view your currently played song in cmus/spotify and access your applist. Did I mention systray is also included?</p>
        <a rel="noreferrer" target="_blank" href="https://github.com/VentGrey/Epitaph/blob/master/polybar.config" class="d-inline-flex align-items-center text-light fw-bold text-decoration-none">
          View polybar <ArrowRight class="mx-1"/>
        </a>
      </div>

      <div class="col">
        <div class="d-inline-flex align-items-center justify-content-center text-bg-red rounded-circle text-dark fs-2 mb-3">
          <Update class="p-2" width="1.5em" height="1.5em"/>
        </div>
        <h3 class="fs-2">Constantly Updated</h3>
        <p>Being an opinionated theme. I'm constantly adding things to Epitaph. You can stick with me if you like it or you can start your own "left hand path"!</p>
        <a rel="noreferrer" target="_blank" href="https://ko-fi.com/ventgrey" class="d-inline-flex align-items-center text-light fw-bold text-decoration-none">
          Support the project <ArrowRight class="mx-1"/>
        </a>
      </div>
    </div>

    <p>Other features include:</p>

    <ul>
      <li>Preconfigured keybinds and workspaces with icons. ✨</li>
      <li>A good-loking rofi configuration file. 👀</li>
      <li>Auto-backup to your config files at installation time. 📑</li>
      <li>POSIX SH compliant, minimal up and down scripts for faster reloading. ⚡️</li>
      <li>Beautiful custom-made wallpapers. 🖼️</li>
      <li>Auto-magick wallpaper slideshows. 🪄</li>
      <li>Compatible with the latest available LeftWM. 🧬</li>
      <li>A small, lightweight calendar written in Perl.📆</li>
    </ul>
</div>