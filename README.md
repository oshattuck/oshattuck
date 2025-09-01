<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The U.S. Gun Control Debate: A Data-Driven Overview</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
        }
        .chart-container {
            position: relative;
            width: 100%;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
            height: 300px;
            max-height: 400px;
        }
        @media (min-width: 768px) {
            .chart-container {
                height: 350px;
            }
        }
    </style>
</head>
<body class="bg-gray-100">

    
    

    
    
    
    
    

    <div class="container mx-auto p-4 md:p-8">
        <header class="text-center mb-12">
            <h1 class="text-4xl md:text-5xl font-bold text-[#003f5c] mb-2">The Firearm Debate</h1>
            <p class="text-lg text-gray-600">A Data-Driven Look at "Common Sense" Gun Control</p>
        </header>

        <main class="grid grid-cols-1 md:grid-cols-2 gap-8">
            
            <div class="md:col-span-2 bg-white rounded-lg shadow-md p-6">
                <h2 class="text-2xl font-bold text-[#003f5c] mb-4 text-center">The Scale of Gun Violence in the U.S.</h2>
                <p class="text-gray-700 mb-6 text-center max-w-3xl mx-auto">To understand the debate, it's crucial to first grasp the numbers. The United States has a gun homicide rate and a level of gun ownership that are unique among high-income countries. The data below provides context on the annual toll of gun violence, which forms the foundation for many arguments on both sides.</p>
                <div class="flex flex-col md:flex-row items-center justify-around gap-8">
                    <div class="text-center">
                        <p class="text-6xl font-bold text-[#ff764a]">43,675</p>
                        <p class="text-lg text-gray-600 mt-2">Total Gun Deaths in 2023</p>
                        <p class="text-sm text-gray-500">(Source: Gun Violence Archive)</p>
                    </div>
                    <div class="chart-container w-full max-w-xs h-64 md:h-72">
                        <canvas id="gunDeathsChart"></canvas>
                    </div>
                </div>
            </div>

            
            <div class="md:col-span-2 bg-white rounded-lg shadow-md p-6">
                <h2 class="text-2xl font-bold text-[#003f5c] mb-4">The Case for Regulation</h2>
                <p class="text-gray-700 mb-6">Proponents of stricter gun control argue that data shows a clear link between access to firearms and increased violence. They often point to international comparisons and loopholes in current laws to make the case for policy changes aimed at reducing firearm availability.</p>
                <div class="grid grid-cols-1 lg:grid-cols-2 gap-8">
                    <div>
                        <h3 class="text-xl font-semibold text-[#374c80] mb-2 text-center">U.S. Gun Homicide Rate vs. Other High-Income Countries</h3>
                        <p class="text-sm text-gray-600 mb-4 text-center">This chart compares the firearm homicide rate per 100,000 people, highlighting the disparity between the U.S. and its economic peers. This data is often used to argue that the prevalence of guns is a primary driver of lethal violence.</p>
                        <div class="chart-container h-80 md:h-96">
                            <canvas id="countryComparisonChart"></canvas>
                        </div>
                    </div>
                    <div>
                        <h3 class="text-xl font-semibold text-[#374c80] mb-2 text-center">Public Support for Key Policies</h3>
                        <p class="text-sm text-gray-600 mb-4 text-center">Despite political polarization, polling indicates broad public support for several specific gun control proposals. Proponents argue this consensus should translate into legislative action.</p>
                        <div class="chart-container h-80 md:h-96">
                            <canvas id="policySupportChart"></canvas>
                        </div>
                    </div>
                </div>
            </div>

            
            <div class="md:col-span-2 bg-white rounded-lg shadow-md p-6">
                <h2 class="text-2xl font-bold text-[#003f5c] mb-4">The Case for Gun Rights</h2>
                <p class="text-gray-700 mb-6">Opponents of stricter gun control emphasize the constitutional right to self-defense and question the effectiveness of such laws. They argue that firearms are a crucial deterrent to crime and that policy should focus on criminals and mental health rather than restricting the rights of law-abiding citizens.</p>
                <div class="grid grid-cols-1 lg:grid-cols-2 gap-8 items-center">
                    <div class="text-center p-4">
                        <h3 class="text-xl font-semibold text-[#7a5195] mb-2">Defensive Gun Use (DGU)</h3>
                        <p class="text-sm text-gray-600 mb-4">A central argument for gun rights is the use of firearms for self-protection. While highly debated, studies estimate that DGUs occur frequently, suggesting guns can be a powerful deterrent to crime.</p>
                        <p class="text-4xl md:text-5xl font-bold text-[#ffa600]">Up to 2.5 Million</p>
                        <p class="text-lg text-gray-600 mt-2">Estimated Defensive Gun Uses Annually</p>
                        <p class="text-sm text-gray-500">(Source: 2021 National Firearms Survey, Kleck)</p>
                    </div>
                    <div>
                        <h3 class="text-xl font-semibold text-[#7a5195] mb-2 text-center">U.S. Crime & Gun Ownership Trends</h3>
                        <p class="text-sm text-gray-600 mb-4 text-center">This chart plots the U.S. violent crime rate against the estimated number of firearms per capita over several decades. Opponents of gun control use this data to argue that there is no simple correlation between the number of guns and the rate of violent crime.</p>
                         <div class="chart-container h-80 md:h-96">
                            <canvas id="crimeTrendsChart"></canvas>
                        </div>
                    </div>
                </div>
            </div>

            
            <div class="md:col-span-2 bg-white rounded-lg shadow-md p-6">
                <h2 class="text-2xl font-bold text-[#003f5c] mb-4 text-center">Discussion Questions</h2>
                <div class="max-w-3xl mx-auto">
                    <ul class="list-disc list-inside space-y-4 text-gray-700">
                        <li>In light of the <span class="font-semibold">Heller</span> decision affirming an individual's right to bear arms, what is the constitutional and legal limit of "reasonable regulation" for firearms in the interest of public safety?</li>
                        <li>How can policymakers effectively address the issue of gun violence when there is such a wide range of data and disagreement on the number of Defensive Gun Uses (DGUs) annually?</li>
                        <li>What ethical considerations must be balanced when implementing "red flag" laws, particularly concerning due process and an individual's rights before they have committed a crime?</li>
                        <li>Considering the unique cultural and legal context of the United States, are policy models from other countries regarding gun control truly applicable or effective, and why or why not?</li>
                    </ul>
                </div>
            </div>
        </main>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', function () {
            
            const brilliantBluesPalette = {
                bg1: 'rgba(0, 63, 92, 0.7)',
                bg2: 'rgba(188, 80, 144, 0.7)',
                bg3: 'rgba(255, 118, 74, 0.7)',
                bg4: 'rgba(255, 166, 0, 0.7)',
                border1: 'rgba(0, 63, 92, 1)',
                border2: 'rgba(188, 80, 144, 1)',
                border3: 'rgba(255, 118, 74, 1)',
                border4: 'rgba(255, 166, 0, 1)',
            };

            const tooltipTitleCallback = (tooltipItems) => {
                const item = tooltipItems[0];
                let label = item.chart.data.labels[item.dataIndex];
                if (Array.isArray(label)) {
                    return label.join(' ');
                }
                return label;
            };

            const commonChartOptions = {
                responsive: true,
                maintainAspectRatio: false,
                plugins: {
                    legend: {
                        position: 'bottom',
                        labels: {
                            font: {
                                size: 12,
                                family: 'Inter'
                            }
                        }
                    },
                    tooltip: {
                        callbacks: {
                            title: tooltipTitleCallback
                        }
                    }
                },
                scales: {
                    y: {
                        ticks: {
                             font: { family: 'Inter' }
                        }
                    },
                    x: {
                       ticks: {
                             font: { family: 'Inter' }
                        }
                    }
                }
            };
            
            function wrapLabel(str, maxWidth) {
                if (str.length <= maxWidth) return str;
                const words = str.split(' ');
                let lines = [];
                let currentLine = words[0];

                for (let i = 1; i < words.length; i++) {
                    if (currentLine.length + words[i].length + 1 < maxWidth) {
                        currentLine += ' ' + words[i];
                    } else {
                        lines.push(currentLine);
                        currentLine = words[i];
                    }
                }
                lines.push(currentLine);
                return lines;
            }


            
            const gunDeathsCtx = document.getElementById('gunDeathsChart').getContext('2d');
            new Chart(gunDeathsCtx, {
                type: 'doughnut',
                data: {
                    labels: ['Suicide', 'Homicide', 'Accidental & Other'],
                    datasets: [{
                        label: 'Breakdown of Gun Deaths (2023)',
                        data: [25327, 16952, 1396],
                        backgroundColor: [brilliantBluesPalette.bg1, brilliantBluesPalette.bg2, brilliantBluesPalette.bg4],
                        borderColor: [brilliantBluesPalette.border1, brilliantBluesPalette.border2, brilliantBluesPalette.border4],
                        borderWidth: 1
                    }]
                },
                options: {
                    ...commonChartOptions,
                     plugins: {
                        ...commonChartOptions.plugins,
                        title: {
                            display: true,
                            text: 'Breakdown of Gun Deaths (2023)',
                            font: { size: 16, family: 'Inter', weight: 'bold' },
                            color: '#374c80'
                        }
                    }
                }
            });

            
            const countryComparisonCtx = document.getElementById('countryComparisonChart').getContext('2d');
            new Chart(countryComparisonCtx, {
                type: 'bar',
                data: {
                    labels: ['United States', 'Canada', 'France', 'Australia', 'Germany', 'United Kingdom'],
                    datasets: [{
                        label: 'Firearm Homicide Rate per 100,000 People',
                        data: [6.1, 0.8, 0.6, 0.4, 0.3, 0.1],
                        backgroundColor: brilliantBluesPalette.bg1,
                        borderColor: brilliantBluesPalette.border1,
                        borderWidth: 1
                    }]
                },
                options: { ...commonChartOptions }
            });

            
            const policySupportCtx = document.getElementById('policySupportChart').getContext('2d');
            const policyLabels = [
                'Universal Background Checks',
                'Preventing mentally ill from purchasing guns',
                '"Red Flag" Laws',
                'Ban on "Assault-Style" Weapons'
            ].map(label => wrapLabel(label, 16));

            new Chart(policySupportCtx, {
                type: 'bar',
                data: {
                    labels: policyLabels,
                    datasets: [{
                        label: '% Public Support',
                        data: [88, 85, 72, 63],
                        backgroundColor: brilliantBluesPalette.bg2,
                        borderColor: brilliantBluesPalette.border2,
                        borderWidth: 1
                    }]
                },
                options: {
                    ...commonChartOptions,
                    indexAxis: 'y',
                }
            });
            
            
            const crimeTrendsCtx = document.getElementById('crimeTrendsChart').getContext('2d');
            new Chart(crimeTrendsCtx, {
                type: 'line',
                data: {
                    labels: ['1993', '2000', '2010', '2020', '2022'],
                    datasets: [
                        {
                            label: 'Violent Crime Rate (per 100k)',
                            data: [747.1, 506.5, 404.5, 398.5, 380.7],
                            borderColor: brilliantBluesPalette.border1,
                            backgroundColor: brilliantBluesPalette.bg1,
                            yAxisID: 'y'
                        },
                        {
                            label: 'Firearms per 100 Residents',
                            data: [90, 95, 108, 120, 120.5],
                            borderColor: brilliantBluesPalette.border3,
                            backgroundColor: brilliantBluesPalette.bg3,
                            yAxisID: 'y1'
                        }
                    ]
                },
                options: {
                     ...commonChartOptions,
                     scales: {
                        y: {
                            type: 'linear',
                            display: true,
                            position: 'left',
                            title: { display: true, text: 'Violent Crime Rate' }
                        },
                        y1: {
                            type: 'linear',
                            display: true,
                            position: 'right',
                            title: { display: true, text: 'Firearms per 100 Residents' },
                            grid: {
                                drawOnChartArea: false
                            }
                        }
                    }
                }
            });
        });
    </script>
</body>
</html>

<!--
**oshattuck/oshattuck** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
