<script>
  import Covid19Stats from "../components/Covind19Stats.svelte";
  import Covid19Chart from "../components/Covid19Chart.svelte";
  import TableContainer from "../components/TableContainer.svelte";
</script>

<svelte:head>
  <title>Covid 19 Tracker App</title>
</svelte:head>

<div class="section header">
  <div class="container">
    <h1>Covid 19 Tracker App!</h1>
    <Covid19Stats />
    <Covid19Chart />
    <TableContainer />
  </div>
</div>
