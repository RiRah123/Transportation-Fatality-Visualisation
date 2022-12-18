# Transportation Fatality Visualisation
[![HTML](https://img.shields.io/badge/HTML-E34F26?style=for-the-badge&logo=HTML5&logoColor=white)]()
[![CSS](https://img.shields.io/badge/CSS-1572B6?style=for-the-badge&logo=CSS3&logoColor=white)]()
[![JavaScipt](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=white)]()
[![SVG](https://img.shields.io/badge/SVG-FFB13B?style=for-the-badge&logo=svg&logoColor=white)]()
[![D3.js](https://img.shields.io/badge/D3.js-F9A03C?style=for-the-badge&logo=D3.js&logoColor=white)]()

## Project Summary

<p align="center">
  <img src="./transportation-fatality-visualisation.gif" width="1000" height="475">
</p>

The `Transportation Fatality Visualisation` is a D3.js multi-line chart visualization, illustrating and comparing the fatality rates (per 100k) for different modes of transportation from 1975 to 2020. On the multi-line chart, the x-axis represented the year, the y-axis represented the death rate, and each line represented a mode of transportation. We also support various user interactions. With our visualisation, users can filter fatality rates for a particular mode of transportation by selecting or deselecting the provided checkboxes. Also, users can evaluate the numerical fatality rates for all current selected modes of transportation of a given year by hovering on the line chart.

## Why We Choose a Multi-Line Chart?
We felt this visualization was appropriate for several reasons. Since the provided CSV file divided the number of vehicle deaths by the year it happened, a line chart would track changes in the number of deaths for a given transportation mode over the years. With our visualization, the audience can quickly identify significant trends, such as cars making about ~70% of the total fatalities and motorcycle fatalities decreasing from 1980-1995 but then increasing again from 1995 onwards. Secondly, we added multiple lines to the line chart as the dataset includes multiple transportation modes rather than one. By including multiple lines and toggling their visibility with the checkboxes, the audience can easily compare the death rates between each transportation type. For example, it is very apparent from our visualization that cars have the highest death rate among all transportation modes, and trucks and motorcycles have the lowest.

## Why We Choose These Variables and How We Encoded Them?
For our visualization, we chose the mode of transportation as our primary variable. As mentioned earlier, we chose this as a variable as the provided dataset already divided deaths by transportation mode, and we thought it was convenient for the audience to compare the death rate between transportation modes. We encoded transportation modes by applying different colors to their respective lines. Based on our in-class lectures, color is a preattentive processing visual cue, allowing users to accumulate basic information from an environment unconsciously. Given this, a user can immediately associate a particular death rate trend with a transportation mode by simply looking at the color of the trend line. Another variable we visualized was the death rate for each transportation per 100K. We chose this over the yearly death rate as it makes it easier for users to understand the likelihood of being involved in a fatal accident if they were to use that mode of transportation. This is because the per 100k values are normalized since all the data is divided by 100,000 people so it also accounts for changes in population. As for how we encoded it, we modified the positioning of the trend line since this is the standard for a multi-chart visualization. Trend lines with a higher position on the multi-line chart indicate a larger fatality rate while those lower indicate a smaller fatality rate

## Important Decisions We Made for Our Visualisation
Finally, we made some other decisions about the dataset and visualization. For example, the population column from the CSV file was removed from our visualization. We decided to cut this metric as we felt it was irrelevant to the visualization’s primary message of illustrating the change in the fatality death rate over time. Including it would only distract the user from the chart’s other visual elements. As for normalization, the data was already normalized per 100k fatalities, so we simply used these values for our visualization. We also provided a filtering option, which would appropriately scale the y-axis based on the modes of transportation selected so that viewers can see more details on demand. This makes it easy to identify any small changes in the fatality rates during certain years. Finally, we decided it was appropriate to include a hovering option because it allowed users to compare direct quantities among the different modes selected for a given year.

## Demo Video

https://user-images.githubusercontent.com/83044307/208308842-ecc59825-7366-48e9-88de-8a717f760939.mp4

# Contacts
- [Amit Kulkarni (Full Stack Developer)](https://github.com/amitkulk123)
- [Rian Rahman (Full Stack Developer)](https://github.com/RiRah123)
