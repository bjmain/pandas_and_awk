# pandas_and_awk

### parse csv from command line
awk 'BEGIN { FS = "," } ; { print $(NF-1) }' udc14_19.txt |grep 19|wc -l

## combined DF only on shared columns
combined = pd.concat([df, df1],join='inner')  # default is columns

## output DF to csv
df.to_csv("out.csv.gz",na_rep="NA",index=False)

## Save a DF if you don't want to re-recreate it.
original_df.to_pickle("orig.pkl")
unpickled_df = pd.read_pickle("orig.pkl")
