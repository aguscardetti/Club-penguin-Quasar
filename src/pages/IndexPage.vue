<template>
  <q-page class="q-pa-md">
    <q-card class="q-mb-md">
      <q-card-section class="title-section">
        <div class="text-h6">Curiosidades de Club Penguin</div>
        <div class="text-subtitle1">¡Descubre algunas cosas interesantes sobre Club Penguin!</div>
      </q-card-section>
    </q-card>
    <q-list bordered>
      <q-item v-for="curiosidad in curiosidades" :key="curiosidad.id" class="curiosidad-item">
        <q-item-section>
          <div class="curiosidad-img-container">
            <q-img :src="curiosidad.img" :alt="curiosidad.text" :class="{'curiosidad-img-redonda': curiosidad.redonda, 'curiosidad-img': !curiosidad.redonda}"></q-img>
          </div>
          <q-item-label class="curiosidad-text">{{ curiosidad.text }}</q-item-label>
        </q-item-section>
      </q-item>
    </q-list>
    <div class="additional-text">
      <p>Lanzamiento y Creación:Fecha de lanzamiento: Club Penguin fue lanzado el 24 de octubre de 2005.
Desarrollador: Fue creado por New Horizon Interactive, una compañía canadiense que luego se convirtió en Disney Canada Inc.</p>
      <p>Adquisición por Disney:En agosto de 2007, Disney adquirió Club Penguin por $700 millones. Esta adquisición ayudó a expandir la audiencia del juego y a mejorar su infraestructura en dispositivos móviles.</p>
      <p>Popularidad:Usuarios registrados: En su apogeo, Club Penguin tenía más de 200 millones de cuentas registradas.
        Idioma: El juego estaba disponible en múltiples idiomas, incluyendo inglés, español, francés, portugués y alemán, lo que permitió una base de jugadores global.</p>
      <p>Monetización:Membresías: Aunque el juego básico era gratuito, Club Penguin ofrecía membresías pagadas que daban a los jugadores acceso a ropa, mascotas y muebles exclusivos.
        Microtransacciones: Los jugadores podían comprar monedas virtuales con dinero real para gastar en artículos dentro del juego.</p>
      <p>Mascotas Puffles:Introducción: Los puffles, pequeñas criaturas peludas, fueron introducidos en el juego como mascotas que los jugadores podían adoptar.
        Variedad: Había diferentes colores y tipos de puffles, cada uno con su propia personalidad y habilidades.</p> 
      <p>Eventos Especiales:Club Penguin organizaba eventos y fiestas temáticas mensuales, como la Fiesta de Halloween, la Fiesta de Navidad y la Fiesta Medieval. Estos eventos incluían decoraciones especiales, minijuegos y artículos exclusivos.</p>
      <p>Cierre del Juego:Fecha de cierre: Club Penguin cerró oficialmente el 29 de marzo de 2017.
        Razón: El cierre se debió a una disminución en la popularidad del juego y a la transición hacia una nueva plataforma, Club Penguin Island, que también cerró en diciembre de 2018.</p>  
    </div>
  </q-page>
</template>

<script>
export default {
  name: 'IndexPage',
  data() {
    return {
      curiosidades: [
        { id: 1, text: 'Club Penguin fue lanzado en octubre de 2005.', img: 'https://i.blogs.es/912bfd/650_1000_image-1/1366_2000.webp', redonda: true },
        { id: 2, text: 'El juego fue creado por New Horizon Interactive.', img: 'https://www.theedigital.com/wp-content/uploads/2016/04/Horizon-Interactive-Awards-Logo-White.jpg', redonda: false },
        { id: 3, text: 'Club Penguin llegó a tener más de 200 millones de cuentas registradas.', img: 'https://dl6pgk4f88hky.cloudfront.net/2021/06/cpr_269_3-1038x689.png', redonda: true },
        { id: 4, text: 'Disney adquirió Club Penguin en 2007 por $700 millones (dinerito riko).', img: 'https://cplabur0.files.wordpress.com/2012/04/club-penguin-logo.png?w=640', redonda: false },
        { id: 5, text: 'El juego cerró oficialmente el 29 de marzo de 2017 (Disney haciendo de Disney).', img: 'https://radnorite.com/wp-content/uploads/2017/05/screen-shot-2017-05-16-at-10-44-20-am.png', redonda: false }
      ]
    };
  }
};
</script>

<style scoped>
.text-h6 {
  font-weight: bold;
}
.text-subtitle1 {
  margin-bottom: 16px;
}
.curiosidad-item {
  padding: 12px;
}
.curiosidad-img-container {
  text-align: center; /* Centra la imagen horizontalmente */
}
.curiosidad-img {
  width: 300px;
  height: auto;
  margin-bottom: 8px; /* Espacio entre la imagen y el texto */
}
.curiosidad-img-redonda {
  width: 300px;
  height: auto;
  border-radius: 50%;
  margin-bottom: 11px; /* Espacio entre la imagen y el texto */
}
.curiosidad-text {
  font-size: 18px;
  line-height: 1.5;
  color: #555;
  text-align: center; /* Centra el texto horizontalmente */
}

/*Posdata para el señor Ariel Onoriaga: No me pegues por dejar comentado el codigo, es para acordarme que hace cada cosa :v*/

.additional-text {
  margin-top: 24px; /* Espacio superior para separar del contenido anterior */
  text-align: left; /* Centra el texto horizontalmente */
}

.title-main {
  color: #1e90ff; /* Color para el título principal */
}
.title-subtitle {
  color: #32cd32; /* Color para el subtítulo */
}
.title-section {
  text-align: center; /* Centra el título y subtítulo */
}

</style>


