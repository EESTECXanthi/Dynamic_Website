<script>
  import clock from "../../assets/clock.svg";
</script>

<div class="grid">
  <img alt="Clock" src={clock} />
  <div class="slider">Hello</div>
  <div class="welcome">Welcome to LC Xanthi!</div>
</div>

<style>
  .grid {
    display: grid;
    justify-content: center;
  }
  img {
    grid-row-start: 1;
    grid-row-end: 3;
    grid-column: 1;
    width: 100px;
  }
  .slider {
    background: red;
    width: 500px;
    min-width: 500px;

    min-height: 100px;
    grid-row-start: 1;
    grid-row-end: 2;
    grid-column-start: 2;
    grid-column-end: 3;
  }
  .welcome {
    padding-left: 100px;
    font-size: xx-large;
    padding-top: 300px;
    grid-row: 3;
    grid-column-start: 2;
    grid-column-end: 3;
  }
</style>
