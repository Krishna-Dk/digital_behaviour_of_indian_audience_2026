<html lang="en">
<head>
<meta charset="UTF-8">
<title>Digital Behaviour of Indian Audience (2026)</title>
<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>

<style>
body {
    font-family: Arial, sans-serif;
    margin: 20px;
    background: #f5f7fa;
}

h1 {
    text-align: center;
    color: #2c3e50;
}

.container {
    width: 90%;
    margin: auto;
}

.section {
    margin-bottom: 40px;
    padding: 20px;
    background: white;
    border-radius: 10px;
    box-shadow: 0px 2px 8px rgba(0,0,0,0.1);
}

canvas {
    max-width: 600px;
    margin: auto;
    display: block;
}

p {
    line-height: 1.6;
}
</style>
</head>

<body>

<h1>Digital Behaviour of Indian Audience (2026)</h1>

<div class="container">

<div class="section">
<h2>Overview</h2>
<p>
India has become one of the largest digital markets in the world with over 900 million internet users. 
Digital behaviour in India is driven by mobile-first usage, increasing social media engagement, 
video consumption, and rapid adoption of digital payments.
</p>
</div>

<div class="section">
<h2>Usage Distribution</h2>
<canvas id="barChart"></canvas>
</div>

<div class="section">
<h2>Activity Share</h2>
<canvas id="pieChart"></canvas>
</div>

<div class="section">
<h2>Growth Trend</h2>
<canvas id="lineChart"></canvas>
</div>

<div class="section">
<h2>Key Insights</h2>
<p>
• Mobile usage dominates internet access in India.<br>
• Social media and video platforms are the most consumed content.<br>
• Regional language content is growing rapidly.<br>
• Digital payments are widely accepted across urban and rural areas.<br>
• Internet usage is becoming part of daily lifestyle activities.
</p>
</div>

</div>

<script>

// BAR CHART
new Chart(document.getElementById("barChart"), {
    type: 'bar',
    data: {
        labels: ["Mobile Usage", "Social Media", "Video Content", "Digital Payments", "Regional Content"],
        datasets: [{
            label: "Usage (%)",
            data: [85, 70, 60, 75, 80]
        }]
    },
    options: {
        responsive: true,
        plugins: {
            legend: { display: false }
        }
    }
});

// PIE CHART
new Chart(document.getElementById("pieChart"), {
    type: 'pie',
    data: {
        labels: ["Social Media", "Video", "Payments", "Browsing", "Others"],
        datasets: [{
            data: [30, 25, 20, 15, 10]
        }]
    },
    options: {
        responsive: true
    }
});

// LINE GRAPH
new Chart(document.getElementById("lineChart"), {
    type: 'line',
    data: {
        labels: ["2022", "2023", "2024", "2025", "2026"],
        datasets: [{
            label: "Internet Users (in millions)",
            data: [750, 800, 850, 900, 950],
            fill: false,
            tension: 0.3
        }]
    },
    options: {
        responsive: true
    }
});

</script>

</body>
</html>
