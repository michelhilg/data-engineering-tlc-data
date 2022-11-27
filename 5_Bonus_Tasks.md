# Bonus Tasks

In this markdown, we will present some extra comments regarding the bonus tasks:

## 1. Weather Conditions

<em>Your data scientists want to make future predictions based on weather conditions. How would you expand your pipeline to help your colleagues with this task?</em>

One good way to expand the pipeline to support this analysis will be by searching for new data regarding the weather in NYC City, ingesting this data, transforming it, and after load in the same database to the data science team be able to query together with data., making correlations.

## 2. Excel Data

<em>Another colleague approaches to you. They are an Excel expert and have been using this tool for a long time. So they need all the available taxi trip records in the XLSX format. Can you re-use your current pipeline? How does this output compare to your existing formats? Do you have any performance concerns?</em>

We could reuse some steps of the pipeline, but now 100%. That is because the output would not be the same, an Excel `.xlsx` only could deal with around 1.05 million rows, so we have to split the data into chunks, or start working with a new time metric, like months. The performance could be a problem since we are working within the limit of the Excel tool.

