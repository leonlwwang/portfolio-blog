<script>
    export let src = null;
</script>

<div id="main-box">
    <div class="box-child">
        <figure>
            <img id="portrait" {src} alt="me-voronoi"/>
        </figure>
        {#if src != null}
            <div style="width: 50%;">
                <a id="reference" href="https://www.mattkeeter.com/projects/swingline/" target="_blank" rel="noreferrer">
                    <span id="caption" style="margin-top: -1rem; margin-left: 2.5rem; display: block; text-align: left; font-size: 0.6rem;">
                        weighted voronoi stippling
                    </span>
                </a>
            </div>
        {/if}
    </div>
    <div id="about-text" style="width: 50%;">
        <div id="pad" style="padding: 5rem;">
            <h2> I'm a junior studying Statistics & Computer Science at UIUC. </h2>
            <h4> 
                I currently work as a web developer intern at the Daily Illini.
                This summer, I'll be working at United Airlines as a Digital Technology intern!
            </h4>
            <p>
                I enjoy combining creativity with programming and designing elegant software solutions.
            </p>
            <p>
                I also produce and songwrite under Night High, my independent artist project.
            </p>
            <p>
                <span>Interested in more?</span>
                Check out my links below! 	
                &#9759;
            </p>
        </div>
    </div>
</div>

<style>
    #main-box {
        display: flex; 
        margin-top: 2rem; 
        justify-content: center;
    }
    .box-child {
        width: 50%;
    }
    figure {
        display: flex;
        justify-content: center;
    }
    #reference, #reference:visited {
        color: inherit;
        text-decoration: none;
    }
    #reference:hover {
        text-decoration: underline;
    }
    #portrait {
        border-left: 1px dashed; 
        border-bottom: 1px dashed; 
        width: 100%; 
        height: auto;
    }
    p {
        text-align: left;
    }
    #about-text {
        font-family: 'SF-Pro';
        display: flex;
        align-content: center;
    }
    @media screen and (max-width: 768px) {
        #portrait {
            border-left: 1px dotted !important; 
            border-bottom: 1px dotted !important; 
        }
        #about-text {
            width: 85% !important;
            padding: 1.5rem;
        }
        #main-box {
            display: block;
            margin-top: 4rem !important;
        }
        .box-child {
            width: 100%;
        }
        #reference:hover {
            text-decoration: none;
        }
        #caption {
            font-size: 0.35rem !important;
        }
        #pad {
            padding: 0rem !important;
        }
        p {
            font-size: 0.8rem;
            text-align: left !important;
            padding: 0rem !important;
        }
	}
</style>