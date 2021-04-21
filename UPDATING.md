# How to update the lists

Since the primary purpose of this list is to help other blocklist maintainers understand and incorporate these domains into their own lists, all of the blocklists are managed through the `domains.csv` file. This simple CSV spreadsheet acts as a sort of database for recording each URL discovered from the papers and documenting its purpose with sources wherever possible.

Because this spreadsheet is a regular CSV file, it can be opened in any sane CSV-capable editor such as LibreOffice or Excel and edited like any spreadsheet (including formulas, formulas not included).

However, because a CSV will preserve the order that the rows are in when you save them, PLEASE be sure to **re-sort by the `order` column (ascending/low-to-high order please) prior to saving if you performed any sorting or filtering on the rows**. This helps keep the diffs clean and readable when your changes are committed. If your changes are hard to review, then the review process may take longer.

If you make any changes to a domain, please ensure that your changes are made to **all domains or URLs to which that change applies** as the spreadsheet contains some domains multiple times in order to preserve the URL that they were initially part of within the associated papers. Sorting by either the `id` column or the `raw_domain` column will group matching domain names together so its easier to make all these changes at once. Dont forget to sort by `order` when you are about to save so you dont commit needless re-arrangements of the rows in the list to the repository.

*Note:* There are a few domains that seem to be identical but are assigned two different `id` values. These appear to be potentially due to formatting errors (such as using a hyphen vs an em-dash) when parsing urls from the original PDF's but were left in due to uncertainty surrounding whether these could be valid as separate domains. If you know for certain that these similar characters are not allowed in domain names, feel free to submit a pull request to correct them.

If you make any changes to the "list" column that specifies which list that domain belongs to, you will also need to regenerate the list files by running `python3 update-lists.py`.


