<script>
import star from '../assets/Star.svg'
import search from '../assets/Frame.svg'
import reviews from "../data/reviews.json"
import Starsystem from '../components/Starsystem.svelte'

const total = reviews.length;
const stars = [1,2,3,4,5];

</script>
<div class="card">
    <header>
        <h2>What others think about the product {total}</h2>
        <div class="summary">
            <div>
                <img src="{star}" alt="star" />
                <span>4.8</span>
            </div>
            <p>Average customer rating</p>
        </div>
    </header>

    <form class='search'>
        <input type="search" 
               name="review-search"
               id="review-search"
               placeholder="Search topics and reviews"/>
        <button type="submit">
            <img src={search} aria-label="run search">
        </button>
    </form>
    <div class="flex-container-stars">
        <p class="reviews-title">Reviews</p>

        <Starsystem voto=5 punteggio=106 larghezza_giallo=329/>
        <Starsystem voto=4 punteggio=32 larghezza_giallo=127/>
        <Starsystem voto=3 punteggio=0 />
        <Starsystem voto=2 punteggio=0 />
        <Starsystem voto=1 punteggio=0 />
    </div>

<button type="button" class='btn'>Write a review</button>
 </div>


<style>



*,
*::before,
*::after {
    box-sizing: border-box;
    margin:0;
    padding: 0;
    
   
}

:root { 
    /* colors */
    --dark: 238 49% 19%;
    --muted: 239 17% 53%;
    --accent: 43 100% 71%;
    --accent--muted: 36 83% 63%; 
    --neutral1: 0 0% 100%;
    --neutral2: 0 0% 97%;
    --neutral3: 0 0% 93%;
    --neutral4: 0 0% 79%;
    --neutral5: 0 0% 90%;
       /* fonts */
    --font-heading: 'Merriweather', serif;
    --font-body: 'Poppins',sans-serif;

}

:global(body){
    font-family: var(--font-body);
    background-color: hsl(var(--neutral4));
    color: hsl(var(--dark));
    display: grid;
    place-items: center;
    min-height: 100vh;
    font-size: 16px;
    line-height: 24px;
    padding: 80px;
}

ul {
    list-style-type: none;
}

.card {
    background-color: hsl(var(--neutral2));
    display: grid;
    padding: 84px;
    gap: 56px;
    max-width: 703px;
    box-shadow: 0px 12px 92px hsl(var(--dark) / 0.1);
    border-radius: 23px;
    position: relative;
}


.card::before{
    content: "";
    position: absolute;
    left: -67px;
    top: -64px;
    background-color: hsl(var(--neutral1));
    width: 100%;
    height: 100%;
    z-index: -1;
    border-radius: 23px;
}

header{
    display: flex;
    flex-wrap: wrap;
    gap:80px;
}

header h2{
    flex: 1 1 0%;
    font-family: var(--font-heading);
    font-size: 34px;
    font-weight: 900;
    line-height: 43px;
    max-width: 13ch;
}

.summary{
    flex: 1 1 0%;
    max-width: 18ch;
    text-align: center;
    display: grid;
    place-items: center;
    padding: 17px;
    gap: 8px;
    background: hsl(var(--neutral1));
    border: 3px solid hsl(var(--neutral1));
    box-shadow: 0px 7px 20px hsl(var(--neutral1));
    border-radius: 15px;
}

.summary div {
    display: flex;
    align-items: center;
    gap: 8px;
}

.summary div span {
    
    font-size: 26px;
    font-weight: 600;
    line-height: 39px;

}

.summary p {
  
    font-size: 14px;
    line-height: 21px;
}

.search {
  display: flex;
  align-items: center;
  background-color: hsl(var(--neutral1));
  padding: 16px;
  gap: 10px;
  border-radius: 26px;
}

.search [type="search"] {
  width: 100%;
  font: inherit;
  border: none;
  padding: 5px 5px 3px;
  border-bottom: 2px solid hsl(var(--neutral1));
  transition: border-color 0.2s cubic-bezier(0.075, 0.82, 0.165, 1);
}

.search [type="search"]:focus {
  outline: transparent;
  border-color: hsl(var(--muted));
}

.search [type="search"]::placeholder {
  color: hsl(var(--muted));
}

.search [type="submit"] {
  order: -1;
  background-color: transparent;
  border: none;
  cursor: pointer;
  display: grid;
  place-items: center;
  border-radius: 5px;
  transition: transform 0.2s cubic-bezier(0.075, 0.82, 0.165, 1), box-shadow 0.2s cubic-bezier(0.075, 0.82, 0.165, 1);
}

.search [type="submit"]:hover {
  transform: scale(1.1);
}

.search [type="submit"]:focus {
  outline: transparent;
}

.search [type="submit"]:focus-visible {
  box-shadow: 0 0 0 2px hsl(var(--neutral1)), 0 0 0 5px hsl(var(--muted));
}

.flex-container-stars {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    gap: 18px;
    margin-top: -20px;
}
.reviews-title{
    
    
    font-family: var(--font-body);
    font-size: 16px;
    font-weight: 600;
    gap: 16px;
}

.btn {
    
    padding: 16px 24px;
    font: inherit;
    border:none;
    max-width: fit-content;

    cursor: pointer;
    background: hsl(var(--dark));
    color:hsl(var(--neutral1));
    border-radius: 34px;
    transition: box-shadow 0.2s cubic-bezier(0.075, 0.82, 0.165, 1);
}

.btn:focus {
    outline: transparent;
}

.btn:where(:hover, :focus-visible) {
    box-shadow: 0 0 0 4px hsl(var(--neutral1)), 0 0 0 8px hsl(var(--dark));
}




</style>