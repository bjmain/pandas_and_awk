# pandas_and_awk

### parse csv from command line
awk -F "," '$19=="S"' udc01_19.txt

## combined DF only on shared columns
combined = pd.concat([df, df1],join='inner')  # default is columns

## output DF to csv
df.to_csv("out.csv.gz",na_rep="NA",index=False)

## Save a DF if you don't want to re-recreate it.
original_df.to_pickle("orig.pkl")
unpickled_df = pd.read_pickle("orig.pkl")

# find and replace 
for f in *_uploader.sh; do sed -i 's/bmh/bmm/g' $f; done

# batch cancel
scancel {19403854..19403880}
