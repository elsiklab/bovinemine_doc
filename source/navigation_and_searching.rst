Navigation and Searching in BovineMine
======================================

There are several ways for users to query BovineMine.

Quick Search
~~~~~~~~~~~~

**Quick Search** allows users to search keywords from any of the BovineMine datasets. There is a Quick Search box on the BovineMine home page or a smaller search box in the upper right corner of all pages.

**We are currently working to fix our Quick Search tool and hope to have it running again soon.**

 .. figure:: images/QuickSearch.png
   :width: 280
   :alt: Quick Search Box on BovineMine home page
   :figclass: align-center
   
   Quick Search from home page
   
   ..



 .. figure:: images/Search-Any.png
   :width: 280
   :alt: Quick Search Box on any page
   :figclass: align-center

   Quick Search from any page
   
   ..

Quick Searches can be conducted with a number of identifiers including gene names, transcripts, pathways, gene identifiers or organisms.  The wildcard character `*` can be used to retrieve all results that match a particular search query.  

As an example, we will consider gene **rpl24**. Enter *rpl24* in the search box and click **Search**. The results page is tabulated and shows a summary about your query, as shown below.


 .. figure:: images/rpl24-search-result.png
   :width: 800px
   :height: 376px
   :alt: rpl24 search result
   :figclass: align-center

   ..

Users can filter the results based on **Category** and **Organism**. The score column in the result table indicates the similarity of your query to each of the result fetched by BovineMine.

The results page can also be converted to a list. To enable this feature click on **Gene** in **Hits by Category**.


 .. figure:: images/rpl24-search-result-filtered.png
   :width: 800px
   :height: 320px
   :alt: filtered rpl24 search result
   :figclass: align-center
   
   ..

This will filter the results for the feature type **Gene** and checkboxes will be available for users to select genes they would like to add to their list. Once the genes are selected, click on **CREATE LIST**.


.. _templates:

Templates
~~~~~~~~~

**Templates** or predefined queries are another search method within BovineMine.  Popular templates are displayed on the home page, grouped by category (e.g., Genes, Proteins, Interactions) and the complete list can be seen by clicking the **Templates** menu tab.


 .. figure:: images/templates-home.png
   :width: 696
   :alt: Popular templates home page
   :figclass: align-center

   Popular templates

   ..

 .. figure:: images/templates-list.png
   :width: 696
   :alt: Full template list
   :figclass: align-center

   Full list of templates on Templates page

   ..

As an example, the **Gene -> Homologues** template queries BovineMine to retrieves all homologues for a given gene.  Here, we will do a search for the gene *GSTM1*.

 .. figure:: images/Gene-homolog-template.png
   :width: 696
   :alt: Gene --> Homologue
   :figclass: align-center

   Example: Gene --> Homologue

   ..

The results page displays all of the homologues for that query gene.  When logged in to BovineMine, users can save their results as a list for further analyses by clicking on the **Save as List** button above the results table then choosing columns to save in their list.  See the lists section for more detail on creating and saving lists.  Note the "Trail: Query" text at the upper left of the results table. Clicking on the "Query" link will bring you back to the query that generated the table to allow for edits without having to start with a new template. 

 .. figure:: images/Gene-homolog-template-results.png
   :width: 696
   :alt: Gene --> Homologue results
   :figclass: align-center

   Example: Gene --> Homologue template search results, identifier for Gene GSTM1

   ..

Generate query code
-------------------
The code for each template query can be retrieved by clicking on the arrow next to **Generate Python Code** and choosing the desired language from the pull-down menu. The language options are Python, Perl, Java, Ruby, JavaScript, and XML.

 .. figure:: images/Gene-homolog-template-save.png
   :width: 496
   :alt: Gene --> Generate code pull-down menu
   :figclass: align-center


   Options for generating code from template query

   ..

Download results
----------------
The search results from a template query can be downloaded by clicking the **Export** button above the table and choosing the desired format from the pull-down menu to the right of the File name field. Available formats are tab-separated values, comma-separated values, XML, and JSON. When the results contain genomic features, they may also be downloaded in FASTA, GFF3, or BED format. Other options may be specified in the submenu to the left of the download box. By default, all rows and all columns are downloaded, but individual columns may be included or excluded by clicking on the toggles next to the column headers in the **All Columns** submenu. The number of rows and row offset are set in the **All Rows** submenu. Download the results as a compressed file by choosing GZIP or ZIP format in the **Compression** submenu (default is **No Compression**). Column headers are not added by default but may be included under the **Column Headers** submenu. Finally, the **Preview** submenu displays the first three rows of the file to be downloaded so that the desired format and options may be finalized before beginning the download. When ready, click the **Download file** button to download the results.


 .. figure:: images/Gene-homolog-template-export.png
   :width: 496
   :alt: template download results
   :figclass: align-center

   Options for downloading results from template query

   ..

