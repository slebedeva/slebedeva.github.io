# My personal TILs 

I got the idea of "TILs" (today I learned): small posts where you write what you learned today from [Stephen Turner](https://stephenturner.us/) who in turn got it from [Simon Willison](https://til.simonwillison.net/).

### 2025

### 2024

### December

**polars**  
`pl.scan_csv()` - super quick taking a look into a data frame without loading it into memory  
`pl.explode()` - allows to make columns with all combinations of values from one column (e.g. [1:{1,2,3}] will become [1:1,1:2,1:3]

### November  

**git**  
`git switch my_remote_branch` is a command to create a new local branch from a remote branch if a local branch doesn't exist yet.

**jupyter**  
`%%capture` is a magic that will capture stdout of the cell.

### October

**pandas**  
`df[::10]` will print every 10th row

**sklearn**  
`feature_extraction.DictVectorizer` (use it to one hot encode categorical features) - especially useful for json input data.

**python env management**  
There is a new kid on the block: [uv](https://docs.astral.sh/uv/). Written in Rust and supposed to be fast.

### September

**pandas x json**  
To convert your list of dictionaries coming from an API request to a pd.DataFrame in one go, use `pd.json_normalize(response.json())`.

**QSAR models**  
QSAR stands for [Quantitative structure-activity relationship](https://en.wikipedia.org/wiki/Quantitative_structure%E2%80%93activity_relationship#). These models predict activity or property of a molecule (y) based on its physical and chemical characteristics (X).  
Conveniently, there is a [kaggle dataset](https://www.kaggle.com/datasets/rajgupta2019/qsar-bioconcentration-classes-dataset). Of course, dedicated packages exist in [R](https://cran.r-project.org/web/packages/rQSAR/vignettes/QSAR-Workflow.html) as well as more modern [python framework with uncertainty quantification](https://chemrxiv.org/engage/chemrxiv/article-details/6603ff689138d231616f084c). See also this recent [cheminformatics course](https://github.com/PatWalters/practical_cheminformatics_tutorials).

**snakemake schemata**  
I was reminded about snakemake validation schema. This allows you to validate that your input is in proper format. See [docs](https://snakemake.readthedocs.io/en/stable/snakefiles/configuration.html#validation).
