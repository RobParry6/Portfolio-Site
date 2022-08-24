<script>
import Desciption from './Desciption.svelte';
import IndividualProjectImage from './Individual-Project-Image.svelte';
import IndividualProjectLink from './Individual-Project-Link.svelte';
import IndividualProjectTitle from './Individual-Project-Title.svelte';
import ViewSelectButtons from './View-Select-Buttons.svelte';
import {
    page
} from '$app/stores';
import {
    showDescription
} from "../../stores/Individual-Project-Store"

const currentPage = $page.url.pathname
</script>

<IndividualProjectTitle currentPage={currentPage}/>
    {#if $showDescription}
    <Desciption currentPage={currentPage}/>
        {:else}
        <IndividualProjectImage currentPage={currentPage}/>
            <IndividualProjectLink currentPage={currentPage}/>
                {/if}

                {#if currentPage === "/front-end" || currentPage === "/group-project"}
                <ViewSelectButtons />
                {/if}
