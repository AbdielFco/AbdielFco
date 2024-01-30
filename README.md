<!-- SVG con CSS y HTML para el README de GitHub -->
<div xmlns="http://www.w3.org/1999/xhtml" class="container">
    <!-- Contenido HTML del banner -->
    <h1>GitHub README with CSS</h1>
    <p>Add CSS to your GitHub READMEs</p>
</div>

<!-- CSS para el diseño del banner -->
<style>
    .container {
        width: 800px;
        height: 400px;
        background-color: #f0f0f0;
        display: flex;
        justify-content: center;
        align-items: center;
        font-family: Arial, sans-serif;
        border: 2px solid #ccc;
        box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    }

    h1 {
        color: #333;
        font-size: 36px;
    }

    p {
        color: #666;
        font-size: 18px;
        text-align: center;
    }
</style>



<svg fill="none" viewBox="0 0 800 400" width="800" height="400" xmlns="http://www.w3.org/2000/svg">
  <foreignObject width="100%" height="100%">
    <div xmlns="http://www.w3.org/1999/xhtml">
      <h3>klk </h3>
      <style>
        h3 {
            font-size: 100px; 
        }
      </style>

      <!-- your HTML -->

    </div>
  </foreignObject>
</svg>





<!-- Instrucciones adicionales para el README -->
<h2>Setting it up</h2>
<p>In your repository, add a new SVG file with whatever name you like, such as header.svg.</p>
<p>Then, embed the image in your README using some plain ol' HTML:</p>
<pre>&lt;img src="header.svg" width="800" height="400"&gt;</pre>
<h2>How does this work?</h2>
<p>According to the repo, you can put HTML (actually XHTML) and CSS inside a &lt;foreignObject&gt; tag inside a SVG file inside an &lt;img&gt; tag inside your readme.</p>
<p>...</p>
<h2>What about JavaScript?</h2>
<p>GitHub has very specific content loading policies on their servers, and when loading any type of asset the server first sanitizes the data to ensure no foreign JavaScript executes in the browser.</p>
<p>...</p>
