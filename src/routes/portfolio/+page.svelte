<script>
    let images = [
        { src: 'portfolio/appdev.jpg', alt: 'Appointment' },
        { src: 'portfolio/appdev2.jpg', alt: 'Appointment' },
        { src: 'portfolio/appdev3.jpg', alt: 'Appointment' },
        { src: 'portfolio/SEBBY.png', alt: 'Appointment' },
    ];

    let additionalImages = [
        { src: 'portfolio/assessment1.png', alt: 'Assessment' },
        { src: 'portfolio/assessment2.png', alt: 'Assessment' },
        { src: 'portfolio/assessment3.png', alt: 'Assessment' },
        { src: 'portfolio/assessment4.png', alt: 'Assessment' },
    ]
</script>

<style>
    .portfolio {
        display: flex;
        flex-wrap: wrap;
        gap: 16px; 
        padding: 20px; 
        background-color: #f0f0f0; 
        border-radius: 8px; 
    }
    .portfolio h1 {
        width: 100%; 
        text-align: center; 
        margin-bottom: 20px; 
    }
    .portfolio img {
        width: calc(50% - 8px); 
        height: auto; 
        max-height: 500px; 
        object-fit: contain; 
        border-radius: 8px; 
        border: 1px solid #5c83aa; 
        padding: 4px; 
        box-shadow: 2px 2px 5px rgba(0, 0, 0, 0.1); 
    }
    .section {
        margin-top: 40px; /* Space between sections */
    }
</style>

<div class="portfolio">
    <h1 class="text-3xl font-bold mb-4 text-center" style="color: #34495e;">Student Appointment System</h1>
    {#each images as image}
        <img src={image.src} alt={image.alt} />
    {/each}
</div>

<div class="portfolio section">
    <h1 class="text-3xl font-bold mb-4 text-center" style="color: #34495e;"> ImageGallery Assessment </h1>
    {#each additionalImages as image}
        <img src={image.src} alt={image.alt} />
    {/each}
</div>