Git location: https://gitlab.com/TheInceptors/finmark/CodeLibrary.git

#### Import csv as panda dataframe
* dailyFullUsdChfD1_pd = pd.read_csv('datasets/2018-05-02-UsdChfD1.csv')

#### Renaming panda dataframe columns
* dailyFullUsdChfD1_pd.columns = ['0', '0','DHigh','DLow','0', '0']

#### Picking a column argument dataframe 
* mDataTime0400_pd = hourlyFullUsdChf_pd [(hourlyFullUsdChf_pd['Time'] == '04:00')]

#### Numpy count results
* (BuyPosSubResult_np == 'Success').sum()

#### Python 3 length count
* countResultForSell = len(SellPosSubResult_np)

#### Drop NaN
* df.dropna()
* https://pandas.pydata.org/pandas-docs/stable/generated/pandas.DataFrame.dropna.html

#### Slicing columns 
* H1_UsdChf_Reshaped01_pd = H1_UsdChf_pd.drop(H1_UsdChf_pd.columns[[0, -1]], axis=1)

#### Resetting Index
* # Reset the index
* H1_UsdChf_Reshaped01_pd.reset_index()

#### Setting Index
* df.set_index('month')

#### Dropping columns (index must start at zero)
* dailyFullUsdChfD1_pd = dailyFullUsdChfD1_pd.drop(['na', 'Close'], axis=1)

#### Display rows 
* mask = H1FullUsdChf_pd[H1FullUsdChf_pd['Date'] == '2015.05.19']

#### Concatenate
* T00x04UsdChf_pd = pd.concat([T0700UsdChf_pd, T0000UsdChf_pd], axis=1)

#### Selecting Columns for max value between H08 and H09
tableH0809 = SummaryTable06[['H08','H09']]

#### Picking Columns
tableC07 = SummaryTable06[['C07']]