.. _Customize output:

Customize output and manage columns
-----------------------------------

To customize the results table layout, click the **Manage Columns** button.  This allows users to rearrange, remove or order columns.  Filters can be edited or removed by clicking the **Manage Filters** button.  To specify the entity relationships within the query and change the way the results are presented in the table, click **Manage Relationships**.  Clicking on the **Manage Relationships** option bring also brings up a blue information panel ("What does this do?") that provides more detailed information.

 .. figure:: images/Gene-homolog-template-customize.png
   :width: 696
   :alt: customize results table
   :figclass: align-center

   Options for customizing the results of a template query.

   ..


To further manage column data, each column has a set of icons in its header.  Mousing over any icon will reveal what it does. The sort icon resembles two triangles and allows you to sort a column in either direction (ascending/descending; a->z, z->a).  To delete any column from your table, click on the "x" icon.  Alternatively, the three dots "..." can be selected to "Toggle column visibility" and hide the column.  Once hidden, the icon turns into a double arrow that can be selected to expand the column into its original form.  The next icon resembling a funnel can be selected to edit or remove any currently active filters.  A summary of the data within a column can be viewed by clicking on the icon that resembles a graph.  The data within each summary can be selected for further filtering or downloading.

 .. figure:: images/Gene-homolog-template-results-ManageColumns.png
   :width: 696
   :alt: customize results table
   :figclass: align-center


   Column header icons available to edit the results of a template query.

   ..


Optional filters
----------------

Some templates have optional filters that are disabled by default. For the Gene --> Homologue query, there is an optional filter to specify the organism used in the query.  To enable the filter, click **ON** below the **Organism > Short Name** label.

 .. figure:: images/Gene-homolog-template-option.png
   :width: 696
   :alt: template query option
   :figclass: align-center

   Using the optional organism filter in the Gene --> Homologue query template.

   ..

QueryBuilder
~~~~~~~~~~~~

The provided templates are suitable for many different types of searches, new queries may be built from scratch using the **QueryBuilder**. The possibilities of queries using the QueryBuilder are endless. The output may be formatted exactly as desired, and the query constraints may be chosen to perform complex search operations.


 .. figure:: images/query-builder-home.png
   :width: 696
   :alt: template query option
   :figclass: align-center
 

To begin, select a **Data Type**. For example, select **Gene** as a Data Type then click the **Select** button to be taken to the Model browser. 

 .. figure:: images/query-builder-select-gene.png
   :width: 696
   :alt: template query gene select
   :figclass: align-center
   
   Selecting data type as **Gene** in QueryBuilder.
   
   ..


Model browser
-------------
After selecting a data type, the **Model builder** appears displaying the attributes for the chosen feature class **Gene**.

First lets select **Gene** as a Data Type in the QueryBuilder. Then click on **Select**. This will take you to a Model browser where you can select the attributes for the feature class ‘Gene’, which you would want to be shown in your results.


 .. figure:: images/query-builder-browser.png
   :width: 696
   :alt: Model browser for query builder
   :figclass: align-center

   Model browser with "Gene" selected as the data type.
   
    ..

QueryBuilder Examples
---------------------

The following three examples provide details as to how to use the QueryBuilder using "Gene" as the selected data type.


Example 1:  Querying for protein coding genes
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

In the Model browser, click **Show** next to **Biotype**, **Gene ID** and **Symbol**, which will add these fields to the query.  Notice that these two fields appear below the data type **Gene** in the Query Overview section.

 .. figure:: images/model-browser-eg1-select.png
   :width: 696
   :alt: Model browser eg1, step1 select
   :figclass: align-center

   Model browser with "Gene" selected as the data type.
   
   Example 1, Step 1: Select fields to be added to the query   

    ..

Then click **Constrain** next to **Biotype**. The first drop-down menu defaults to `=` (equals sign). In the second drop-down menu, select **Protein Coding**, then click the **Add to query** button. This adds a constraint to the query to search only for protein coding genes. Notice that the Query Overview section now shows "Biotype = Protein Coding". Also, two types of icons appear next to the attributes. Clicking on the red "X" icon next to an attribute will remove that field or constraint from the query. Clicking on the blue pencil icon next to a constraint brings up the constraint editing window where changes may be made to the query filters.



 .. figure:: images/model-browser-eg1-constrain.png
   :width: 696
   :alt: Query Builder for Gene showing attributes and constrained by status 'Protein Coding'
   :figclass: align-center

   Example 1, Step 2 Adding a constraint to the query on Biotype.

   ..   


 .. figure:: images/model-browser-eg1-with-contraint.png
   :width: 696
   :alt: Query Builder for Gene showing attributes with contraint 'Protein Coding'
   :figclass: align-center

   Example 1, Step 2  Constraint has been added to the query on Biotype.

   ..   

