* **Data visualization:** The graphic representation and presentation of data.
1. Looking at visuals in order to understand and draw conclusions about data.
2. Creating visuals using raw data to tell a story.

## Frameworks for organizing your thoughts about visualization

Frameworks help organize your thoughts about data visualization and give you a useful checklist to reference as you plan and evaluate your data visualization. Here are two frameworks that employ slightly different techniques. Both are intended to improve the quality of your visuals. 

[The McCandless method](https://www.informationisbeautiful.net/visualizations/what-makes-a-good-data-visualization/)

The McCandless method lists four elements of good data visualization: 
1. **Information:** the data with which you’re working 
2. **Story:** a clear and compelling narrative or concept
3. **Goal:** a specific objective or function for the visual
4. **Visual form:** an effective use of metaphor or visual expression

[Kaiser Fung’s Junk Charts trifecta checkup](https://www.junkcharts.com/junk-charts-trifecta-checkup-the-definitive-guide/)

This approach is a set of questions that can help consumers of data visualization critique what they are consuming and determine how effective it is. You can also use these questions to determine if your data visualization is effective:
1. What is the practical question? 
2. What does the data say?
3. What does the visual say? 
Each of these questions offers an opportunity to investigate a given problem with a slightly different context. A well-designed visual effectively answers all three of those questions at once. Moreover, this framework helps you think about your data viz from the perspective of your audience.

### Marks

**Marks** are basic visual objects such as points, lines, and shapes. Every mark can be broken down into four qualities:
1. **Position:** Where is a specific mark in space relative to a scale or to other marks? 
For example, if you’re looking at two different trends, position allows you to compare the pattern of one element relative to another. 

![simple line chart with two lines. One is red and one is blue, and there is obvious space between them.](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/w13YHmt8QaiMlhM_FMoQnA_20fa0b545f3d43779dad888c4eab81f1_PoHaiHktPbMb89eEc9Vpp-UE_BTfwzjST1tLbw1_3HOQ7m0bSk9A2t7Bv-w7nM_57RH4dUH92FkOsuNe0RN6mlu15J8WF1WP3NuoToX7QUOd2UCGjzosjgeeaPnG_gaVxJm4rOoCc5r-ApSOG6ZdPiw?expiry=1783635137667&hmac=dtyOxdpPRpeCJWUZRlA54Jk8HQpjBC56sepbvh5tX5I)

2. **Size:** How big, small, long, or tall is a mark?
The comparison of object sizes can be an easy visual interpretation for humans. This can be very useful for conveying the relationship between categories or data points. However, this also presents a potential problem: The human eye can inadvertently interpret comparisons that aren’t intended to convey meaning. For example, sometimes objects that appear to be the same size when they are not. Controlling the scale of a visual is important even when comparative sizes are not intended to offer information.

![A plot with points that are different sizes.](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/G1By0iKbT6S20RyOJOLakw_8e3b96d8d62b41dab3a0e9b037da2cf1_GODjKcAHrADKXJsRxDT2itjTl9NO4ism_dt63kvp6YzrO7aIUOhVjyUscltPeyX2XNlXJwyEOGz1ibCd7JZXTnAlcjVB3Wvtfjcszugj1WSA4XWqoGP-UHGlrlC54ZNksUkdKtXHlg6Wg7AD_HJMgZU?expiry=1783635137667&hmac=JXTMUQ6FccwJxtHT-n4iC9lXzj_ee8TR4JPyB7KXZW8)

3. **Shape:** Does the shape of a specific object communicate something about it?
Rather than using simple dots or lines, a bit of creativity can enhance how quickly people are able to interpret a visual by using shapes that align with a given application. In the example below, it is immediately obvious that numbers of people are represented because the bars are person-shaped. 

![horizontal bar chart, but bars are made of icons shaped like people](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/vIWV0cFASZG52lgye2TkcA_32e7afe4ba304c8db5d3dd396a1e5ff1__mfHWWDLd73KXZcCE8V0tPKY1iltunaMx63y5jMoIXySA0-d1Hx40MZctiQIlt2yZNTr_r0wp3NRjDA7L8mrPRJPZls-ta5RPIeDbYssZMDiLrfWolXOXKF5kkY67YPr8WfkgMzxZK-WNlB53g-_rIU?expiry=1783635137667&hmac=se1kcFZbPzFoeA9Bh1nzxvKpfPJCYdWQANDVxpcAIIE)

4. **Color:** What color is a mark?
Colors can be used both as a simple differentiator of groupings or as a way to communicate other concepts such as profitable versus unprofitable, or hot versus cold. 

![a bar chart with a red, green, yellow, grey, and blue bar](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/i6Lpsc88RzeYrF-r61-lkA_c9ee968f09d24a33849524397a00a7f1_uWZn95j6KM0A4os33IazLDL0nNrpIix7WMtlZ_4sb9HafOB0G4kVuQ7vR0oXEhn9WVnLkCKj8sAMffZKaZHSN7z6gkgcLfK1plWtwxXdaFWB5mnMii8lgVewDtq6DRmzDad_9yzAFpQ1kFoGm12aWE8?expiry=1783635137667&hmac=7cwmoPqiCiCNk0jbD56OIr9xMaaDL251-xDCRmm_Itg)

### Channels

**Channels** are visual aspects or variables that represent characteristics of the data in a visualization. They are basically specialized marks that have been used to visualize data. It’s important to understand that channels vary in terms of how effective they are at communicating data based on three elements: 
1. **Accuracy:** Are the channels helpful in accurately estimating the values being represented?

For example, color is very accurate when communicating categorical differences, such as apples and oranges. But it is much less effective when distinguishing quantitative data, such as 5 from 5.5.

![a plot with apples and oranges representing the data points](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/Wf6s1QnXRXSjIqWek_8Sag_d7aefd5069c34982bb9e2b6ee00083f1_eddRCinr1PXCxLOOT7ouF1uWgWXoPJsomsNUfjno7rJ4AT4IDk10Elhyvr8HX8wIfxIj2Xj0ATEHcGv26wenha8PMqjkWo3UnZOToCze3iWgzhZx9_a6Zth5fSPHR7wC6fKxY0B4ICh9jHbLyB4L0QI?expiry=1783635137667&hmac=_oUkqMMtdK0qBZl4u-siT_cQ0Gay4c4ONbP_j6f3Srw)

2. **Popout:** How easy is it to distinguish certain values from others?
There are many ways of drawing attention to specific parts of a visual, and lots of them leverage pre-attentive attributes including line length, size, line width, shape, enclosure, hue, and intensity.

![a line chart with three blue lines of different shades, and one red line](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/sxYBbaJKSsuP4_7UcjOeew_d8c55324fda24a5c9f4d53f59c393df1_9V9JqTSQJKOQ5Gn-fkp-ZmJILLWBHwvKOJGFXhrBXs2Vo2mOVUENTLqJbs9nQucXedmVprZ_EhmZz2JBTYTVpfWtSGDqfUaEOxP0Bm8TUwbKYLwjPwd4zpbL2AFUQJZ3xKKfrNqDoY8ofGqkPvqaI3Y?expiry=1783635137667&hmac=to241uL1c9RQwkaM2_48S4sLw9AOXdZk2xldUj__8CA)

3. **Grouping:** How effective is a channel at communicating groups that exist in the data?
Consider the proximity, similarity, enclosure, connectedness, and continuity of the channel.

![bar chart with four groups of bars. In each group, there is a red bar and a blue bar](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/YVCqvj29RueUw-qbXakeiQ_55494966d85946208cb20fa514cddcf1_clRwSjOaDIJfbIETWvYtnENapMqisUqPNl6ZOpdVKMyD8UwKbulM6NodwVe3N_ePiuwzGm9qbaWSS10vHgnhAeICBrN5j4sDpO931SkKSriacYXA8OHcb3XYkyZzsrV5jD1x-CMXSxQ0ps1cOD0oEv8?expiry=1783635137667&hmac=HyVi8pLVnt7k-3BoM8lHYS4BNXyz3IvwjWNTJ4yZtqI)

But, remember: The more you emphasize one single thing, the more that counts. Emphasis diminishes with each item you emphasize because the items begin to compete with one another.


* **Bar graphs:** Use size contrast to compare two or more values.
* **Line graphs:** Help your audience understand shifts or changes in your data.
* **Pie charts:** Show how much each part of something makes up the whole.
* **Maps:** Help organize data geographically.


### Useful links
- [The data visualization catalogue](https://datavizcatalogue.com/#google_vignette "The Data Visualization Catalogue"): Not sure where to start with data visualization? This catalogue features a range of different diagrams, charts, and graphs to help you find the best fit for your project. As you navigate each category, you will get a detailed description of each visualization as well as its function and a list of similar visuals. 
    
- [The 25 best data visualizations](https://visme.co/blog/best-data-visualizations/ "The 25 best data visualizations"): In this collection of images, explore the best examples of data that get made into a stunning visual. Simply click on the link below each image to get an in-depth view of each project, and learn why making data visually appealing is so important.
    
- [10 data visualization blogs](https://www.tableau.com/learn/articles/best-data-visualization-blogs "10 data visualization blogs"): Each link will lead you to a blog that is a fountain of information on everything from data storytelling to graphic data. Get your next great idea or just browse through some visual inspiration.  
    
- [Information is beautiful](https://informationisbeautiful.net/wdvp/gallery-2019/ "Information is beautiful"): Founded by David McCandless, this gallery is dedicated to helping you make clearer, more informed visual decisions based on facts and data. These projects are made by students, designers, and even data analysts to help you gain insight into how they have taken their own data and turned it into visual storytelling.
    
- [Data studio gallery](https://datastudio.google.com/gallery?category=visualization "Data studio gallery"): Information is vital, but the information presented in a digestible way is even more useful. Browse through this interactive gallery and find examples of different types of data communicated visually. You can even use the data studio tool to create your own data-driven visual.

* **Correlation charts:** Show relationships among data
* **Causation:** Occurs when an action directly leads to an outcome.

## Correlation and causation
- **Correlation** in statistics is the measure of the degree to which two variables move in relationship to each other. An example of correlation is the idea that “As the temperature goes up, ice cream sales also go up.” It is important to remember that correlation doesn’t mean that one event causes another. But, it does indicate that they have a pattern with or a relationship to each other. If one variable goes up and the other variable also goes up, it is a positive correlation. If one variable goes up and the other variable goes down, it is a negative or inverse correlation. If one variable goes up and the other variable stays about the same, there is no correlation.
- **Causation** refers to the idea that an event leads to a specific outcome. For example, when lightning strikes, we hear the thunder (sound wave) caused by the air heating and cooling from the lightning strike. Lightning causes thunder.![[Pasted image 20260710231145.png]]

* **Static visualizations:** Do not change over time unless they're edited.
* **Dynamic visualizations:** Visualizations that are interactive or change over time.
* **Tableau:** A business intelligence and analytics platform that helps people see, understand, and make decisions with data.

## Line chart 

A **line chart** is used to track changes over short and long periods of time. When smaller changes exist, line charts are better to use than bar graphs. Line charts can also be used to compare changes over the same period of time for more than one group.

## Column chart 

**Column charts** use size to contrast and compare two or more values, using height or lengths to represent the specific values.

## Heatmap 

Similar to bar charts, **heatmaps** also use color to compare categories in a data set. They are mainly used to show relationships between two variables and use a system of color-coding to represent different values

## Pie chart

The **pie chart** is a circular graph that is divided into segments representing proportions corresponding to the quantity it represents, especially when dealing with parts of a whole

## Scatterplot

**Scatterplots** show relationships between different variables. Scatterplots are typically used for two variables for a set of data, although additional variables can be displayed.
## Distribution graph

A **distribution graph** displays the spread of various outcomes in a dataset.
Let’s apply this to real data. To account for its supplies, a brand new coffee shop owner wants to measure how many cups of coffee their customers consume, and they want to know if that information is dependent on the days and times of the week. That distribution graph would resemble something like this:

![Histogram showing cups of coffee purchased across all 7 days of the week largest consumed mid week on Wednesday around 100](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/iXJq4GcJRM-yauBnCZTPkQ_68a9c0b7f2314e4c82bb4f134c178c52_Screen-Shot-2021-02-26-at-4.42.30-PM.png?expiry=1783826734494&hmac=4XCAr-zKS1dAJSCXivOv6txkxuuM25XPXjQRDobcg20)

From this distribution graph, you may notice that the amount of coffee sales steadily increases from the beginning of the week, reaching the highest point mid-week, and then decreases towards the end of the week.

Reviewing each of these visual examples, where do you notice that they fit in relation to your type of data? One way to answer this is by evaluating patterns in data. Meaningful patterns can take many forms, such as:

- **Change:** This is a trend or instance of observations that become different over time. A great way to measure change in data is through a line or column chart.
    
- **Clustering:** A collection of data points with similar or different values. This is best represented through a distribution graph.
    
- **Relativity:** These are observations considered in relation or in proportion to something else. You have probably seen examples of relativity data in a pie chart.
    
- **Ranking:** This is a position in a scale of achievement or status. Data that requires ranking is best represented by a column chart.
    
- **Correlation:** This shows a mutual relationship or connection between two or more things. A scatterplot is an excellent way to represent this type of data pattern.

## Data grows on decision trees

A **decision tree** is a decision-making tool that allows you, the data analyst, to make decisions based on key questions that you can ask yourself. Each question in the visualization decision tree will help you make a decision about critical features for your visualization. Below is an example of a basic decision tree to guide you towards making a data-driven decision about which visualization is the best way to tell your story. Please note that there are many different types of decision trees that vary in complexity, and can provide more in-depth decisions. 

![A decision tree leading to the best chart](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/iV-otJ4pQCafqLSeKZAmjg_9519536f4aa94268af3600263793b237_Screen-Shot-2021-02-23-at-4.21.13-PM.png?expiry=1783827018735&hmac=EDZTgdVC5PhMZ0d1YtUGyblYGmPvgC34X22Xgr8AvOI)

-Does your data have only one numeric variable? Histogram or Density plot -Are there multiple data sets?  Line chart or pie chart -Are you measuring changes over time? Bar chart -Do relationships between the data need to be shown? Scatter plot or heatmap

## Begin with your story

Start off by evaluating the type of data you have and go through a series of questions to determine the best visual source:

- **Does your data have only one numeric variable?** If you have data that has one, continuous, numerical variable, then a histogram or density plot are the best methods of plotting your categorical data. Depending on your type of data, a bar chart can even be appropriate in this case. For example, if you have data pertaining to the height of a group of students, you will want to use a histogram to visualize how many students there are in each height range:
    

![A histogram measuring the height of students and how many students are in each height grouping](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/rVQyQMBvRoKUMkDAbwaCWg_aaa67e65c6254e76998babe14f84b525_Screen-Shot-2021-03-02-at-10.48.02-AM.png?expiry=1783827018735&hmac=0K9YcjmZrpBn3p-E4GZqKRw6oWZ85CMBUFA8RfyzPfE)

- **Are there multiple datasets?** For cases dealing with more than one set of data, consider a line or pie chart for accurate representation of your data. A line chart will connect multiple data sets over a single, continuous line, showing how numbers have changed over time. A pie chart is good for dividing a whole into multiple categories or parts. An example of this is when you are measuring quarterly sales figures of your company. Below are examples of this data plotted on both a line and pie chart.
    

![A line graph measuring quarterly sales figures throughout 1st, 2nd, 3rd and 4th quarters](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/3MRAH5jdRuaEQB-Y3Sbm7A_67d5ecf363804b8d8f285bfc648b3639_Screen-Shot-2021-03-02-at-10.48.34-AM.png?expiry=1783827018735&hmac=NKXz84kb6oXp_qdPM-_vF42xzyt_2m3Gsk7r1yMtyFE)

![A pie chart measuring quarterly sales figures for 1st quarter (55.6%), 2nd quarter (30.1%), 3rd q (7.8%), 4th q (6.5%)](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/y7sQLyDRQpG7EC8g0cKRAA_e678b13ea07e4d15ad451695bf469514_Screen-Shot-2021-03-02-at-10.48.39-AM.png?expiry=1783827018735&hmac=8OABiaQakmlU2GcxU-CQrlQg_9yw5kZXljNh2hAsNVQ)

- **Are you measuring changes over time?** A line chart is usually adequate for plotting trends over time. However, when the changes are larger, a bar chart is the better option. If, for example, you are measuring the number of visitors to NYC over the past 6 months, the data would look like this:
    

![A bar graph measuring number of visitors over the months of June to November](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/Qb5mXHLIQuu-ZlxyyNLrbg_db202cb2d1c4496b8953ed5212b0b465_Screen-Shot-2021-03-02-at-10.50.00-AM.png?expiry=1783827018735&hmac=jHKexPVxj0De5TXtBKOJov6JWdcB8w9l5gVo7twrMwI)

- **Do relationships between the data need to be shown?** When you have two variables for one set of data, it is important to point out how one affects the other. Variables that pair well together are best plotted on a scatterplot. However, if there are too many data points, the relationship between variables can be obscured so a heat map can be a better representation in that case. If you are measuring the population of people across all 50 states in the United States, your data points would consist of millions so you would use a heat map. If you are simply trying to show the relationship between the number of hours spent studying and its effects on grades, your data would look like this:
    

![A scatterplot measuring the rise in test scores corresponding with the increase of minutes spent studying](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/s3R2A0spTg-0dgNLKe4Paw_b5332baafd9346bb8d1311bbda388d5d_Screen-Shot-2021-03-02-at-10.50.39-AM.png?expiry=1783827018735&hmac=q2K_-C-ExF6MAwigytBu6vL-KA1ZRSm0VdzQne1HG38)

Before you use the decision tree in a scenario to create successful data visualizations, take a moment to review some of the design concepts and best practices you’ve learned so far. Recall that there are four elements of successful data visualization:

- **Information:** reflects the conclusion you’ve drawn from the data, which you will communicate with visualization
    
- **Story:** adds meaning to the data and makes it interesting
    
- **Goals:** makes the data usable and useful
    
- **Visual form:** creates both beauty and structure
    

![Four overlapping ovals outlining the four different parts of data visualization: Information, story, goal, and visual form](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/nFq79wWOSAC69Riv8u086w_91eec3046e334a6981c6c02f694de7e1_image.png?expiry=1783827141732&hmac=IDpSoVu9Wh2pq-UEjLntMpzkYR6KtIokHTDk_1e8MsE)

### Design data visualizations
The elements of art:
* Line: Can be curved or straight, thick or thin, vertical, horizontal, or diagonal. They can add visual form to your data and help build a structure for your visualization.
* Shape: Should always be two-dimensional. Three-dimensional objects can confuse the audience in a visualization. Shapes are also a great way to add eye-catching contrast, especially size contrast.
* Color: Can be described by their hue (blue, green, red, etc), intensity (how bright or dull a color is) and value (how dark and light the colors are in a visualization).
* Space: Is the area between, around and in the objects. There should always be space in data visualizations.
* Movement: Used to create a sense of flow or action in a visualization.

## Principles of design
There are nine basic **principles of design** that data analysts should think about when building their visualizations.  

![The 9 principles of design icons: Balance, emphasis, movement, pattern, repetition, proportion, rhythm, variety, unity](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/mn0oQGvPS2K9KEBrz8tidQ_a674eeba5224451db6df1c973e41d44b_Screen-Shot-2021-02-26-at-3.20.16-PM.png?expiry=1783902093962&hmac=mnVJksVLtIhpcCsn3eWdJnDoZdna8guKbLDdsj7bao0)

**1. Balance**: The design of a data visualization is balanced when the key visual elements, like color and shape, are distributed evenly. This doesn’t mean that you need complete symmetry, but your visualization shouldn’t have one side distracting from the other. If your data visualization is balanced, this could mean that the lines used to create the graphics are similar in length on both sides, or that the space between objects is equal.

**2. Emphasis:** Your data visualization should have a focal point, so that your audience knows where to concentrate. In other words, your visualizations should emphasize the most important data so that users recognize it first. Using color and value is one effective way to make this happen. By using contrasting colors, you can make certain that graphic elements—and the data shown in those elements—stand out.

**3. Movement:** Movement can refer to the path the viewer’s eye travels as they look at a data visualization, or literal movement created by animations. Movement in data visualization should mimic the way people usually read. You can use lines and colors to pull the viewer’s attention across the page.

**4. Pattern:** You can use similar shapes and colors to create patterns in your data visualization. This can be useful in a lot of different ways. For example, you can use patterns to highlight similarities between different data sets, or break up a pattern with a unique shape, color, or line to create more emphasis.

**5. Repetition:** Repeating chart types, shapes, or colors adds to the effectiveness of your visualization. Think about the book sales chart from the previous example: the repetition of the colors helps the audience understand that there are distinct sets of data. You may notice this repetition in all of the examples we have reviewed so far. Take some time to review each of the previous examples and notice the elements that are repeated to create a meaningful visual story.

**6. Proportion:** Proportion is another way that you can demonstrate the importance of certain data. Using various colors and sizes helps demonstrate that you are calling attention to a specific visual over others. If you make one chart in a dashboard larger than the others, then you are calling attention to it. It is important to make sure that each chart accurately reflects and visualizes the relationship among the values in it.

**7. Rhythm:** This refers to creating a sense of movement or flow in your visualization. Rhythm is closely tied to the movement principle. If your finished design doesn’t successfully create a flow, you might want to rearrange some of the elements to improve the rhythm.

**8. Variety:** Your visualizations should have some variety in the chart types, lines, shapes, colors, and values you use. Variety keeps the audience engaged. But it is good to find balance since too much variety can confuse people. The variety you include should make your dashboards and other visualizations feel interesting and unified.

**9. Unity:** The last principle is unity. This means that your final data visualization should be cohesive. If the visual is disjointed or not well organized, it will be confusing and overwhelming.

* **Data composition:** Combining the individual parts in a visualization and displaying them together as a whole.

Elements for effective visuals:
* Clear meaning: Communicate their intended insight.
* Sophisticated use of contrast: Separate the most important data from the rest using visual context.
* Refined execution: Include deep attention to detail, using visual elements like lines, shapes, colors, value, space and movement.

Four elements of successful visualizations:
- **Information (data):** The information or data that you are trying to convey is a key building block for your data visualization. Without information or data, you cannot communicate your findings successfully.
    
- **Story (concept):** Story allows you to share your data in meaningful and interesting ways. Without a story, your visualization is informative, but not really inspiring. 
    
- **Goal (function):** The goal of your data visualization makes the data useful and usable. This is what you are trying to achieve with your visualization. Without a goal, your visualization might still be informative, but can’t generate actionable insights.
    
- **Visual form (metaphor):** The visual form element is what gives your data visualization structure and makes it beautiful. Without visual form, your data is not visualized yet.

### Design thinking and visualizations
* **Design thinking:** A process used to solve complex problems in a user-centric way.
Design process has five phases:
* **Empathize**: Here you think about the emotions and needs of the target audience of your data viz, whether it's stakeholders, team members or the general public.
* **Define**: Helps you to find your audiences needs, their problems and your insights. "Which data to show in your visualization".
* **Ideate**: You start to generate your data viz ideas. Brainstorm potential data viz solutions.
* **Prototype**: Putting visualizations together for testing and feedback.
* **Test:** Showing prototype visualizations to people before stakeholders see them.

## Headlines that pop

A **headline** is a line of words printed in large letters at the top of a visualization to communicate what data is being presented. It is the attention grabber that makes your audience want to read more.

## Subtitles that clarify

A **subtitle** supports the headline by adding more context and description. Adding a subtitle will help the audience better understand the details associated with your chart. Typically, the text for subtitles has a smaller font size than the headline.

## Labels that identify

A **label** in a visualization identifies data in relation to other data. Most commonly, labels in a chart identify what the x-axis and y-axis show. Always make sure you label your axes. Data can also be labeled directly in a chart instead of through a chart legend. This makes it easier for the audience to understand data points without having to look up symbols or interpret the color coding in a legend.

## Annotations that focus

An **annotation** briefly explains data or helps focus the audience on a particular aspect of the data in a visualization.

Applying all of the above:

![[Pasted image 20260713133836.png]]

|Visualization components|Guidelines|Style checks|
|---|---|---|
|Headlines|- **Content**: Briefly describe the data - **Length**: Usually the width of the data frame - **Position**: Above the data|- Use brief language - Don’t use all caps - Don’t use italic - Don’t use acronyms - Don't use abbreviations - Don’t use humor or sarcasm|
|Subtitles|- **Content**: Clarify context for the data - **Length**: Same as or shorter than headline - **Position**: Directly below the headline|- Use smaller font size than headline - Don’t use undefined words - Don’t use all caps, bold, or italic - Don’t use acronyms - Don't use abbreviations|
|Labels|- **Content**: Replace the need for legends - **Length**: Usually fewer than 30 characters - **Position**: Next to data or below or beside axes|- Use a few words only - Use thoughtful color-coding - Use callouts to point to the data - Don’t use all caps, bold, or italic|
|Annotations|- **Content**: Draw attention to certain data - **Length**: Varies, limited by open space - **Position**: Immediately next to data annotated|- Don’t use all caps, bold, or italic - Don't use rotated text - Don’t distract viewers from the data|

## Ways to make data visualizations accessible:
* **Labeling**
* **Text alternatives**
	* **Alternative text:** Alternative text provides a textual alternative to non-text content.
* **Text-based format**
* **Distinguishing**
* **Simplify**

  
![Image of pie chart divided into 4 timed sections which equal 60 minutes](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/n11dF8pFSbKdXRfKRdmy9A_c0707d21e99d4004b8b2fe44e32c55b6_Screen-Shot-2021-02-26-at-4.35.02-PM.png?expiry=1784051155339&hmac=-7bTwte92ycwB50mayKRUXFSvc7tFjNl-OZrALqd4jc)

Follow this high-level 60-minute chart to guide your thinking whenever you begin working on a data visualization. 

**Prep (5 min):** Create the mental and physical space necessary for an environment of comprehensive thinking. This means allowing yourself room to brainstorm _how_ you want your data to appear while considering the amount and type of data that you have.

**Talk and listen (15 min):** Identify the object of your work by getting to the “ask behind the ask” and establishing expectations. Ask questions and really concentrate on feedback from stakeholders regarding your projects to help you hone how to lay out your data. 

**Sketch and design (20 min):** Draft your approach to the problem. Define the timing and output of your work to get a clear and concise idea of what you are crafting.

**Prototype and improve (20 min):** Generate a visual solution and gauge its effectiveness at accurately communicating your data. Take your time and repeat the process until a final visual is produced. It is alright if you go through several visuals until you find the perfect fit.

## Glossary terms

**Alternative text:** Text that provides an alternative to non-text content, such as images and videos

**Annotation:** Text that briefly explains data or helps focus the audience on a particular aspect of the data in a visualization

**AVERAGEIF:** A spreadsheet function that returns the average of all cell values from a given range that meet a specified condition 

**Balance:** The design principle of creating aesthetic appeal and clarity in a data visualization by evenly distributing visual elements

**Bar graph:** A data visualization that uses size to contrast and compare two or more values

**Calculus:** A branch of mathematics that involves the study of rates of change and the changes between values that are related by a function 

**Causation:** When an action directly leads to an outcome, such as a cause-effect relationship

**Channel:** A visual aspect or variable that represents characteristics of the data in a visualization

**Chart:** A graphical representation of data from a worksheet

**Cluster:** A collection of data points on a data visualization with similar values

**CONVERT:** A SQL function that changes the unit of measurement of a value in data

**Correlation:** The measure of the degree to which two variables change in relationship to each other

**CREATE TABLE:** A SQL clause that adds a temporary table to a database that can be used by multiple people

**Data composition:** The process of combining the individual parts in a visualization and displaying them together as a whole 

**Decision tree**: A tool that helps analysts make decisions about critical features of a visualization

**Design thinking:** A process used to solve complex problems in a user-centric way

**Distribution graph:** A data visualization that displays the frequency of various outcomes in a sample 

**DROP TABLE:** A SQL clause that removes a temporary table from a database

**Dynamic visualizations:** Data visualizations that are interactive or change over time

**Emphasis:** The design principle of arranging visual elements to focus the audience’s attention on important information in a data visualization

**HAVING:** A SQL clause that adds a filter to a query instead of the underlying table that can only be used with aggregate functions

**Headline:** Text at the top of a visualization that communicates the data being presented

**Heat map:** A data visualization that uses color contrast to compare categories in a dataset

**Histogram:** A data visualization that shows how often data values fall into certain ranges

**Inner query:** A SQL subquery that is inside of another SQL statement

**Label:** Text in a visualization that identifies a value or describes a scale

**Legend:** A tool that identifies the meaning of various elements in a data visualization

**Line graph:** A data visualization that uses one or more lines to display shifts or changes in data over time

**Map:** A data visualization that organizes data geographically

**Mark:** A visual object in a data visualization such as a point, line, or shape

**MAXIFS:** A spreadsheet function that returns the maximum value from a given range that meets a specified condition

**Mental model:** A data analyst’s thought process and approach to a problem

**Movement:** The design principle of arranging visual elements to guide the audience’s eyes from one part of a data visualization to another

**MINIFS:** A spreadsheet function that returns the minimum value from a given range that meets a specified condition

**Narrative:** (Refer to story)

**Ordinal data:** Qualitative data with a set order or scale

**Pattern:** The design principle of using similar visual elements to demonstrate trends and relationships in a data visualization

**Pie chart:** A data visualization that uses segments of a circle to represent the proportions of each data category compared to the whole

**Pre-attentive attributes:** The elements of a data visualization that an audience recognizes automatically without conscious effort

**Proportion:** The design principle of using the relative size and arrangement of visual elements to demonstrate information in a data visualization

**R:** A programming language used for statistical analysis, visualization, and other data analysis 

**Ranking:** A system to position values of a dataset within a scale of achievement or status

**Relativity:** The process of considering observations in relation or proportion to something else

**Repetition:** The design principle of repeating visual elements to demonstrate meaning in a data visualization

**Rhythm:** The design principle of creating movement and flow in a data visualization to engage an audience

**Scatterplot:** A data visualization that represents relationships between different variables with individual data points without a connecting line 

**SELECT INTO:** A SQL clause that copies data from one table into a temporary table without adding the new table to the database

**Sort range:** A spreadsheet menu function that sorts a specified range and preserves the cells outside the range

**Sort sheet:** A spreadsheet menu function that sorts all data by the ranking of a specific sorted column and keeps data together across rows

**Static visualization:** A data visualization that does not change over time unless it is edited

**Story:** The narrative of a data presentation that makes it meaningful and interesting 

**Subtitle:** Text that supports a headline by adding context and description

**Tableau:** A business intelligence and analytics platform that helps people visualize, understand, and make decisions with data

**Unity:** The design principle of using visual elements that complement each other to create aesthetic appeal and clarity in a data visualization

**Variety:** The design principle of using different kinds of visual elements in a data visualization to engage an audience

**Visual form:** The appearance of a data visualization that gives it structure and aesthetic appeal

**X-axis:** The horizontal line of a graph usually placed at the bottom, which is often used to represent time scales and discrete categories

**Y-axis:** The vertical line of a graph usually placed to the left, which is often used to represent frequencies and other numerical variables


Continues in [[Module 2 - Create Data Visualizations with Tableau]]