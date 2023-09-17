<script>
import logo from '../assets/images/logo.svg'
import freccia from '../assets/images/icon-arrow-down.svg'
</script>

<!-- PRIMO PEZZO -->
<div class="top-content">
    <div class="flex-nav">
      <img src={logo} alt="">
        <div class="navlinks">
            <ul>
                <a href="#"><li>About</li></a>
                <a href="#"><li>Services</li></a>
                <a href="#"><li>Projects</li></a>
                <a href="#"><button>CONTACT</button></a>
            </ul>
        </div>
    </div>

    <h1>WE ARE CREATIVES</h1>

    <div class="freccia">
        <img src={freccia} />
    </div>
</div>

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

.top-content{
    background-image: url("../assets/images/desktop/image-header.jpg");
    background-size: cover;
    background-position: center;
    height: 44.5rem;
    
}

.flex-nav{
    display: flex;
    justify-content: space-between;
    padding: 2rem 2.2rem;
    max-width: 100%;
}

.div-navlinks{
    display: flex;
   
    
}

li{
display: inline;
padding: 2rem;
color: var(--white);
font-family: var(--barlow-font);
font-size: 18px;
}

a{ 
    text-decoration: none;
    cursor: pointer;
}

 button{
    font-weight: 900;
    border-width: 1px;
    font-size: 0.9rem;
    font-family: var(--frauces-font);
    padding: 0.9rem 1.5rem;
    border-radius: 25px;
    margin-right: 0.4rem;
    border: none;
}

 button:hover {
    
    transition: background-color 0.4s ease, color 0.3s ease;
    background-color: orange;
    color: white;

}


h1 {
    font-family: var(--frauces-font);
    text-align: center;
    font-size: 2.3rem;
    color: var(--white);
    padding: 4rem;
    font-weight: 900;
    letter-spacing: 0.6rem;
}

.freccia{
 margin-top: 25px;
 text-align: center;
}

.secondo-container{
    display: grid;
    grid-auto-columns: 1fr;
    gap: 1.5rem;
    grid-template-areas: 
    'one two'
    'three four'
    'five six';
}

.griglia-1{
    grid-area: one;
}

.griglia-1 h1 {
    color: black;
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
}

.griglia-4 h1{
    color: black;
}


.griglia-5{
    grid-area: five;
    background-image: url('../assets/images/desktop/image-graphic-design.jpg');
    background-size: cover;
    background-position: center;
    min-width: 50%;
    height: 100%;
}

.griglia-6{
    grid-area: six;
    background-image: url('../assets/images/desktop/image-photography.jpg');
    background-size: cover;
    background-position: center;
    min-width: 50%;
    height: 100%;
}
</style>