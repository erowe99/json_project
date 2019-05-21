#### JSON Exercise Results:
1. Find the 10 countries with most projects
The 10 countries with most projects
                               
countryname     |    count    
--------------- | -----------------          
People's Republic of China        | 19
Republic of Indonesia             | 19
Socialist Republic of Vietnam     | 17
Republic of India                 | 16
Republic of Yemen                 | 13
Kingdom of Morocco                | 12
Nepal                             | 12
People's Republic of Bangladesh   | 12
Africa                            | 11
Republic of Mozambique            | 11

2. Find the top 10 major project themes (using column 'mjtheme_namecode')

name  | code | count
----- | ---- | -------
Environment and natural resources management |  11   |  250
Rural development                            |  10   |  216
Human development                             |   8   |  210
Public sector governance                     |   2  |  199
Social protection and risk management        |   6  |  168
Financial and private sector development     |   4  |  146
Social dev/gender/inclusion                  |   7   | 130
Trade and integration                        |   5  |   77
Urban development                            |   9   |  50
Economic management                        |     1  |   38

3. In 2. above you will notice that some entries have only the code and the name is missing. Create a dataframe with the missing names filled in.

New dataframe json_df_filled is a copy of json_df but with filled values for missing theme names

Example entry that is filled now:

> json_df['mjtheme_namecode'][0]:
>
> `[{'code': '8', 'name': 'Human development'}, {'code': '11', 'name': ''}]`
>
> json_df_filled['mjtheme_namecode'][0]:
>
> `[{'code': '8', 'name': 'Human development'}, {'code': '11', 'name': 'Environment and natural resources management'}]`


