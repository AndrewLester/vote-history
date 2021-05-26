<script lang="ts">
export let value: string | number = '';

function isNumber(val: typeof value): val is number {
    return typeof val === 'number';
}
</script>

<input type="text" inputmode={isNumber(value) ? 'numeric' : 'latin'} bind:value>

<style>
input {
    box-sizing: border-box;
    height: calc(var(--content-font-size) * 2.5);
    font-size: var(--content-font-size);
    border: 2px solid var(--prussian-blue);
    border-radius: 5px;
    padding: 5px 10px;
}

input[inputmode="numeric"] {
    width: 100px;
}

input::placeholder {
    color: rgba(0, 0, 0, 0.60);
}

input:focus {
    border-radius: 5px;
    border-color: hsl(210, 70%, 50%);
    outline: none;
}

input:invalid {
    border-color: var(--maximum-red);
}
</style>
