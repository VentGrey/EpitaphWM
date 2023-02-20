<script lang="ts">
    let contributors = [];

    /* Try to fetch the current contributors */
    fetch("https://api.github.com/repos/VentGrey/Epitaph/contributors")
    .then(res => res.json())
    .then(data => {
        contributors = data;
    })
    .then(() => {
        contributors.forEach(contributor => {
            fetch(contributor.url)
            .then(res => res.json())
            .then(user => {
                contributor.avatar_url = user.avatar_url;
            });
        });
    });
</script>

<section class="container my-2 text-light">
    <p class="display-5 fw-bold">Special thanks!</p>
    <p class="fw-light small">Here is a small hall of fame. These are the people who have contributed to Epitaph so far!</p>
</section>

<section class="text-light container">
<table class="table table-striped table-dark">
  <thead>
    <tr>
      <th>Contributor</th>
      <th>Contributions</th>
      <th>Avatar</th>
    </tr>
  </thead>
  <tbody>
    {#each contributors as contributor}
      <tr>
        <td>
          <a class="text-decoration-none text-light fw-bold" rel="noreferrer" href={contributor.html_url} target="_blank">{contributor.login}</a>
        </td>
        <td>{contributor.contributions}</td>
        <td>
          {#if contributor.avatar_url}
            <img class="rounded-circle" height="64" width="64" src={contributor.avatar_url} alt={contributor.login} />
          {:else}
            <span>No avatar</span>
          {/if}
        </td>
      </tr>
    {/each}
  </tbody>
</table>
</section>