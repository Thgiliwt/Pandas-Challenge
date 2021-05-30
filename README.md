# Pandas-Challenge
This is the 4th homework from my coding bootcamp course.
This assignment involves using Pandas in Python to solve tasks via Jupyer Notebook. Due to the recent lock-down I am not able to slice my working time in days so I have to try to finish it as least time as possible. That is the reason why this time I have not made many commits as before. For the assignment, I have picked the option 1, 'Heroes of Pymoli' to work with. It is basically very straight forword where I could just apply very basic functions etc. to obtain the answers. However there are things I am not sure about.

## Key Reflects

### New Findings
I have researched for some methods or functions to assist in completing some of the tasks, such as '.div(<a list>,axis=0)' to calculate the 'avg total purchase per person' under purchasing analysis (age), is to use a column of data within a dataframe divide another list of data, the 'axis=0' is to set the division along the row or index so the corresponded value will be determined. 'pd.concat' and '~<a dataframe>.columns.duplicated()' to merge multiple dataframes and then remove the dulicapted column names at once. This is super efficient.

### New Tricks
This is mostly applied in order to stylish or manage the layout of displays. I could use '.set_index(['col1','col2'...])' to hide the index numbers and column labels in the printed table. I could also use '.rename_axis(None)' to achieve the same outcomes. The '.to_frame()' is a easier way to generate a series to be displayed as a dataframe.
    
### Uncertainties
There are things I am not sure, for example, under the purchasing analysis (age) task, I see a 'settingwithcopywarning' after the final outcome. The results are correct and I made my study on this issue, it looks like that that the list I set 'ppl' is treated as a slice from a dataframe, where it may confuse the system whether if this value should be returned back. With this being said, I am not sure if this is the cause.
Another one is that, my method to solve most of the tasks is:
    1.  'select related data from raw data'
    2.  'find the first column of values using groupby or generating new dataframe'
    3.  'find the second column of values ...'
    4.  repeat the above steps until all values are determined
    5.  combine all dataframes together
    6.  adjust layouts, styles etc. to form the final output table or display
I have viewed some of the posts about how to apply calculations to a groupby dataframe directly, such as .agg, .apply and then using lambda x etc. But I have not tried as it just making the functions complcated.
