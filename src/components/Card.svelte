<script>
  export let cardInfo = {
    title: "",
    cardTitle: "",
    cardDescription: "",
    image: "",
    imageAlt: "",
    color: "",
    route: "",
  };
</script>

<div class={`w-56 h-80 rounded ${cardInfo.color}`}>
  <img class="object-cover" alt={cardInfo.imageAlt} src={cardInfo.image} />
  <h2>{cardInfo.title}</h2>
</div>
