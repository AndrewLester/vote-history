<script lang="ts">
export let value: string;
</script>

<select bind:value>
    <slot></slot>
</select>

<style>
select {
    height: calc(var(--content-font-size) * 2.5);
    font-size: var(--content-font-size);
    border: 2px solid var(--prussian-blue);
    border-radius: 5px;
    padding: 5px 10px;
}

select:focus {
    border-radius: 5px;
    border-color: hsl(210, 70%, 50%);
    outline: none;
}

select:invalid {
    border-color: var(--maximum-red);
}
</style>
