<script>
import {
    page
} from '$app/stores';
const currentPage = $page.url.pathname
</script>

<div class="NavBar">
    <a href="/"><button type="button" class={currentPage==="/"? "block & currPage" :"block & notCurrPage"}>Home</button></a>
    <a href="/front-end"><button type="button" class={currentPage==="/front-end"? "block & currPage" :"block & notCurrPage"}>Front End Project</button></a>
    <a href="/back-end"><button type="button" class={currentPage==="/back-end"? "block & currPage" :"block & notCurrPage"}>Back End Project</button></a>
    <a href="/group-project"><button type="button" class={currentPage==="/group-project"? "block & currPage" :"block & notCurrPage"}>Read Me A Story Project</button></a>
</div>

<style>
a {
    text-decoration: none;
}

.NavBar {
    background-color: black;
    border: 1px black solid;
    display: flex;
    justify-content: space-around;
    justify-items: stretch;
    margin: 0px;
}

.block {
    display: block;
    border: none;
    background-color: black;
    color: aliceblue;
    padding: 14px 28px;
    font-size: 16px;
    cursor: pointer;
    text-align: center;
}

.currPage {
    display: inline-block;
    position: relative;
}
.currPage:after {
    content: "";
    position: absolute;
    width: 80%;
    height: 2px;
    bottom: 15px;
    left: 10%;
    background-color: aqua;
}

.notCurrPage {
    display: inline-block;
    position: relative;
}

.notCurrPage:after {
    content: "";
    position: absolute;
    width: 80%;
    transform: scaleX(0);
    height: 2px;
    bottom: 15px;
    left: 10%;
    background-color: aqua;
    transform-origin: center;
    transition: transform 0.25s ease-out;
}

.notCurrPage:hover:after,
.notCurrPage:focus:after {
    transform: scaleX(1);
    transform-origin: center;
}
</style>
