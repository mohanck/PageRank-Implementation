# PageRank-Implementation

0) ant clean; ant\n
1)hadoop dfs -mkdir input\n
2)hadoop dfs -put PageRankDataGenerator/pagerank5000g50.input.0 input\n
3)hadoop jar dist/HadoopPageRankMooc.jar indiana.cgl.hadoop.pagerank.HadoopPageRank input output 5000 1\n
4)hadoop dfs -cat output/part-r-00000\n

Usge: hadoop jar dist/HadoopPageRankMooc.jar [inputDir][outputDir][numUrls][number of iterations]
