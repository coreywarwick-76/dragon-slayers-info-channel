# dragon-slayers-info-channel
Dragon Slayers web
index.html<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Dragon Slayers Info Channel</title>
<link rel="stylesheet" href="style.css">
</head>
<body>

<header class="hero">
    <div class="overlay">
        <h1>DRAGON SLAYERS INFO CHANNEL</h1>
        <p>Research • Media • Community • Archives</p>

        <input type="text" id="searchInput"
        placeholder="Search information..."
        onkeyup="searchContent()">
    </div>
</header>

<section id="latest">
    <h2>Latest Updates</h2>
    <div class="card searchable">
        Featured articles and updates from our community.
    </div>
</section>

<section id="research">
    <h2>Research Vault</h2>
    <div class="card searchable">
        Research documents, reports and archived information.
    </div>
</section>

<section id="videos">
    <h2>Video Library</h2>
    <div class="card searchable">
        Video resources and educational content.
    </div>
</section>

<section id="downloads">
    <h2>Downloads</h2>
    <div class="card searchable">
        Downloadable files and resources.
    </div>
</section>

<section id="community">
    <h2>Community</h2>
    <div class="card">
        <a href="https://www.facebook.com/" target="_blank">
            Visit Community
        </a>
    </div>
</section>

<footer>
    <p>Dragon Slayers Info Channel © 2025</p>
</footer>

<script>
function searchContent() {
    let input =
    document.getElementById('searchInput').value.toLowerCase();

    let items =
    document.getElementsByClassName('searchable');

    for(let i=0;i<items.length;i++){
        let text =
        items[i].innerText.toLowerCase();

        items[i].style.display =
        text.includes(input) ? "block" : "none";
    }
}
</script>

</body>
</html>
style.cssbody{
    margin:0;
    background:#111;
    color:#eee;
    font-family:Arial,sans-serif;
}

.hero{
    height:80vh;
    background:url('banner.jpg') center center/cover;
    display:flex;
    justify-content:center;
    align-items:center;
}

.overlay{
    text-align:center;
    background:rgba(0,0,0,0.6);
    padding:30px;
    border-radius:12px;
}

h1{
    color:#D4AF37;
    font-size:3rem;
}

h2{
    color:#D4AF37;
}

section{
    padding:40px;
}

.card{
    background:#222;
    padding:20px;
    border-left:4px solid #8B0000;
    margin-top:15px;
    border-radius:10px;
}

input{
    width:300px;
    max-width:90%;
    padding:12px;
    margin-top:20px;
}

footer{
    text-align:center;
    padding:20px;
    background:#000;
}
banner.jpg
