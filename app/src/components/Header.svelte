<script>
  export let items = [];
</script>

<!-- # markup (zero or more items) goes here -->
<div class="nav">
  <ul>
    {#each items as item}
      <li><div>{item.title}</div></li>
    {/each}
  </ul>
</div>

<div class="nav2">
    {#each items as item}
      <div>{item.title}</div>
    {/each}
</div>

<style lang="scss">
  .nav {
    background: yellow;
    ul {
      display: flex;
      justify-content: space-around;
      align-items: center;
      height: 200px;
      li {
        list-style: none;
        border: 1px solid dodgerblue;
        border-radius: 5px;
        padding: 10px 20px;
        &:hover {
          background: dodgerblue;
        }
      }
    }
  }

  .nav2 {
    background: yellow;
    height: 200px;
    display: flex;
    justify-content: space-around;
    align-items: center;
    div {
      border: 1px solid dodgerblue;
      padding: 10px 20px;
      border-radius: 5px;
      cursor: pointer;
      &:hover {
        background: dodgerblue;
      }
    }

  }
</style>
