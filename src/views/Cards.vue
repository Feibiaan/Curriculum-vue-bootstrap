<template>
  <div class="mt-5">
      <b-button variant="success">
          Texto
      </b-button>
      <b-button variant="info">
          Texto
      </b-button>
      <b-button variant="danger">
          Texto
      </b-button>
      <b-button variant="primary">
          Texto
      </b-button>
      <b-button variant="warning">
          Texto
      </b-button>
      


    <b-row class="mt-5">
        <b-col cols="12" md="4">
            <b-card
            title="Card Title"
        img-src="https://picsum.photos/600/300/?image=25"
        img-alt="Image"
        img-top
        tag="article"
        style="max-width: 20rem;"
        class="mb-2"
            >
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Assumenda maxime distinctio, reiciendis est minus optio praesentium, impedit maiores atque consectetur possimus laboriosam nam magnam a ipsa alias delectus. Debitis, voluptatem?</p>
                <b-button variant="dark" href="#">
          Texto
      </b-button>
            </b-card>
        </b-col>
    </b-row>

  </div>
</template>

<script>
export default {
    name: 'Cards'
}
</script>