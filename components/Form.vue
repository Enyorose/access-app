<template>
  <form>
    <label for="input-search">Restaurant Name:</label>
    <input type="text" id="input-search" placeholder="Search Restaurant" />
    <label for="input-range">Search Range:</label>
    <input
      type="range"
      max="400"
      min="100"
      step="50"
      id="input-range"
      placeholder="Search Range"
    /><button>Search</button>
  </form>
</template>