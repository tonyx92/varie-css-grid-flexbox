<script>
import star from '../assets/Star.svg'
import reviews from "../data/reviews.json"

export let voto;
export let punteggio;
export let larghezza_giallo;
</script>




                    <div class="reviews">
                        <span>{voto}</span>
                        <div class="star">
                            <img src={star} alt="" class="star">
                        </div>
                        <div class="barra">
                        {#if larghezza_giallo>0}
                            <div class="inner-bar" style="width: {larghezza_giallo}px;"/>
                        {/if}
                            <div class="rectangle">

                            </div>
                        </div>
                        <span>{punteggio}</span>
                    </div>



<style>
    .reviews {
    display: flex;
    gap: 8px;
    align-items: center;
}



.rectangle{
    height: 10px;
    width: 426.355px;
    background-color: #EEE;
    border: 1px solid #C9C9C9;
    border-radius: 23px;
    gap: 4px;
}

.inner-bar{
   
    position: absolute;
    background: #FFD66C;
    height: 10px;
    border-radius: 23px;
    border: 1px solid #EFB153;
    border-radius: 13px;
}

.star{
    width: 25.4px;
height: 25.4px;
}
</style>