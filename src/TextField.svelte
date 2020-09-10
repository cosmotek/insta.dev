<script>
    export let label = null;
    export let placeholder = "";
</script>

<div id="textfield">
    {#if label !== null }
        <h3 id="label">{ label }</h3>
    {/if}

    <input type="text" placeholder={placeholder}/>
</div>

<style type="text/scss">
    @import "./colors.scss";

    #textfield {
        flex-direction: column;
        justify-content: left;
        align-items: left;
        display: flex;
    }

    input {
        font-family: 'Gilroy', sans-serif;
        font-weight: 500;
        font-size: 16px;

        border: 1px solid black;
        border-radius: 5px;
    }

    input:focus {
        border: 2px solid $th-primary;
    }

    #label {
        font-family: 'Gilroy', sans-serif;
        font-size: 16px;
        text-align: left;
        margin: 0 0 8px 0;
    }
</style>