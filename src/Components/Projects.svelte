<script>
  import ProjectItem from './ProjectItem.svelte';
  import FooterSvg from '../assets/footer.svg';
</script>

<div class="projects-container">
  <div class="w-full lg:p-32 p-16 pt-10 lg:pt-40">
    <div class="w-4/5 flex lg:flex-row flex-col">
      <div class="">
        <h2 class="projects-title" id="works">
          <span class="menu-number">01.</span> Some of my works
        </h2>
      </div>
      <div class="border-b border-gray-500 my-auto w-1/3 ml-4 pt-3 " />
    </div>
    <div class="project-items-container">
      <ProjectItem />
      <ProjectItem />
      <ProjectItem />
    </div>
  </div>
  <div class="w-full flex justify-center">
    <img src={FooterSvg} alt="" />
  </div>
</div>
