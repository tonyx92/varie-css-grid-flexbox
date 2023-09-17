<script>

import emily from '../assets/images/image-emily.jpg'
import thomas from'../assets/images/image-thomas.jpg'
import jennie from'../assets/images/image-jennie.jpg'
  import Hero from '../components/Hero.svelte';
  import Content from '../components/Content.svelte';
  import Testimonials from '../components/Testimonials.svelte';
</script>



<Hero />

<Content />


<Testimonials />





<style>


*{
    box-sizing: border-box;
    margin:0;
    padding: 0;
}

:root{
    /* colors */

    --soft-red: #fe7867;
    --yellow: #fad400;
    --dark-desaturated-cyan: #25564b;
    --dark-blue: #19536b;
    --dark-moderate-cyan: #458c7e;
    --header-bg: #3ebfff;
    --footer-bg: #8ed0c4;
    --container-bg: #fffbf8;
    --very-dark-desaturated-blue: #23303e;
    --very-drak-grayish-blue: #5a636c;
    --dark-grayish-blue: #818498;
    --grayish-blue: #a7abae;
    --white: #ffffff;


    /* fonts */
    --barlow-font: "Barlow", sans-serif;
    --frauces-font: "Frauces", serif;
}


:global(body){
    
}









.quarto-container{
    display: grid;
    height:  180vh;
    grid-template-areas: 
    'one two three four';
}


</style>