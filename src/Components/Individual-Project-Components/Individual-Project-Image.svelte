<script>
export let currentPage

let pics = [];

if (currentPage === '/front-end') {
    pics = [{
        title: "Home Page",
        src: "Images/fun-review.png",
        alt: "Funbelievable Reviews"
    }]
} else if (currentPage === '/group-project') {
    pics = [{
        title: "Login Page",
        src: "Images/RMAS/RMAS-Login.png",
        alt: "Read Me A Story - Login"
    }, {
        title: "Register Page",
        src: "Images/RMAS/RMAS-Register.png",
        alt: 'Read Me A Story - Register'
    }, {
        title: "Home Page",
        src: "Images/RMAS/RMAS-Home.png",
        alt: 'Read Me A Story - Home'
    }, {
        title: "The Recording Page",
        src: "Images/RMAS/RMAS-Record.png",
        alt: 'Read Me A Story - Record'
    }, {
        title: "The Bookshelf Page",
        src: "Images/RMAS/RMAS-Bookshelf.png",
        alt: 'Read Me A Story - Bookshelf'
    }, {
        title: "Logout Page",
        src: "Images/RMAS/RMAS-Logout.png",
        alt: 'Read Me A Story - Logout'
    }]
}
</script>
<ul class="image-list">
    {#each pics as {title,src,alt}}
    <li>
        <h3 class="image-title">{title}</h3>
        <img src={src} alt={alt}>
    </li>
    {/each}
</ul>

<style>
img {
    border: solid black 1px;
    display: block;
    margin: auto;
    margin-bottom: 2rem;
    width: 60%
}

li {
    width: 30%;
    list-style: none;
}

.image-list {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
}

.image-title {
    font-size: 24px;
    text-align: center;
    text-decoration: underline 2px aqua;
}
</style>
