<script>

import group from '../assets/Group.svg'
import linea from '../assets/Vector.svg'
</script>

<div class="card">
        <p class="advice">ADVICE #117</p>
    <div class="content-center">
        <p>"it is easy to sit up and take notice, what's difficult is getting up and take action"</p>
    </div>
    <div class="divisori">
        <img src="{linea}" alt="" class="linea">
        <img src="{group}" alt="">
    </div>
</div>

<style>

*,
*::before,
*::after {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

:root {
    /* colors */
     --light-cyan:#CEE3E9 ;
     --neon-green: #52FFA8;
     --grayish-blue: #4E5D73;
     --dark-grayish-blue: #323A49;
     --dark-blue: #1F2632;

     /* Fonts  */
    --font-body: 'Manrope'
}

:global(body){
    
    place-items: center;
    display: grid;
    place-items: center;
    min-height: 100vh;
    padding: 80px;
    background-color: var(--dark-blue );
}

.card{
    display: grid;
    background-color: var(--dark-grayish-blue);
    padding: 47px 48px 72px 48px;
    border-radius: 15px;
}

.advice{
    color: #52FFA8;
    font-family: var(--font-body);
    font-size: 14px;
    letter-spacing: 3.5px;
    text-align: center;
    margin-bottom: 24px;
}

.content-center{
    color: var(--light-cyan);
    font-family: var(--font-body);
    font-size: 28px;
    letter-spacing: -0.28px;
    text-align: center;
    margin-bottom: 40px;
    min-width: 14ch;
    max-width: 25ch;
}
    
.divisori{
    display: flex;
    justify-content: center;
    align-items: center;
    
}

.linea{
    display: flex;
   position: absolute;
   width: 60%;
   max-width: fit-content;
}






</style>