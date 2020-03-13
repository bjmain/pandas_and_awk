# pandas_and_awk

awk 'BEGIN { FS = "," } ; { print $(NF-1) }' udc14_19.txt |grep 19|wc -l

combined = pd.concat([df, df1],join='inner')  # default is columns
 # combined DF only on shared columns

df.to_csv("out.csv.gz",na_rep="NA",index=False)

original_df.to_pickle("orig.pkl")
unpickled_df = pd.read_pickle("orig.pkl")
