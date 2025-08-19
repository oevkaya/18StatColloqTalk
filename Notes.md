## **3. Fundamental Concepts of Data Visualization**

In terms of the data visualization task, it is crucial to understand the data set you have, type of variables and which data viz representations are suitable for the succesful data story telling. Beyond these details, it is a very design-oriented process from the design perspective to avoid any harm on human sight or perception. Rather than manipulating what the raw data says by its nature, the designer should stick to the certain design choices based on the problem and data set. For this purpose, this section collects and gathers various related ideas and details to investigate the necessity of data visualization for data communication and specific principles alongside the effective and responsible data visualization practices. 

> The simple graph has brought more information to the data analyst's mind than any other device. (John Tukey)

### 3.1 What is Data Visulization, Why Do We Need to Visualize?

As human begins we are generally both good and bad in terms of seeing inherited patterns, spot anomalies, generate questions from them when they look at any specific data viz case. Generally, the purpose is to literally *see* what your data seems to say. This framework allows to communicate findings clearly and persuasively with audience under the pre-specified design choices that we are making accordingly. Especially, for the data analysis workflow, to understand data and ask relevant research questions, this exploration, known as Exploratory Data Analysis (EDA), plays a crucial role from beginning to end, for identyfing the relevant rabbit hole to dive in and any possible refinement of the analysis for later stages. 

In a different way, EDA is the first step in **understanding** the main features and structures of a data set, this brings us doing specific data visualization type choices and as such. There are many statistical tools and techniques are used when performing EDA, but crucially they are **simple** to allow the data __speak__ for itself, including but not limited to the list of (i) Data transformation/wrangling, (ii) Calculation of simple summary statistics (mean, median, variance, correlation, etc.) and (iii) tabulation, graphical or visual representations. From that point of view, to investigate our toolkit in an efficient way, it is better to focus on the concept of graphical or visual representations in depth. 

### 3.2 Data Types and Appropriate Visualization Techniques

There are many types of data visualisation, each designed with a particular purpose of conveying a message. As a rule of thumb, to determine which visualisation style is appropriate, we need to consider the responses of such questions 

1. What are the properties and type of variables? Either having a Quantitative or Qualitative variable etc.
2. How many variables to include in the data visualisation? Either we have univariate, bivariate or multivariate style of visualization 
3. What aspect of the data do you want to explore, investigate and communicate? Either just illustrative or supportive for the results

Regarding the types of variables, a brief summary can be examplified as follows including some data set variables that is described before 

| Variable Type | Subtype                | Description                                                              | Examples                                                 |
| ------------- | --------------------   | ------------------------------------------------------------------------ | -------------------------------------------------------- |
| Quantitative  | Discrete               | Describes count data, typically non-negative integer values.             | Number of IDS students; number of election votes.        |
| Quantitative  | Continuous             | Real-valued measurements, rounded to a specified number of decimals/s.f. | Penguin bill length; body mass; flipper length.          |
| Qualitative   | Categorical (factor)   | Unordered labels; arithmetic is not meaningful.                          | Penguin breeds (Adelie, Chinstrap, Gentoo).              |
| Qualitative   | Ordinal                | Categories with a natural ordering, possibly unequal spacing             | Degree grades: First, upper-second, lower-second, third. |
| Temporal      | Date / duration        | Calendar/time values; often analyzed via derived numeric features.       | Dates, timestamps, time deltas                           | 
| Spatial       | Geographic coordinates | Location information on a map or grid.                                   | Latitude/longitude, easting/northing                     |

For the case of Quantitative case, one can also consider a varible as Proportion / percentage that describes Fraction of a whole; bounded, often derived from counts.  On the Qualitative side, one specific categorical example can be Binary (dichotomous) setting that defines exactly two categories such as Passed/Failed; Vaccinated/Not. Most of the time, in data sets one can detect directly Identifier (key) syle of variables that stores unique labels (ie. Codes, IDs, UUIDs, postcodes) used to identify entities; not analyzed as features. 

In terms of the number of variables, one might to univariate data visulization to identify what is the _location_, _spread_ and _shape_ of the data, via **histogram** or **box plot**. When the interest is the relatioship between two variables, this setting can be defined as bivariate data visulization specifically that covers examples like **scatter plot**, or **segmented bar plot**. Whenever the the relationship between many variables are investigated simultaneously, this can be called as Multivariate data visualization which requests additional aspects or breakdown using **colour**, **style** and/or **faceting**.

All these details brings us the necessity of certain principles that we need to follow. In principle, when we visualize data, the data values are converted systematically and logically into the visual elements for specific purposes. One one hand, this process is mapping data into certain aesthetics that preserves data properties and with this mapping we are creating different visuals under specific recipes. With the jargon from "grammer of graphics", aesthetics describe every aspect of a given graphical element such as position, shape, size, color. Depending on the type of varibles of interest, some of these aesthetics can represent both continuous and discrete data (position, size, line width, color) while others can usually only represent discrete data (shape, line type). One illustrative image can be borrowed from [Fundamentals of Data Visualization](https://clauswilke.com/dataviz/), given as below Figure 3X.1

Figure 3X.1

### 3.3 Principles of Effective Visualization



### 3.4. Navigating your journey: Additional resources 

Thanks to the open-source minded people and all passionate developers, designers in the field of data visualization, there are various sources to understand what is the most effective way of doing data visualization. Specifically, certain resources include both examples and the correspondign code snippets under differen languages that allows reader can adapt the given example to their scenario over a different data set. Definitely listing all sources can be another useful curation, but here the most widely know and up-to-date ones are listed with their brief details 

#### [RSS: Best Practices for Data Visualisation](https://royal-statistical-society.github.io/datavisguide/)

Mainly, **Best Practices for Data Visualisation** aims to equip readers with the fundamentals for creating data visualizations that are high-quality, readable, impactful, and accurate in both presentation and interpretation. This specific guide blends both the scientific and creative aspects of visualization — it emphasizes that data viz is not just plotting defaults, but actively telling a story and choosing design elements deliberately to serve that story. Although primariy aim is better visuals at RSS publications (Significance magazine, JRSS Series A, Real World Data Science), the guidance is broadly relevant for any data viz task. 

To select the right chart type, their suggested two aspects of data to dig in, **Data type** and **Data relationship** with specific external sources to create your checklist. In terms of the design chocies point of view, one should think about these items (i) Be clear on the visualization's purpose, (ii) Know your audience, (iii) Choose chart type based on data structure or relationship (iv) Refine with audience’s graph literacy in mind. They emphasised the importance of styling for the accesibility purposes, that means using thoughtful choices in color, annotation, fonts, and alternative text. From that angle, **Unstyled** version uses default colors and labels, whereas **Styled** version includes readable font sizes, contrast-aware color fills, in-chart labels, and clear titles/subtitles — vastly improving interpretability.  

