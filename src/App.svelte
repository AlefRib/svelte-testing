<script lang="ts">
  import { Class } from "./../node_modules/@eslint/eslintrc/node_modules/type-fest/source/basic.d.ts";
  import Dog1 from "../src/assets/images/dog1.png";
  import Dog2 from "../src/assets/images/dog2.png";
  import { writable } from "svelte/store";
  import logo from "./assets/svelte.png";
  import Card from "./components/Card.svelte";
  import PageTitle from "./components/PageTitle.svelte";

  const cardHome = [
    {
      title: "Test1",
      cardTitle: "Title1",
      cardDescription: "description",
      image: Dog1,
      imageAlt: "Imagem teste",
      color: "bg-cyan-500",
      route: "/adotar",
    },
    {
      title: "Test2",
      cardTitle: "Title2",
      cardDescription: "description2",
      image: Dog2,
      imageAlt: "Imag em teste",
      color: "bg-cyan-500",
      route: "/adotar1",
    },
  ];
</script>

<main class="text-center mx-0">
  <div
    class="bg-indigo-600 text-cyan-500 p-5 flex items-center justify-between"
  >
    <img class="w-10" alt="logo" src={logo} />
    <div>
      <button
        class="max-w-xs sm:max-w-none my-4 text-lg font-semibold bg-cyan-500 text-indigo-600 p-3 rounded-full mr-4"
      >
        Quer Ajudar?
      </button>
      <button class="max-w-xs sm:max-w-none my-4 text-lg font-semibold  ">
        Entre em contato
      </button>
    </div>
  </div>
  <!-- <PageTitle title="Quer Ajudar" subtitle="E você?" /> -->
  <div class="flex justify-center items-center gap-x-4 p-11">
    <!-- {#each cardHome as card}
      <Card cardInfo={card}></Card>
    {/each}	 -->

    <div class="flex justify-between items-center  w-full">
      <div class="text-start flex flex-col gap-8">
        <h1 class="text-5xl">ONG DE ANIMAIS</h1>
        <h3 class="text-3xl">
          Ajudando a encontrar lares paras todos os animais
        </h3>
        <button class="bg-lime-700 p-6 text-white max-w-sm">Quero Adotar</button
        >
      </div>
      <img alt="Imagem de um cachorro sentado" src={Dog1} />
    </div>
  </div>
</main>

<style lang="postcss">
  :root {
    --svelte-rgb: 255, 62, 0;
    background-color: rgb(79 70 229);
  }
</style>
