<template>
  <b-container fluid>
    <div class="container">
      <b-carousel
        :interval="4000"
        class="carousel m-4"
        controls
        indicators
        img-width="1024"
        img-height="480"
      >
        <b-carousel-slide
          v-for="(slide,i) in carousel"
          :key="i"
          :caption="slide.caption"
          :text="slide.text"
          :img-src="slide.img"
        />
      </b-carousel>
    </div>
    <b-row class="bg-info text-white p-5 my-5">
      <h2>Parrafo</h2>
      <p>{{ lorem }}</p>
      <p>{{ lorem }}</p>
      <p>{{ lorem }}</p>
    </b-row>
    <b-row class="my-5">
      <div class="container">
        <b-card-group deck>
          <b-card
            v-for="(card,i) in cards"
            :key="i"
            :title="card.title"
            :img-src="card.src"
            :img-alt="card.alt"
            img-top
          >
            <p class="card-text">
              This is a wider card with supporting text below as a
              natural lead-in to additional content. This content
              is a little bit longer.
            </p>
            <div slot="footer">
              <small class="text-muted">Last updated 3 mins ago</small>
            </div>
          </b-card>
        </b-card-group>
      </div>
    </b-row>
  </b-container>
</template>

<script>
const lorem = `Lorem ipsum dolor sit amet consectetur adipisicing elit. Soluta sint est ipsam, beatae repudiandae harum autem eius molestias corporis molestiae eum  tempora nulla natus repellendus architecto minus in recusandae. Quod, repellendus nemo aliquam quam animi non, consequuntur explicabo eius molestiae qui placeat voluptates adipisci, ex distinctio nam magnam perferendis. Perferendis quo asperiores autem assumenda commodi quaerat deleniti. Nulla, ipsum? Distinctio nobis dolorem laudantium nam perspiciatis sit harum voluptas adipisci necessitatibus corrupti rem laborum doloremque porro totam quidem explicabo maiores alias fuga aliquam, incidunt sunt ad ex numquam. Adipisci, repellendus? Distinctio architecto illum sint beatae at labore aperiam optio velit itaque! Cupiditate dignissimos hic rerum fuga quam. Laboriosam, error quae? Commodi placeat exercitationem soluta illum dicta magnam ea perferendis provident. Numquam tenetur dolore nam inventore modi quia sed, rerum ut? Ut id deleniti, pariatur eum odio dolor rem iure temporibus delectus explicabo expedita officia commodi consequatur, numquam nihil dolorum quaerat.`
export default {
  data() {
    return {
      lorem,
      carousel: [
        {
          caption: 'imagen 1',
          text: 'muelle',
          img: 'https://picsum.photos/1024/480/?image=52'
        },
        {
          caption: 'imagen 2',
          text: 'montaña',
          img: 'https://picsum.photos/1024/480/?image=54'
        },
        {
          caption: 'imagen 3',
          text: 'faro',
          img: 'https://picsum.photos/1024/480/?image=58'
        }
      ],
      cards: [
        {
          title: 'Title',
          src: 'https://picsum.photos/300/300/?image=41',
          alt: 'img'
        },
        {
          title: 'Title',
          src: 'https://picsum.photos/300/300/?image=41',
          alt: 'img'
        },
        {
          title: 'Title',
          src: 'https://picsum.photos/300/300/?image=41',
          alt: 'img'
        }
      ]
    }
  }
}
</script>
