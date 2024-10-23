---
layout: post
title:  "Introduction to Seaborn"
date: 2024-10-03
author: Alyssa Ford
description: Getting Started with Seaborn: A Fun Guide to Stunning Data Visualizations
image: "/assets/images/seagull.jpg"
---
<h1>Don’t let your data sink! Take a swim with <em><strong>Seaborn</strong></em></h1>

---

Seaborn, a common package in Python, creates beautiful visuals for your data set. 

Built in styles make graphs easy to read, documentation is simple to learn, and graphics are easy to customize. 

Additionally, seaborn carries built-in statistical functions to create graphs like scatterplots, histograms, and violin plots. 

Here are some cool examples of graphics created using Seaborn!

---

<img src = "{{site.url}}/{{site.baseurl}}/assets/images/graph_beginning.png" alt = "graph_beginning"/>

*This image shows multiple examples of scatterplots and distributions:*

- **A variety of data points** with contrasting colors.
- **Smooth distribution curves** layered over scatterplots.
- **Customized axes** with labels and ticks to enhance readability.
- **Creative layouts** with subplots, offering multiple perspectives on the data.

Explore how Seaborn allows you to channel your inner creativity and bringing your data to life!

---

<img src = "{{site.url}}/{{site.baseurl}}/assets/images/seaborn_heatmap.png" alt = "graph_heat"/>

*This graph is a colorful representation of temperature. The **lighter** the color is, the **hotter**. Seaborn allows users to be creative with their data visualization!*

---

<img src = "{{site.url}}/{{site.baseurl}}/assets/images/Final-scatterplot-in-Seaborn.png" alt = "graph_penguin"/>

*Lastly, we can add **titles**, **colors**, and a **legend** to our graphs. This comes in handy when presenting data to others. In this example, the creator is comparing bill length to bill depth based on species and sex as seen in the difference of shapes and colors.

---

<h2><em><strong>Step 1:</strong></em> Installing Seaborn</h2>

As mentioned previously, Seaborn is a Python library. It is built off of another package called <em><strong>Matplotlib</strong></em>. 

Because of this, it is necessary to make sure Python is installed. 
To check if you have Python installed on your computer, you can open a terminal and type `python --version`. 

The computer will show the version of Python on your computer...if you do not have it installed, here is a link for an easy setup! 

[Click here to install Python](https://www.python.org/downloads/) 

---

Now that we have Python, we are ready to install <em><strong>Seaborn!</strong></em> 

*Keep the terminal open and simply type `pip install seaborn`. This should install automatically onto your computer after a few seconds. 

*To import seaborn into your code, you type `import seaborn as sns` (see picture below) and now you are free to use Seaborn functions! 

<img src = "{{site.url}}/{{site.baseurl}}/assets/images/importing_libraries.png" alt = "graph_import" />

Note: if your confused at any point of installation, here is a link directly to Seaborn!

[Click here to go directly to Seaborn!](https://seaborn.pydata.org/)

---

<h3><em><strong>Step 2:</strong></em> The Basics</h3>

One of the firt things I would recommend when practicing functions in Seaborn is to look through all of their <em><strong>built in data sets</strong></em>. This is a powerful tool to create your own visuals on data that is already clean and provided. 

- In order to discover a built in data set, use the function `sns.get_dataset_names()`. An example that I will use is the "titanic" dataset. 

- To access it, we would type `data = sns.load_dataset('titanic')'. After running this, the titanic dataset is now stored in a variable called "data". 

- To view summarized data, the next line of code written is `data.head()`. This allows us to view the first five rows of our dataset. 
Similarly, we could type `data.tail()` to view the last five rows of the dataset. 

---

## Basic Graph Functions
Here is a list of a few basic graph functions using Seaborn. For simplicity in this post, I have typed my code using a Google Colab File.

<img src = "{{site.url}}/{{site.baseurl}}/assets/images/basic_graphs.png" alt = "graph_basic"/>
 
 Notice the parts of a function in Seaborn:

 - First, we have `sns`. This is consistent in each of our visuals. 
 
 - Next is the name of the plot. The names are pretty self explanatory as `sns.barplot` creates a bar chart, `sns.scatterplot` creates a scatter plot, etc. 
 
 - Following the name of the plot, is a set of paranthesis containing variables. Notice how in each of these plots, we specify our `x` variable, our `y` variable, and our data. Using an equal sign with quotes is how we assign our variables. Since data is already a stored variable, we do not put quotes around it. 
 
 - Lastly, see the line below the graph function where it says `plt.show()`. This will guarantee that your graph will show up in your notebook. Some environments like Jupyter Notebook do not require `plt.show()` to display the graphic, however, I add that line just in case. At this point, try opening a Python file to practice these Seaborn functions. 
 
---

 <h4><em><strong>Advanced Graphs</strong></em> With an Example From My Work </h4>
 <p> Here, I have attached a project I worked on using Seaborn. I created visuals to represent my data but oftentimes, I needed more information than just two variables. I will walk through the details as we go along! <em><strong>First</strong></em> take a look at how I imported my data set. </p>

<img src = "{{site.url}}/{{site.baseurl}}/assets/images/data-myproject.png" alt = "graph_code"/>

*I did not import a dataset from Seaborn. Instead, I imported a dataset from github using Pandas (another Python package). However, Seaborn functions work on any dataset imported.*

---

<img src = "{{site.url}}/{{site.baseurl}}/assets/images/regplot with color.png" alt = "first_graph"/>

<img src = "{{site.url}}/{{site.baseurl}}/assets/images/regplot with color pic.png" alt = "first_another"/>

* This code has details to customize my linear regression plot. At the beginning, I specified my variables as we did in the graphs previously. My `x` variable in this data set is 'sugars' and my `y` variable is 'calories'. 

* `Scatter_kws` customizes the scatter plot on the graph. In this case, I made the color blue with markers of size 50 and an opacity of 70%. 

* Next, `line_kws` customizes the linear regression line. I used a red dashed `"--"` line with a width of 2. 

*Lastly, I made the markers of my scatterplot circles as seen on the visual. These customizations make the graph prettier and easier to read.

---

<img src = "{{site.url}}/{{site.baseurl}}/assets/images/second.png" alt = "graph_second"/>

<img src = "{{site.url}}/{{site.baseurl}}/assets/images/second pic.png" alt = "second_anotha"/>

*This graph has different elements to it! When looking at the code, a lot of it is similar to the previous graph. 

*Now, I added a title `(plt.title('Sugars vs Calories in Cereal'))`, confidence interval bands which are shown by light red outside of the regression line, and labels for `x` and `y`. 

*These are just a few more ways you can expand your creativity to show your data.

---

# **_Seaborn in Python_**
In summary, Seaborn is a valuable tool in Python that aids in data visualization in a simple way. Documentation is clear, there are built in datasets, and it pairs really well with other packages like Pandas. I invite you to spend some time this week to find a dataset you are interested in and practice creating visuals to display information. 