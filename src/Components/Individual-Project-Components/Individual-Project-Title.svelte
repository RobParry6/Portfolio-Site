<script>
export let currentPage;
let title;

currentPage === "/front-end" ? title = "Front End React Project" :
    currentPage === "/back-end" ? title = "Back End API Project" :
    currentPage === "/group-project" ? title = "Read Me A Story Project" :
    title = "Project does not exist"
</script>

<h1>{title}</h1>

<style>
h1 {
    background-color: aqua;
    margin: auto;
    margin-bottom: 1rem;
    padding: 1rem;
    text-align: center;
}
</style>
