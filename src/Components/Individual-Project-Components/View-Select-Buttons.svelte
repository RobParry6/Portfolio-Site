<script>
import {showDescription} from "../../stores/Individual-Project-Store"
</script>

<div class="ButtonSelector">
    <button type="button" class={$showDescription ? "block & left" : "block & left & unselected"} on:click={()=>{$showDescription=true}}>Description</button>
    <button type="button" class={!$showDescription ? "block & right" : "block & right & unselected"} on:click={()=>{$showDescription=false}}>App View</button></div>

<style>
.ButtonSelector {
    display: flex;
    justify-content: center;
    margin-bottom: 16px;
    text-align: center;
}

.block {
    display: block;
    border: none;
    background-color: black;
    color: aqua;
    padding: 11px 28px;
    font-size: 16px;
    cursor: pointer;
    text-align: center;
}

.left {
    border-radius: 2rem 0rem 0rem 2rem;
}

.right {
    border-radius: 0rem 2rem 2rem 0rem;
}

.unselected {
    background-color: lightslategray;
    color: black;
}
</style>
