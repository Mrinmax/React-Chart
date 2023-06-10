# React-Chart

# Chart.js

Chart.js is a powerful and flexible JavaScript charting library that allows you to create interactive and customizable charts for your web applications. It provides a wide range of chart types, including line, bar, pie, doughnut, radar, polar area, and more.

![Chart.js Example](chart-example.png)

## Getting Started

To get started with Chart.js, follow these simple steps:

### Installation

You can install Chart.js using npm:

```shell
npm install chart.js

<h1>Alternatively, you can include the Chart.js library directly in your HTML file:</h1>

<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>

<h1>Usage</h1>
<p>To create a chart using Chart.js, you need to have a <canvas> element in your HTML file:</p>
<canvas id="myChart"></canvas>

<h1>Then, you can use JavaScript to retrieve the canvas element and create a new chart:</h1>

var ctx = document.getElementById('myChart').getContext('2d');
var myChart = new Chart(ctx, {
    type: 'bar',
    data: {
        labels: ['Red', 'Blue', 'Yellow', 'Green', 'Purple', 'Orange'],
        datasets: [{
            label: '# of Votes',
            data: [12, 19, 3, 5, 2, 3],
            backgroundColor: [
                'rgba(255, 99, 132, 0.2)',
                'rgba(54, 162, 235, 0.2)',
                'rgba(255, 206, 86, 0.2)',
                'rgba(75, 192, 192, 0.2)',
                'rgba(153, 102, 255, 0.2)',
                'rgba(255, 159, 64, 0.2)'
            ],
            borderColor: [
                'rgba(255, 99, 132, 1)',
                'rgba(54, 162, 235, 1)',
                'rgba(255, 206, 86, 1)',
                'rgba(75, 192, 192, 1)',
                'rgba(153, 102, 255, 1)',
                'rgba(255, 159, 64, 1)'
            ],
            borderWidth: 1
        }]
    },
    options: {
        scales: {
            y: {
                beginAtZero: true
            }
        }
    }
});
