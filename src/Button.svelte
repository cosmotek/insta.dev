<script>
    export let text;
    export let onTap = () => {};
</script>

<div id="button" on:click={onTap}>
    <p>{text}</p>
</div>

<style lang="scss">
    @import "./colors.scss";

    #button {
        border-radius: 8px;
        padding: 2px;
        background-color: $th-primary;
        color: $th-txt-light;
        display: inline-block;
        padding: 16px 96px 16px 96px;

        p {
            padding: 0;
            margin: 0;

            font-family: "Gilroy";
        }
    }
</style>