<script>
import './/css/styles.css';
import logo from '../assets/logo.svg'
import illustration from '../assets/illustration-intro.svg'
import icon_hamburger from '../assets/icon-hamburger.svg'
import icon_close from '../assets/icon-close.svg'
import  main from '../routes/javascript/main.js'
import { onMount } from 'svelte';


onMount(() => {
    main();
})






</script>
<body>
    <header class="primary-header">
        <div class="container">
            <div class="nav-wrapper">
            <a href="#"><img src={logo} alt="Manage"></a>
                <button class="mobile-nav-toggle" aria-controls="primary-navigation" aria-expanded="false">
                    <img class="icon_hamburger" src={icon_hamburger} alt="" aria-hidden="true">
                    <img class="icon_close" src={icon_close} alt="" aria-hidden="true">
                    <span class="visually-hidden">Menu</span>
                </button>
                <nav class="primary-navigation" id="primary-navigation">
                    <ul aria-label="primary" role="list" class="nav-list">
                        <li><a href="#">Pricing</a></li>
                        <li><a href="#">Product</a></li>
                        <li><a href="#">About Us</a></li>
                        <li><a href="#">Careers</a></li>
                        <li><a href="#">Community</a></li>
                    </ul>
                </nav>
                <button class="button | display-sm-none display-md-inline-flex">Get Started</button>
            </div>
        </div>
    </header>

    <main>
        <section class="padding-block-900">
            <div class="container">
                <div class="even-columns">
                    <div><h1 class="fs-primary-heading fw-bold"></h1>
                    <p>Manage makes it simple for software teams to plan day-to-day tasks while keeping the larger team goals in
                        view.</p>
                    <button class="button">Get Started</button>
                    </div>
                    <div>
                        <img src={illustration} alt="">
                    </div>
                </div>
            </div>
        </section>

        <section class="padding-block-900">
            <div class="container">
                <div class="even-columns">
                    <div>
                        <h2 class="fs-secondary-heading fw-bold">What’s different about Manage?</h2>
                        <p>Manage provides all the functionality your team needs, without the complexity. Our software is
                            tailor-made for modern
                            digital product teams.</p>
                    </div>
                    <div>
                        <ul class="numbered-items" role="list">
                            <li>
                                <h3 class="fs-600 fw-bold">Track company-wide progress</h3>
                                <p>See how your day-to-day tasks fit into the wider vision. Go from tracking progress at the milestone
                                    level all the way
                                    done to the smallest of details. Never lose sight of the bigger picture again.</p>
                            </li>
                            <li>
                                <h3 class="fs-600 fw-bold">Advanced built-in reports</h3>
                                <p>>Set internal delivery estimates and track progress toward company goals. Our customisable dashboard
                                    helps you build out
                                    the reports you need to keep key stakeholders informed.</p>
                            </li>
                            <li>
                                <h3 class="fs-600 fw-bold">Everything you need in one place</h3>
                                <p>Stop jumping from one service to another to communicate, store files, track tasks and share
                                    documents. Manage offers an
                                    all-in-one team productivity solution.</p>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </section>

        <section class="carousel | padding-block-700">
            <h2 class="fs-secondary-heading fw-bold">What they've said</h2>
            <!-- Carosello qua!  -->
            <button class="button">Get Started</button>
        </section>

        <section class="cta | padding-block-700 bg-accent-400 text-neutral-100">
            <div class="container">
                <div class="even-columns">
                    <div>
                        <p class="fs-secondary-heading fw-bold">Simplify how your team works today.</p>
                    </div>
                    <div>
                        <button class="button" data-type="inverted">Get Started</button>
                    </div>
                </div>
            </div>
        </section>
    </main>

    <footer class="padding-block-700 bg-neutral-900 text-neutral-100">
        <div class="container">
            <div class="even-columns">
                <div>
                    <a href="#"><img src={logo} alt="Manage"></a>
                    <ul role="list" aria-label="Social links">
                        <li><a aria-label="facebook" href="#"></a></li>
                        <li><a aria-label="youtube" href="#"></a></li>
                        <li><a aria-label="twitter" href="#"></a></li>
                        <li><a aria-label="pinterest" href="#"></a></li>
                        <li><a aria-label="instragram" href="#"></a></li>
                    </ul>
                </div>
                <div>
                    <nav class="footer-nav">
                      <ul aria-label="Footer" role="list">
                        <li><a href="#">Home</a></li>
                        <li><a href="#">Pricing</a></li>
                        <li><a href="#">Products</a></li>
                        <li><a href="#">About Us</a></li>
                        <li><a href="#">Careers</a></li>
                        <li><a href="#">Community</a></li>
                        <li><a href="#">Privacy Policy</a></li>
                      </ul>
                    </nav>
                </div>
                <div>
                    <form action="">
                        <input type="email">
                        <button class="button">Go</button>
                        <p>Copyright 2020. All Rights Reserved</p>
                      </form>
                </div>
            </div>
        </div>
    </footer>


    
</body>




<style>


</style>