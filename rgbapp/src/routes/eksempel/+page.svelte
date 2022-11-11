<script>
    import { Toggle, Tile } from "carbon-components-svelte";

    function sendToggle()
    {
        const data = fetch('https://maker.ifttt.com/trigger/toggle/json/with/key/l8im8Let_5mQNHHGcHUv-jKMAb-sFb4eQfbc1DPEiLj', {
            method: "GET",
            mode: "no-cors"
        });
    }
</script>

<svelte:head><link rel="stylesheet" href="https://unpkg.com/carbon-components-svelte@0.30.0/css/g10.css" /></svelte:head>

<Tile class="tile">
    <Toggle labelText="Skru lampe på og av" labelA="" labelB="" on:toggle={sendToggle} />
</Tile>