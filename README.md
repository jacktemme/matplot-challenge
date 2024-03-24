Module 5

This repository takes data from an experiment testing different anti-cancer medictations on mice. The purpose of this experiment is to determine how effective these drugs are on treating squamous cell carcinoma (SCC), which is is a common type of skin cancer. The data for this experiment can be found in the "data" folder with the data analysis in the Jupyter Notebook file. The progam language of Python was used for this analysis along with the pandas and matplot library for data manipulation and visulization. The main findings of this analysis are written up in this file as well:


For certain errors and syntax issues, ChatGPT was utilized for code throughout this analysis:

For creating a simplified code to create a DataFrame with statistical findings, this code was referenced:

    grouped_stats = df.groupby('group')['value'].agg(['mean', 'median', 'var'])

Then this code was used to find the last timepoint of a mouse, by utilizing the tail function:

    last_occurrences = df.groupby('Variable').tail(1)


Finally, syntax help for changing an outlier size and color as well as printing out the r value of a correlation coefficient used this code:

    flierprops=dict(marker='o', markerfacecolor='red', markersize=8))
    
    correlation_coefficient = correlation_result[0]
