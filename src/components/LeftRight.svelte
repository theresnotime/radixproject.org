<script>
    import Img from "./Img.svelte";
</script>

<main>
    <div class="left">
        <div>
            <h2 class="heading-title">Your project is our priority<span class="dot">.</span></h2>
            <p class="mono">The Radix Project is committed to providing free-of-charge need-based hosting on request for your FLOSS/open source endeavors. You can apply for our base plan, or contact us for more powerful solutions.</p>
        </div>
        <div class="img">
            <Img themed svg src="icons/star_icon"/>
        </div>
    </div>

    <div class="right">
        <div class="img">
            <Img themed svg src="icons/globe_icon"/>
        </div>
        <div>
            <h2 class="heading-title">Reliable infrastructure for a dedicated community<span class="dot">.</span></h2>
            <p class="mono">Sponsored by world-class hosting providers, we are equipped to deliver our partners with powerful hosting solutions to meet the needs of the open source community as effectively as possible.</p>
        </div>
    </div>

    <div class="left">
        <div>
            <h2 class="heading-title">Trust & safety first<span class="dot">.</span></h2>
            <p class="mono">
                We will never share confidential or sensitive information with third parties, so you can rest assured that your valuable project infrastructure is in trustworthy hands. Partners, sponsors, & information are treated with respect. The infrastructure we provide is entirely powered by open-source software, so you can see what's going on under the hood at any time.
            </p>
        </div>
        <div class="img">
            <Img svg themed src="icons/lock_icon"/>
        </div>
    </div>
</main>

<style>
    main {
        display: flex;
        flex-direction: column;
        align-items: center;
    }

    .left, .right {
        display: flex;
        flex-direction: row;
        width: 100%;
        margin: 50px 0;
        justify-content: center;
    }

    @media screen and (max-width: 600px) {
        .left, .right {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            align-items: center;
            margin: 20px 0;
        }

        .left {
            flex-direction: column-reverse;
        }

        .img {
            padding: 0 0 35px 0 !important;
        }
    }

    .img {
        width: 170px;
        height: 170px;
    }

    .left .img {
        padding-left: 50px;
    }

    .right .img {
        padding-right: 50px;
    }
</style>
