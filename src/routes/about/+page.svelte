<svelte:head>
    <title>About | in.decoded</title>
</svelte:head>

<div class="about-page">
    <nav class="top-nav">
        <div class="nav-left">
            <a href="/" class="logo">in.decoded</a>
        </div>
        <div class="nav-right">
            <a href="/about">About</a>
            <a href="/contact">Contact</a>
        </div>
    </nav>

    <main class="about-content-wrapper">
        <header class="about-header">
            <span class="sub-label">About the Project</span>
            <h1>in.decoded</h1>
            <p class="tagline">Decoding India, One Dataset at a Time.</p>
        </header>

        <section class="about-section text-center">
            <p class="lead">
                Making public data visual, interpretable, and citizen-centric.
            </p>
            <p>
                India's public institutions produce an immense volume of data—through censuses, budgets, elections, and administrative records. Yet, much of this remains locked behind dense, complex formats.
            </p>
            <p>
                Through visual storytelling, design, cartography, and interactive tools, we translate these datasets into intuitive experiences. We treat data as an artifact to be explored, revealing hidden histories, systems, and connections to help us better understand the country we inhabit.
            </p>
        </section>

        <hr class="separator" />

        <section class="about-section text-center">
            <h2>Proudly Independent</h2>
            <p>
                We are self-funded and completely independent. We believe that critical topics like policy, geography, elections, and economics don't have to be dry. We hope our stories and tools feel like a friend sharing their latest visual obsession, making complex systems accessible and engaging for everyone.
            </p>
        </section>

        <div class="actions">
            <a href="/" class="btn back-btn">← Back to Stories</a>
        </div>
    </main>
</div>

<style>
    .about-page {
        min-height: 100vh;
        background-color: #fcfbf8;
        padding-top: 120px;
        color: #3e2723;
        font-family: "Inter", sans-serif;
    }

    /* --- NAVBAR --- */
    .top-nav {
        position: fixed;
        top: 1.5rem;
        left: 50%;
        transform: translateX(-50%);
        width: calc(100% - 3rem);
        max-width: 1200px;
        box-sizing: border-box;
        z-index: 50;
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 1rem 2.5rem;
        background: rgba(255, 255, 255, 0.4);
        backdrop-filter: blur(24px);
        -webkit-backdrop-filter: blur(24px);
        border-radius: 100px;
        box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.07);
        border: none;
    }

    .nav-left .logo {
        font-family: "Inter", sans-serif;
        font-weight: 700;
        font-size: 1.5rem;
        letter-spacing: -0.04em;
        color: #3e2723;
        text-decoration: none;
    }

    .nav-right {
        display: flex;
        gap: 3rem;
        align-items: center;
    }

    .nav-right a {
        color: rgba(62, 39, 35, 0.7);
        text-decoration: none;
        font-size: 0.9rem;
        font-weight: 500;
        transition: color 0.3s ease;
    }

    .nav-right a:hover {
        color: #3e2723;
    }

    /* --- CONTENT LAYOUT --- */
    .about-content-wrapper {
        max-width: 760px;
        margin: 0 auto;
        padding: 3rem 2rem 6rem 2rem;
        box-sizing: border-box;
    }

    .about-header {
        text-align: center;
        margin-bottom: 4rem;
    }

    .sub-label {
        font-size: 0.85rem;
        text-transform: uppercase;
        letter-spacing: 0.05em;
        color: rgba(93, 64, 55, 0.7);
        font-weight: 500;
    }

    h1 {
        font-family: "Instrument Serif", serif;
        font-size: 5rem;
        font-weight: 400;
        line-height: 1;
        margin: 0.5rem 0 1rem 0;
        letter-spacing: -0.02em;
    }

    .tagline {
        font-family: "Instrument Serif", serif;
        font-style: italic;
        font-size: 1.8rem;
        color: #5d4037;
        margin: 0;
    }

    .about-section {
        margin-bottom: 3.5rem;
    }

    .text-center {
        text-align: center;
    }

    h2 {
        font-family: "Instrument Serif", serif;
        font-size: 2.8rem;
        font-weight: 400;
        color: #3e2723;
        margin-top: 0;
        margin-bottom: 1.5rem;
        letter-spacing: -0.01em;
    }

    p {
        font-size: 1.125rem;
        font-weight: 300;
        line-height: 1.75;
        color: #5d4037;
        margin: 0 auto 1.5rem auto;
        max-width: 680px;
        text-align: center;
    }

    .lead {
        font-size: 1.25rem;
        line-height: 1.8;
        color: #3e2723;
        text-align: center;
    }

    .separator {
        border: none;
        border-top: 1px solid rgba(62, 39, 35, 0.1);
        margin: 3.5rem 0;
    }

    /* --- ACTIONS --- */
    .actions {
        text-align: center;
        margin-top: 4rem;
    }

    .btn {
        display: inline-flex;
        align-items: center;
        justify-content: center;
        font-family: "Inter", sans-serif;
        font-size: 0.95rem;
        font-weight: 500;
        text-decoration: none;
        color: #ffffff;
        background-color: #3e2723;
        padding: 0.75rem 1.5rem;
        border-radius: 100px;
        transition: all 0.3s ease;
        border: none;
    }

    .btn:hover {
        background-color: #2b1a17;
        transform: translateY(-2px);
        box-shadow: 0 4px 12px rgba(62, 39, 35, 0.2);
    }

    /* Responsive */
    @media (max-width: 768px) {
        .about-page {
            padding-top: 140px;
        }

        .top-nav {
            flex-direction: column;
            align-items: flex-start;
            gap: 1.5rem;
            padding: 2rem;
        }

        h1 {
            font-size: 3.5rem;
        }

        .tagline {
            font-size: 1.4rem;
        }

        h2 {
            font-size: 2.2rem;
        }

        p {
            font-size: 1.05rem;
        }

        .lead {
            font-size: 1.15rem;
        }

        .about-content-wrapper {
            padding: 1rem 1.5rem 4rem 1.5rem;
        }
    }
</style>
