# Stacked Bar Chart for Visualizing Monotonically Varying Data

Line chart is often used for visualizing data. But if the data varies monotonically, it may be replaced by a bar chart.

The height of this bar chart directly represents the final value of the variable (y) whereas the color encoded body of the bar chart describes what ranges of x contributes to the change in the variable(y). By using this type of encoding:

- We eliminate the visual clutering of the line chart. This is the main aim of this chart.
- We focus more on the final value of variable (y) and less on the intermediate values. (This may be a good or a bad thing depending on the need of user)

Possible further improvements/changes include:

- Addition of curvy gridlines for constant values of x. This may even eliminate the need of using color encoding for bar chart.
- Extending this idea for monotonically decreasing data.

## Example

In this example, we show how total deaths per million increased (monotonically) over time. The regions of continuous same(similar) color shows that during that color(time range), there was a huge increase in total deaths.

![Alt](monotonic_bar_chart.png "Monotonic Data represented using Bar Chart")

(TODO: Correct the color bar by using datetime formatter)

Compared to this, when we use line chart, we get a cluttered view. To remove this visual clutering, the user needs interaction and/or good color encoding scheme. This becomes particularly challenging as we increase the number of countries.

![Alt](monotonic_line_chart.png "Monotonic Data represented using Line Chart")