Lastly, click on **Show Results** above the Model Browser.  The resulting table contains all protein coding genes in the database, with Gene ID, Gene Symbol and Gene Biotype as the table columns.  Because the Biotypes should all be the same (protein coding), that column can be deleted by clicking the "x" above it. Alternatively, the three dots "..." can be selected to "Toggle column visibility" and hide the column.  See the :ref:`Customize output` section to review ways to manage column data.

 .. figure:: images/model-browser-eg1-results.png
   :width: 696
   :alt: Query Builder for Gene showing attributes results eg.1
   :figclass: align-center

   Example 1, Step 3 Display query results.

   ..



Example 2:  Querying for protein coding genes on a particular chromosome
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Users can customize the previously run query by adding another constraint for **Chromosome**.  Note the "Trail: Query" text at the upper left of the results table. Clicking on the "Query" link will bring you back to the query that generated the table to allow for edits without having to build a new query.  In the Model browser, click on the "+" (plus sign) next to the Chromosome feature class to display its attributes.


 .. figure:: images/query-builder-eg2-chromosome-constraint.png
   :width: 396
   :alt: Adding an additional constraint for Chromosome name
   :figclass: align-center

   Example 2, Step 1 View attributes of Chromosome feature class

   ..


Next click on the  **Chromosome ID** attribute and in the text box of the pop-up window select "=" (equals).  Enter **NC_019465.1** then click on **Add to Query**, which adds the additional constraint to the query.


 .. figure:: images/query-builder-eg2-add-chrom-constraint.png
   :width: 696
   :alt: Browser after adding an additional constraint for Chromosome name
   :figclass: align-center

   Example 2, Step 2 Adding a constraint to the Chromosome ID

   ..


Click on **Show results** and the query will result in all protein-coding genes on the Chromosome with constrained ID.  Note that the number of results has been reduced with the addition of the constraint.

 .. figure:: images/query-builder-eg2-chromosome-constraint-results.png
   :width: 696
   :alt: Results after additional constraint for Chromosome name
   :figclass: align-center

   Example 2, Step 3 Result table after constraining by Chromosome ID

   ..



Example 3: Querying for Protein Coding genes on a particular chromosome and their exons
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

This last example builds upon the previous queries to display all exons for each gene on a particular chromosome.  Again, note the "Trail: Query" text at the upper left of the results table. Clicking on the "Query" link will bring you back to the query that generated the table to allow for edits without having to build a new query.  Scroll down to **Exon** feature class and select the "+" (plus sign) next to Exons to display its attributes.  Click **Show** next to **Length** and **Exon Identifier**.


 .. figure:: images/query-builder-eg3-exon-constraint.png
   :width: 696
   :alt: Results after additional constraint for exon
   :figclass: align-center

   Example 3, Step 1 Expand exon attributes and add fields to the query

   ..


The Query Overview shows the query in progress with the selected fields. Also notice that a third type of icon, a blue square, appears next to some attributes. Clicking on a blue square icon brings up a window where the query Join Style may be modified. When adding a constraint, you can decide whether you want to show only those results with the information (genes with exons) or all results and the constrained feature if it exists (e.g., all genes and indicate exons if they exist).  Click on the blue square icon next to **Exon collection** to bring up the Switch Join Style window. The default option is to show only Genes if they have a exon (inner join). Change this to **Show all Genes and show Exons if they are present** (outer join) then click **Add to query**.

 .. figure:: images/query-builder-eg3-exon-constraint-join.png
   :width: 396
   :alt: Selecting join constraint for exon
   :figclass: align-center

   Example 3, Step 2 Select join style for exons

   ..

Then click "Show results" to run the new query.


 .. figure:: images/query-builder-eg3-exon-constraint-join-results.png
   :width: 796
   :alt: exon Join window results
   :figclass: align-center

   Example 3, Step 3 Query results with exon constraint

   ..

The results table now lists a new column **Gene Exons**, which we added to the query.  If we look at the second row in the table, it lists 7 exons.  Click on the **7 exons** link to expand that entry.  That column now has additional rows containing the **Exon identifier** and **Length** for each of the 7 exons.

 .. figure:: images/query-builder-eg3-exon-expand-length.png
   :width: 796
   :alt: exon expand results
   :figclass: align-center

   Example 3, Step 4 Query results with exon column expanded

   ..

In changing the join style to an outer join, the exons have been grouped together by gene making it easier to determine how many exons are contained in each gene. If the same query is run with the default join (outer join) of **Show only Genes if they have an Exon**, the results table adds a new row for each new exon rather than grouping exons by gene.

 .. figure:: images/query-builder-eg3-exon-constraint-alt-join-results.png
   :width: 796
   :alt: exon default join results
   :figclass: align-center

   Example 3, Step 5 Query results with default join style run for genes containing exons

   ..
