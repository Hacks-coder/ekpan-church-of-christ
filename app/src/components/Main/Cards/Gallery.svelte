<script>
  const galleryOne = [
    { src: "/members/img1.jpg", alt: "Image 1", w: "w-45 @xl:90", h: "h-30" },
    { src: "/members/img2.jpg", alt: "Image 2",w: "w-45 @xl:90", h: "h-35" }, 
    { src: "/members/img3.jpg", alt: "Image 3",w: "w-45 @xl:90", h: "h-30" }  
  ];
  // const galleryTwo = [
  //   { src: "/members/img4.jpg", alt: "Image 4", w: "w-40", h: "h-57" },
  //   { src: "/members/img5.jpg", alt: "Image 5", w: "w-40", h: "h-40" } 
  // ];
</script>

<div class="@container">
  <div class="flex gap-3 px-2">
    <div class="flex flex-col gap-2 border-4">
      {#each galleryOne as { src, alt, w, h}}
        <div class={`${w} ${h} @xl:w-60 bg-amber-900 bg-cover bg-center rounded-md`}
             style="background-image: url({src})"
             role="img"
             aria-label={alt}>
        </div>
      {/each}
    </div>

    <div class="flex flex-col gap-2">
      <!-- {#each galleryTwo as { src, alt, w, h }}
        <div class={`${w} ${h} bg-green-500 bg-cover bg-center rounded-md`}
             style="background-image: url({src})"
             role="img"
             aria-label={alt}>
        </div>
      {/each} -->
    </div>
  </div>
</div>
