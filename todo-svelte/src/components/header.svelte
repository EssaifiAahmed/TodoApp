<script>
    import {items} from "../stores";
    
    $: itemCount = $items.length;
    $: completedItemCount = $items.filter((item) => item.complete).length;
</script>

<style>
    .header{
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 15px 20px;
        color: #ffffff;
        font-weight: bold;
        font-size: 1.5em;
        background: #009579;    
    }
</style>

<dev class="header">
    <span>Dom's To-Do List</span>
    <span>{completedItemCount}/{itemCount}</span>
</dev>