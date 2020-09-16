# Class 12: Reading Assignment 12
*Secions Read:*
- [Article](https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/)
- [Chart.js](https://www.chartjs.org/docs/latest/)
- Several MDN articles on `<canvas>`

### What is Chart.js?
Chart.js is an opensource JavaScript library that utilizes the `<canvas></canvas>` tag to easily create visually stunning charts for your webpage. Chart.js is a collection of JavaScript files that you can access remotely or you can download locally to your machiine. 


### Why use Chart.js?
Charts overall are easier for a viewer to understand datasets; data becomes visualized and easier to interpret rather than reading values from a table. Besides, Chart.js does all of the hardwork for you. Reading through the [documentation](https://www.chartjs.org/docs/latest/) and all you need to know is readily available. 

Chart.js offers support for several different chart types: bar, line, pie, radar, bubble, scatter and you can even mix charts together on a single graph. 

### Example Code: 
***NOTE:*** this piece of code was taken from my Lab 12 script and modified to be used as an example. 

```
var ctx = document.getElementById('CanvasID').getContext('2d');
    var mixedChart = new Chart(ctx, {
        type: 'bar', 
        data: {
            datasets: [{
                label: '# of Likes',
                data: [4, 6, 2, 1, 1]
            }, {
                label: '# of Dislikes',
                data: [3, 3, 4, 2, 2],
            }],
            labels: ['Cat','Dog','Mouse','Fish', 'Bird'],
        },

        options: {
            legend: {
                display: false,
            },
            title: {
                display: true,
                text: 'Pets: Liked & Disliked',
                position: 'top'
            }
        }
    });
```

`type` intakes a string that indicates the type of graph that Chart.js will produce hence `'bar'`

`label` intakes a string to label the data being displayed on the y-axis for this bar chart

`data:`intakes an array of values to be displayed on the y axis

`labels` not to be confused with label in dataset, labels the x axis 

`options` offers additional chart options. `legend` and `title` are chosen for the example 

`legend` controls the legend options

`title` controls the title options, allows you to set the title and position it