<script>
import App from '../kanban.svelte';

  import Column from './Column.svelte'
  import {store} from '../stores/store.js'
import Board from './Board.svelte';
</script>

{#each $store as column (column.id)}
  <Column {column} />
{/each}

