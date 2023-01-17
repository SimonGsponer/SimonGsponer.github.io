---
# the default layout is 'page'
icon: fas fa-info-circle
order: 1
---

> Add Markdown syntax content to file `_tabs/about.md`{: .filepath } and it will show up on this page.
{: .prompt-tip }


<html>
<script src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/3.9.1/chart.js"></script>
<body>
<canvas id="myChart" style="width:100%;max-width:700px"></canvas>
<p>Placeholder text</p>
<canvas id="myChart1" style="width:100%;max-width:600px"></canvas>
<p>Placeholder text redux</p>
<canvas id="pieChart" style="width:100%;max-width:600px"></canvas>
<script>
var xyValues = [
  {x:50, y:7},
  {x:60, y:8},
  {x:70, y:8},
  {x:80, y:9},
  {x:90, y:9},
  {x:100, y:9},
  {x:110, y:10},
  {x:120, y:11},
  {x:130, y:14},
  {x:140, y:14},
  {x:150, y:15}
];

new Chart("myChart", {
  type: "scatter",
  data: {
    datasets: [{
      pointRadius: 4,
      pointBackgroundColor: "rgb(0,0,255)",
      data: xyValues
    }]
  },
  options: {
    legend: {display: false},
    scales: {
      xAxes: [{ticks: {min: 40, max:160}}],
      yAxes: [{ticks: {min: 6, max:16}}],
    }
  }
});

var xValues = ["Italy", "France", "Spain", "USA", "Argentina"];
var yValues = [55, 49, 44, 24, 15];
var barColors = [
  "#b91d47",
  "#00aba9",
  "#2b5797",
  "#e8c3b9",
  "#1e7145"
];

new Chart("myChart1", {
  type: "pie",
  data: {
    labels: xValues,
    datasets: [{
      backgroundColor: barColors,
      data: yValues
    }]
  },
  options: {
    title: {
      display: true,
      text: "World Wide Wine Production 2018"
    }
  }
});

const data = {
  labels: [
    'Management Consulting',
    'Pre-Sales & Sales',
    'Project & People Management',
    'Frontend, Visualisations, Design',
    'Python-based Software Engineering',
    'Continuously Acquiring new Technical Skills',
    'Machine Learning & Data Science',
    'Cloud-native Development',
    'Public Speaking & Recognised Open Source Contributions'
  ],
  datasets: [{
    label: 'How I used to spend my time.',
    data: [4, 4, 6, 3, 7, 4, 7, 3, 2],
    fill: true,
    backgroundColor: 'rgba(255, 99, 132, 0.2)',
    borderColor: 'rgb(255, 99, 132)',
    pointBackgroundColor: 'rgb(255, 99, 132)',
    pointBorderColor: '#fff',
    pointHoverBackgroundColor: '#fff',
    pointHoverBorderColor: 'rgb(255, 99, 132)'
  }, {
    label: 'How I want to spend my time.',
    data: [1, 0, 3, 3, 7, 6, 7, 7, 4],
    fill: true,
    backgroundColor: 'rgba(54, 162, 235, 0.2)',
    borderColor: 'rgb(54, 162, 235)',
    pointBackgroundColor: 'rgb(54, 162, 235)',
    pointBorderColor: '#fff',
    pointHoverBackgroundColor: '#fff',
    pointHoverBorderColor: 'rgb(54, 162, 235)'
  }]
};

const config = {
  type: 'radar',
  data: data,
  options: {
    elements: {
      line: {
        borderWidth: 3
      }
    }
  },
};

new Chart("pieChart", config);


</script>

</body>
</html>