# Average, Sum, AverageIf, SumIf -- What you need to know!

Manually summing and then averaging large data sets is quite taxing.  Of course it's easy when there are only a few data points, averaging 2 and 3 is trivial, 2+3 = 5/2 = 2.5, you're done!  However, if I handed you a data set of 1,000 numbers and expected the average quickly I'd be disappointed.  Luckily, Excel has a few built in functions that allow us to easily sum or average together large quantities of data.  These are the Average and Sum functions.  

| | AVERAGE | SUM |
| --- | --- | ---|
|Syntax| AVERAGE(number1, [number2], [number3], ...)| SUM(number1, [number2], [number3], ...)  |
| Examples | AVERAGE(A1:A20), AVERAGE(A1, A2) | SUM(A1:A5), SUM(A1:A5, B1:B5) |

Occasionally, we may want to only sum or average certain pieces of a large data set, but the data set isn't organized or sorted.  For example, we want to only sum purchases over $1000 but your sheet is organized chronologically.  We ~could~ just use AVERAGE, and manually select which cells are over 1000, but this could take an exceptionally long time.  Luckily, (again), Excel has a build in conditional AVERAGE and conditional SUM functions, respectively named AVERAGEIF and SUMIF.

| | AVERAGEIF | SUMIF |
| --- | --- | ---|
| Syntax | AVERAGEIF(range, condition, [average_range])  |SUMIF(range, condition, [sum_range]) |
| Examples | AVERAGEIF (A1:A10, >10) | SUMIF(B10:D4, <50) | 

# How To Use

## Step One - Start with Data
Need to originally have a spreadsheet with different data values that you want to average or sum.   

<img src="https://hggorel.github.io/AdvancedDataScience/assets/images/Spreadsheet.png" width="450" height="325">

## Step Two - Select Cell to Place Average In  
<img src="https://hggorel.github.io/AdvancedDataScience/assets/images/ChoosingCell.png" width="450" height="325">

## Step Three - Write Function Call
For this example, we're going to use the Average function, if you wanted to use a different one you would simply type that command.  

<img src="https://hggorel.github.io/AdvancedDataScience/assets/images/WriteFunctionCall.png" width="450" height="325">

## Step Four - Add Parameters
Let's say we want to average everything in the first column, so we are going to use the range A1:A10.  As you type in the parameters, the range you're selecting will highlight on the spreadsheet.  

<img src="https://hggorel.github.io/AdvancedDataScience/assets/images/FullCommand.png" width="450" height="325">

## Step Five - Hit Enter :)
Hitting enter or leaving the box makes the function execute and leaves you with your final result, no math on your part!  

<img src="https://hggorel.github.io/AdvancedDataScience/assets/images/FinalAverage.png" width="450" height="325">

# Comparing the Different Functions
Our thorough example uses the AVERAGE function, however, to change out the functions you only change the last two steps, let's compare these on our data.

## Average Vs. AverageIf

| AVERAGE | AVERAGEIF |
| --- | --- | 
| hi | hi |
| <img src="https://hggorel.github.io/AdvancedDataScience/assets/images/AverageSmallCommand.png" width="350" height="350"> |  <img src="https://hggorel.github.io/AdvancedDataScience/assets/images/AverageIfCommand.png" width="350" height="350"> |  

<img src="https://hggorel.github.io/AdvancedDataScience/assets/images/AverageVsAverageIf.png" width="300" height="300">  
So we can see that when we're only averaging things that are above 100, the average will go up because the lower numbers aren't bringing the average down.

## Sum Vs. SumIf
| SUM | SUMIF |  
| --- | --- |
| hi | hi |
| <img src="https://hggorel.github.io/AdvancedDataScience/assets/images/SumCall.png" width="300" height="300">  | <img src="https://hggorel.github.io/AdvancedDataScience/assets/images/SumifCall.png" width="300" height="300"> |  

 <img src="https://hggorel.github.io/AdvancedDataScience/assets/images/SumResults.png" width="300" height="300">  
So we can see that the SUMIF is less than the SUM because we restricted which ones we were adding.

# Second Example


<!-- Then link the spreadsheet -->


<!-- ## Welcome to GitHub Pages 

You can use the [editor on GitHub](https://github.com/hggorel/AdvancedDataScience/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files. 

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/hggorel/AdvancedDataScience/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.

-->
