<script>
import qr from '../assets/image-qr-code.png'
</script>

<div class="card">
    <img src={qr} alt="" class="qr">
    <div class="titolo">
        <p>Improve your front-end skills by building projects</p>
    </div>
    <div class="paragrafo">
        <p>Scan the QR code to visit Frontend Mentor and take your coding skills to the next level</p>
    </div>
</div>
<p class="finale">Challenge by <a target="_blank" href="https://www.frontendmentor.io/"> Mentor </a>Coded by <a target="_blank" href="https://github.com/tonyx92?tab=repositories">meself</a></p>

<style>

*,
*::before,
*::after {
    box-sizing: border-box;
    margin:0;
    padding: 0;
    font-family: "Outfit", sans-serif;
   
}

:root{

    /* colors */
    --sfondo: var(#d6e2f0)
    --bianco: var(#FFFFFF)

    /* Fonts */
    --titolo: var("Outfit", sans-serif)

}

:global(body){
    background-color: #d6e2f0;
    display: grid;
    place-content: center;
    min-height: 90vh;
    width: 100%;
}

.qr {
    max-width: 260px;
    max-height: 260px;
    border-radius: 10px;
}

.card{
    display: grid;
    align-content: center;
    width: 300px;
    padding: 20px 20px 40px 20px;
    border-radius: 20px;
    box-shadow: 2px 10px 30px rgba(0, 0, 0, 0.1);
    background-color: white;
    margin-bottom: 20px;
}

.titolo{
  
    padding-top: 5px;
    font-size: 1.3rem;
    font-weight: 700;
    text-align: center;
}

.paragrafo{
    margin-top: 10px;
  
    padding-top: 5px;
    font-size: 1rem;
    font-weight: 400;
    text-align: center;
    color: #7b879d;
}

.finale{
    font-size: 11px;
    text-align: center;
    
}
</style>