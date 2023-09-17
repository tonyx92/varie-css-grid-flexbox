<script>
import qr from '../assets/image-qr-code.png'
</script>

<div class="card">
    <img src={qr} alt="" class="qr">
    <div class="titolo">
        <h1>Improve your front-end skills by building projects</h1>
    </div>
    <div class="paragrafo">
        <p>Scan the QR code to visit Frontend Mentor and take your coding skills to the next level</p>
    </div>
</div>

<style>

:root{

    /* colors */
    --sfondo: var(#d6e2f0)
    --bianco: var(#FFFFFF)

}

:global(body){
    background-color: var(--sfondo);
    display: grid;
    place-content: center;
    min-height: 90vh;
    width: 100%;
}

.qr {
    max-width: 260px;
    max-height: 260px;
   
}

.card{
    display: grid;
    align-content: center;
    width: 300px;
    padding: 20px 20px 40px 20px;
    border-radius: 20px;
    box-shadow: 2px 10px 30px rgba(0, 0, 0, 0.1);
}

</style>