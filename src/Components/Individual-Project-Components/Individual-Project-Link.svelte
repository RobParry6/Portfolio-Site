<script>
export let currentPage
</script>

{#if currentPage === "/front-end"}
<p class='Link'>A hosted version of Funbelievable Reviews can be found here: <a href="https://funbelievable-reviews.netlify.app/">Funbelievable Reviews</a></p>
{:else if currentPage === "/group-project"}
<p class='Link'>A hosted version of the Read Me A Story app can be found here: <a href="https://read-me-a-story.netlify.app/">Funbelievable Reviews</a></p>
{/if}

<style>
p {
    margin: auto;
    margin-bottom: 16px;
    width: 60%;
}

.Link {
    text-align: center;
}
</style>
