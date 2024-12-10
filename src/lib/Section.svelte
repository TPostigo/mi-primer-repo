<script>
    export let title;
    export let items;
  </script>
  
  <section class="section">
    <h2>{title}</h2>
    <div class="carousel">
      {#each items as item}
        <div class="card">
          <img src={item.img} alt={item.title} />
          <p>{item.title}</p>
        </div>
      {/each}
    </div>
  </section>
  
  <style>
    .section {
      padding: 2rem;
      color: #fff;
    }
    .carousel {
      display: flex;
      gap: 2rem;
      overflow-x: auto;
    }
    .card {
      text-align: center;
      width: 150px;
    }
    img {
      width: 100%;
      height: 230px;
      border-radius: 8px;
      border: solid 3px #216AF7;
    }
  </style>
  