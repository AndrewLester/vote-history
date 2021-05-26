<button on:click>
    <slot />
</button>

<style>
button {
    display: flex;
    flex-flow: no nowrap;
    align-items: center;
    color: white;
    -webkit-tap-highlight-color: transparent;
    background: var(--prussian-blue);
    border: none;
    border-radius: 5px;
    padding: 5px 20px;
    cursor: pointer;
    font-size: 15px;
    height: 40px;
    margin-top: 15px;
    box-shadow: 0px 0px 4px 1px rgba(0, 0, 0, 0.3);
    transition: all 250ms ease;
}

button:hover,
button:focus {
    background-color: hsl(201, 100%, 24%);
    box-shadow: 0px 0px 8px 2px rgba(0, 0, 0, 0.3);
    outline: none;
    -webkit-tap-highlight-color: transparent;
}

button:active {
    box-shadow: 0px 0px 4px 1px rgba(0, 0, 0, 0.3);
    background-color: var(--prussian-blue);
}
</style>
