<script>
let {
    heading,
    src,
    description = "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Facilis, magni.",
    
} = $props()
</script>

<div class="flow bg-white">
<img {src} alt="">
<h3>heading</h3>
<p>{description}</p>
<a href="">Read More &raquo;</a>
</div>

<style>
div {
    position: relative;
    padding: 2rem;
    border-radius: 1rem;
    font-size: 1.125rem;
}

img {
    max-width: 3.5rem;
    position: absolute;
    top: -1.5rem;
}

a {
display: inline-block;
font-weight: bold;
}


</style>