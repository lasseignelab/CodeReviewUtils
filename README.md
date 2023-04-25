# CodeReviewUtils


## Purpose
Functions used to compare outputs during code review in the Lasseigne lab

## Usage Examples

compareObj.R compares saved R objects

```{r}
cr_path <- here::here("results", "CR_results", "processed_normalized_expression")
ca_path <- here::here("results", "CA_results", "processed_normalized_expression")
compare_obj(ca_path = ca_path, cr_path = cr_path)
```

compareDelim.R compares saved delimited files

```{r}
cr_path <- here::here("results", "CR_results", "alpaca_run")
ca_path <- here::here("results", "CA_results", "alpaca_run")
compare_delim(ca_path = ca_path, cr_path = cr_path, delim = "\t", patt = ".txt")
```

compareFigs.R stages image files for visual comparison

```{r}
cr_path <- here::here("results", "CR_results", "FAERS_plots")
ca_path <- here::here("results", "CA_results", "FAERS_plots")
compare_figure(ca_path = ca_path, cr_path = cr_path, patt = ".png")
```

