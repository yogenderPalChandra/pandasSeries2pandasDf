#Description: Pip installable package avilable at:

https://pypi.org/project/l-pdseries-2-l-dfs/


The function: <l_pdseries_2_l_dfs> stands for List_pdSeries_to_list_dataFrames, converts a list of
#pandas series to list of pandas data frame. For further easy analysis of 
#list of dfs. Many times we are faced that we have a list of list of pandas df.
# this function helps in such situations

#To use:

import l_pdseries_2_l_dfs as s2df

l_series_2_l_dfs = s2df.l_pdseries_2_l_dfs(l_series, ndfs)

#where l_series is a list of pandas series. It must be of the shape:

>>shape_of_l_series = [inner_element.shape for inner_element in l_series]
>>shape_of_l_series

[(1232,),
 (1232,),
 (1232,),
 (1232,),
 (1232,),
 (1232,),
 (1232,),
 (1232,),
 (1232,),
 (1232,),
 (1232,),
 (1232,),
 (1232,),
 (1232,),
 (1232,),
 (1232,),
 (1232,),
 (1232,),
 (1232,),
 (1232,),
 (1232,),
 (1232,),
 (1232,),
 (1232,),
 (1232,),
 (1232,),
 (1232,),
 (1232,),
 (1232,),
 (1232,),
 (1232,),
 (1232,),
 (1232,),
 (1110,),
 (1110,),
 (1110,),
 (1110,),
 (1110,),
 (1110,),
 (1110,),
 (1110,),
 (1110,),
 (1110,),
 (1110,),
 (1110,),
 (1110,),
 (1110,),
 (1110,),
 (1110,),
 (1110,),
 (1110,),
 (1110,),
 (1110,),
 (1110,),
 (1110,),
 (1110,),
 (1110,),
 (1110,),
 (1110,),
 (1110,),
 (1110,),
 (1110,),
 (1110,),
 (1110,),
 (1110,),
 (1110,),
 (234,),
 (234,),
 (234,),
 (234,),
 (234,),
 (234,),
 (234,),
 (234,),
 (234,),
 (234,),
 (234,),
 (234,),
 (234,),
 (234,),
 (234,),
 (234,),
 (234,),
 (234,),
 (234,),
 (234,),
 (234,),
 (234,),
 (234,),
 (234,),
 (234,),
 (234,),
 (234,),
 (234,),
 (234,),
 (234,),
 (234,),
 (234,),
 (234,),
 (1930,),
 (1930,),
 (1930,),
 (1930,),
 (1930,),
 (1930,),
 (1930,),
 (1930,),
 (1930,),
 (1930,),
 (1930,),
 (1930,),
 (1930,),
 (1930,),
 (1930,),
 (1930,),
 (1930,),
 (1930,),
 (1930,),
 (1930,),
 (1930,),
 (1930,),
 (1930,),
 (1930,),
 (1930,),
 (1930,),
 (1930,),
 (1930,),
 (1930,),
 (1930,),
 (1930,),
 (1930,),
 (1930,),
 (841,),
 (841,),
 (841,),
 (841,),
 (841,),
 (841,),
 (841,),
 (841,),
 (841,),
 (841,),
 (841,),
 (841,),
 (841,),
 (841,),
 (841,),
 (841,),
 (841,),
 (841,),
 (841,),
 (841,),
 (841,),
 (841,),
 (841,),
 (841,),
 (841,),
 (841,),
 (841,),
 (841,),
 (841,),
 (841,),
 (841,),
 (841,),
 (841,)]

# so we have a list of series of pandas series with shapes each: [(1232,), (1110,), (234,), (1930,), #(841,)]
#So if we want to create a data frame out of these list of series we can use the above module. 
#Again we have 33 series (columns) of each of the shape, so we want to make a data frame with 33. Also, #we have 5 different series so we want to have 5 dfs. hence, ndfs = 5 in this case. please choose #according to your data the value of ndfs. correct value of ndfs is imporant otherwise it will throw #error. The return value of module is a list of data frames of shape: [(1207, 33), (1086, 33), (234, #33), (1905, 33), (816, 33)]

 
