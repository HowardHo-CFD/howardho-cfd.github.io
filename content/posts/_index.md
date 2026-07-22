<style>
  /* Hide Blowfish default page title header */
  header h1, header .text-3xl, header .text-4xl, .article-title {
    display: none !important;
  }

  /* 1. MAKE BACKGROUND OBVIOUS (Very light overlay) */
  body {
    background-image: linear-gradient(180deg, rgba(0, 0, 0, 0.15) 0%, rgba(15, 23, 42, 0.5) 100%), 
                      url('/img/backgrounds/fluids-bg-cropped.jpg') !important;
    background-size: cover !important;
    background-position: center !important;
    background-attachment: fixed !important;
  }

  /* Ensure navbar text remains white and readable */
  header a, nav a {
    color: #ffffff !important;
    text-shadow: 0 2px 4px rgba(0, 0, 0, 0.8) !important;
  }

  /* 2. POST BOXES — solid enough to read, still feels "glass" */
  article, .article, .card {
    /* Higher alpha (0.82) so the busy background doesn't fight the text */
    background-color: rgba(15, 23, 42, 0.82) !important; 
    
    /* Backdrop blur ensures text remains readable even with low opacity */
    backdrop-filter: blur(12px) !important; 
    -webkit-backdrop-filter: blur(12px) !important;
    
    padding: 1.25rem !important;
    border-radius: 10px !important;
    border: 1px solid rgba(255, 255, 255, 0.12) !important;
    margin-bottom: 1.5rem !important;
    transition: background-color 0.2s ease, transform 0.2s ease !important;
  }

  /* Subtle highlight on hover */
  article:hover, .article:hover, .card:hover {
    background-color: rgba(15, 23, 42, 0.9) !important;
    transform: translateY(-2px) !important;
  }

  /* Strong text shadow so white text pops against bright areas of the background image */
  article h2, article h3, article a {
    color: #ffffff !important;
    text-shadow: 0 2px 4px rgba(0, 0, 0, 0.8) !important;
  }

  article p, article div, article span {
    color: #f8fafc !important;
    text-shadow: 0 1px 3px rgba(0, 0, 0, 0.7) !important;
  }
</style>

