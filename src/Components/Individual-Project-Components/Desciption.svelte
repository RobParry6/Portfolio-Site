<script>
import BackEndDescription from "./Project-Descriptions/Back-End-Description.svelte";
import FrontEndDescription from "./Project-Descriptions/Front-End-Description.svelte";
import GroupProjectDescription from "./Project-Descriptions/Group-Project-Description.svelte";

export let currentPage;
</script>

<section class="description">
    {#if currentPage === "/front-end"}
    <FrontEndDescription/>
        {:else if currentPage === "/back-end"}
        <BackEndDescription/>
            {:else if currentPage === "/group-project"}
            <GroupProjectDescription/>
                {/if}
                </section>
