# swund283-Movies-ETL.

This function imports the files from the 3 requested places, cleans up the data, and then creates a data output into a new table.  It also 'lightly' handles errors.

Here are a few assumptions we are making:
1. The file locations won't change. EX: if the json file gets moved or the name changed we need to manually update that.
2. The file structure doesn't change.  If it does we will need to manually add in the the additional 'column' of information to the data output
3. We are assuming that there won't be additional ways to input values.  EX if someone adds in the revenue column a 'new' regex to manage that input
4. We are assuming that as the versions of the software/dependencies get upgrades we will not have any import or parsing errors.  This is a long term risk to using the function.
5. We hardcoded out one outlier in the data.  We are making two assumptions by leaving that piece of code. A) that outlier will continue to be an outlyer and needs to be surpassed.  B) that no other outliers will come as the data changes.  We are only managing that one outlier we identified when investigating this initial dataset.

 
