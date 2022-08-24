<script>
import BackEndCard from "./BackEndCard.svelte";
import FrontEndCard from "./FrontEndCard.svelte";
import ReadMeAStoryCard from "./ReadMeAStoryCard.svelte";
</script>

<h1>Projects</h1>

<ul>
    <li><div class="leftListItem"><BackEndCard /></div></li>
    <li><div class="rightListItem"><FrontEndCard/></div></li>
        <li><ReadMeAStoryCard/></li>
            </ul>

<style>
h1 {
    background-color: aqua;
    margin: auto;
    margin-bottom: 1rem;
    padding: 1rem;
    text-align: center;
}

* {
    margin: 0px;
    padding: 0px;
}

ul {
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
    list-style-type: none;
    margin: auto;
    padding: 0px;
    width: 80%;
}

li {
    padding: 16px;
    width: 40%;
}

.leftListItem {
    padding-inline: 32px;
    border-right: solid black 2px;
}

.rightListItem {
    padding-inline: 32px;
    border-left: solid black 2px;
}
</style>
