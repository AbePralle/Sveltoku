<script>
  let one_to_nine = [1,2,3,4,5,6,7,8,9];
</script>

<table class="SudokuGrid">
  {#each one_to_nine as row}
    <tr>
    {#each one_to_nine as column}
      <td></td>
    {/each}
    </tr>
  {/each}
</table>

<style>
  table.SudokuGrid
  {
    font-size:24pt;
    text-align:center;
    color:black;
    border:1pt black solid;
    width:324pt;
    height:324pt;
    padding:0;
    margin:0;
    background-color:white;
    border-collapse:collapse;
  }

  table.SudokuGrid tr td
  {
    width:36pt;
    height:36pt;
    border:1pt black solid;
    background-color:white;
    padding:0;
    margin:0;
  }

  table.SudokuGrid tr td:nth-child(3), table.SudokuGrid tr td:nth-child(6)
  {
    border-right:3pt black solid;
  }

  table.SudokuGrid tr:nth-child(3), table.SudokuGrid tr:nth-child(6)
  {
    border-bottom:3pt black solid;
  }
</style>
