### Focus
Use simple libraries and functions to do explorary data analysis.

### Dataset 1: 'ri_police.csv'
* Traffic stops by police officers
* Collected data from 31 US states, but only 'Rhode Island' in this case
* Some of the columns and rows have been removed, full dataset can be downloaded at https://openpolicing.stanford.edu/


### Dataset 2: 'Weather in ri.csv'
* Exploring the weather dataset
* From NOAA: National Centers For Environmental Information

### Libraries
* pandas
* matplotlib.pyplot

### Functions
* df.isnull().sum()
* df.shape
* df.dropna(subset=[' '], inplace=True)
* df.col.astype(' ') / df.dtypes
* df.col1.str.cat(ri.col2, sep=' ')
* pd.to_datetime(col)
* df.value_counts() / df.value_counts(normalize=True)
* df.col.mean()
* df.groupby(['col1', 'col2']).col3.mean()
* df['bool column'] = df.col1.str.contains('string', na=False)
* df.plot() / df.plot(subplots=True) / (kind='bar', stacked= True) / (kind='barh') / (kind='hist', bins=n) / (kind='box')
** # Add the xlabel, ylabel, and title
*** plt.xlabel('Hour')
*** plt.ylabel('Arrest Rate')
*** plt.title('Arrest Rate by Time of Day')
** # Display the plot
*** plt.show()
* df.resample(' ').mean()
* pd.crosstab(df.col1, df.col2)
* df.loc['col1': 'col2'])
* df.col.unique()
* df.col.map({org1 : map1, org2 : map2,.....})
* df.sort_values()
* df['col1', 'col2',...].describe()
* df.sum(axis='columns')
* df.reset_index(inplace=True)
* df.set_index('col', inplace=True)
* newdf = pd.merge(left=df1, right=df2, left_on='df1.col1', right_on='df2.col2', how='left') #right
* df.pivot_table(index='col1', columns='col2', values='col3')
