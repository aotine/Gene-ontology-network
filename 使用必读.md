# Gene-ontology-network

#文章来源(Nat Neurosci):
链接：https://pubmed.ncbi.nlm.nih.gov/31061494/  OR  https://www.nature.com/articles/s41593-019-0393-4
Van Hove, H., Martens, L., Scheyltjens, I. et al. A single-cell atlas of mouse brain macrophages reveals unique transcriptional identities shaped by ontogeny and tissue environment. Nat Neurosci 22, 1021–1035 (2019). https://doi.org/10.1038/s41593-019-0393-4

其中作出了一张Gene-ontology-network图：
![41593_2019_393_Fig4_HTML](https://user-images.githubusercontent.com/58368896/156860968-d912c793-44f8-49a3-9fdd-07a226095cda.png)

完成使用的工具：
Rstuido cyotoscape AI

代码主要注意事项：

1.先装bioconductor包中的simplifyEnrichment包：
https://www.bioconductor.org/packages/release/bioc/html/simplifyEnrichment.html

2.再运行代码，中间如果出现错误：
package or namespace load failed for ‘XXX’ in loadNamespace(i, c(lib.loc, .libPaths()), versionCheck = vI[[i]]):
不存在叫‘XX’这个名字的程辑包：
就用步骤1中的方法装好包重启RStudio

3.代码运行完毕得到df.txt\net.tet,用cyotoscape导入，方法是File-import-Network from file，接下来步骤是cytoscape常用方法

4.完成调整图形后可以导出pdf，通过AI再进行调整绘图。
