<script>
  export let item = {
    title: '',
    stacks: [
      {
        image: '',
      },
    ],
  };
</script>

<div class="speciality-container">
  <p class="text-base text-black">{item.title}</p>
  <div class="flex flex-row mt-3 justify-start">
    {#each item.stacks as stack, index (index)}
      <img src={stack.image} alt="" class="mx-1 w-6" />
    {/each}
  </div>
</div>
