<script>


</script>


<!-- SECONDO PEZZO -->
<div class="secondo-container">

    <div class="griglia-1">
        <h1>Transform your brand</h1>
        <p>We are a full-service creative agency specializing in helping brands grow fast. Engage your clients through compelling visuals that do most of the marketing for you.</p>
        <a href="#">LEARN MORE</a>
    </div>
    <div class="griglia-2" />
    <div class="griglia-3" />
    <div class="griglia-4">
        <h1>Stand out to the right audience</h1>
        <p>Using a collaborative formula of designers, researchers, photographers, videographers, and copywriters, we’ll build and extend your brand in digital places.</p>
        <a href="#">LEARN MORE</a>
    </div>
    <div class="griglia-5">
        <h1>Graphic Design</h1>
        <p>Great design makes you memorable. We deliver artwork that underscores your brand message and captures potential clients’ attention</p>
    </div>
    <div class="griglia-6">
        <h1>Photography</h1>
        <p>Increase your credibility by getting the most stunning, high-quality photos that improve your business image.</p>
    </div>
</div>


<style>

.secondo-container{
    display: grid;
    height:  180vh;
    grid-template-areas: 
    'one two'
    'three four'
    'five six';
}

.griglia-1{
    grid-area: one;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  
}

.griglia-1 h1 {
    color: var(--very-dark-desaturated-blue);
    font-family: var(--frauces-font);
    font-size: 2.4rem;
    font-weight: 900;
    word-spacing: -1px;
    letter-spacing: -2px;
}

.griglia-1 p {
    color: var(--dark-grayish-blue);
    font-family: var(--frauces-font);
    line-height: 30px;
    padding-top: 1.5rem;
    max-width: 25ch;
}


.griglia-2{
    grid-area: two;
    background-image: url("../assets/images/desktop/image-transform.jpg");
    background-size: cover;
    background-position: center;
    min-width: 50%;
    height: 100%;

}

.griglia-3{
    grid-area: three;
    background-image: url('../assets/images/desktop/image-stand-out.jpg');
    background-size: cover;
    background-position: center;
    min-width: 50%;
    height: 100%;
}
.griglia-4{
    grid-area: four;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

.griglia-4 h1{
    color: black;
}


.griglia-5{
    grid-area: five;
    background-image: url('../assets/images/desktop/image-graphic-design.jpg');
    background-size: 175%;
    background-position: center;
    min-width: 50%;
    height: 100%;
    text-align: center;
    
}

.griglia-6{
    grid-area: six;
    background-image: url('../assets/images/desktop/image-photography.jpg');
    background-size: 175%;
    background-position: center;
    min-width: 50%;
    height: 100%;
    text-align: center;
}

</style>