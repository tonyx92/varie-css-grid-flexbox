<script>
import emily from '../assets/images/image-emily.jpg'
import thomas from'../assets/images/image-thomas.jpg'
import jennie from'../assets/images/image-jennie.jpg'

</script>

<div class="terzo-container">

    <div class="testimonials-titolo">
        <h1>client Testimonials</h1>
    </div>
    <div class="griglia-7">
        <img src={emily} alt="">
        <p>We put our trust in Sunnyside and they delivered, making sure our needs were met and deadlines were always hit.</p>
        <h1>Emily R.</h1>
       <p>Marketing Director</p>
    </div>

    <div class="griglia-8">
        <img src={thomas} alt="">
        <p>We put our trust in Sunnyside and they delivered, making sure our needs were met and deadlines were always hit.</p>
        <h1>Emily R.</h1>
       <p>Marketing Director</p>
    </div>

    <div class="griglia-9">
        <img src={jennie} alt="">
        <p>We put our trust in Sunnyside and they delivered, making sure our needs were met and deadlines were always hit.</p>
        <h1>Emily R.</h1>
       <p>Marketing Director</p>

    </div>

</div>



<style>
    .terzo-container{
    display: grid;
    height:  180vh;
    grid-template-areas: 
    'one two three';
}

.griglia-7{
    grid-area: one;
}

.griglia-8{
    grid-area: two;
}
.griglia-9{
    grid-area: three;
}
</style>
