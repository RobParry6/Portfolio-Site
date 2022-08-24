<script>
import {
    onMount
} from 'svelte'
import {
    showDescription
} from "../stores/Individual-Project-Store"
import Header from "../Components/Common-Components/Header.svelte";
import IndividualProject from "../Components/Individual-Project-Components/IndividualProject.svelte";

onMount(() => {
    $showDescription = true
})
</script>

<Header/>
    <IndividualProject/>
