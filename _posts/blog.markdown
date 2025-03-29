---
title: "Plot in a Blog Post"
date: 2024-03-29
---

## My Blog Post with a Chart

<canvas id="postChart" width="400" height="200"></canvas>

<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
<script>
  document.addEventListener("DOMContentLoaded", function () {
    const ctx = document.getElementById('postChart').getContext('2d');

    new Chart(ctx, {
      type: 'bar',
      data: {
        labels: ['Jan', 'Feb', 'Mar', 'Apr'],
        datasets: [{
          label: 'Sales Data',
          data: [5, 10, 8, 12],
          backgroundColor: 'orange'
        }]
      }
    });
  });
</script>
