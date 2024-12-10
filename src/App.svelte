<script>
  import Header from './lib/Header.svelte';
  import Nav from './lib/Nav.svelte';
  import Section from './lib/Section.svelte';
  import Footer from './lib/Footer.svelte';

  // Datos de prueba
  const librosInicio = [
    { id: 1, title: "Libro 1", img: "../public/img/img1.png" },
    { id: 2, title: "Libro 2", img: "../public/img/img2.png"  },
    { id: 3, title: "Libro 3", img: "../public/img/img3.png"  },
    { id: 4, title: "Libro 4", img: "../public/img/img1.png"  },
    { id: 5, title: "Libro 5", img: "../public/img/img2.png" }
    
  ];

  const librosGeneros = [
    { id: 1, title: "Género 1", img: "../public/img/img2.png"  },
    { id: 2, title: "Género 2", img: "../public/img/img3.png" },
    { id: 3, title: "Género 3", img: "../public/img/img1.png" },
    { id: 4, title: "Género 4", img: "../public/img/img2.png" },
    { id: 5, title: "Género 5", img: "../public/img/img3.png" }
  ];

  const librosRecomendaciones = [
    { id: 1, title: "Recomendado 1", img: "../public/img/img3.png" },
    { id: 2, title: "Recomendado 2", img: "../public/img/img1.png" },
    { id: 3, title: "Recomendado 3", img: "../public/img/img2.png" },
    { id: 4, title: "Recomendado 4", img: "../public/img/img3.png" },
    { id: 5, title: "Recomendado 5", img: "../public/img/img1.png" }
  ];
</script>

<Header />
<Nav />
<main>
  <Section title="Inicio" items={librosInicio} />
  <Section title="Géneros" items={librosGeneros} />
  <Section title="Recomendaciones" items={librosRecomendaciones} />
</main>
<Footer />

<style>

:global(body, html) {
  background-color: #1A1B1A;
  font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  
  }
</style>
