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



<style>
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


</style>