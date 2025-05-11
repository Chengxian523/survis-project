# SurVis - Visual Literature Browser

![Screenshot](/doc/survis.png)

SurVis is a flexible online browser to present and analyze scientific literature. The system is made for authors of survey articles, theses, or books who want to share their references in a user-friendly way. All you need to start is a bib file and a list of keywords for your papers.

Test SurVis with a reference literature database: http://dynamicgraphs.fbeck.com

## How To Use SurVis for Your Literature Collection

Dowload the latest SurVis release or fork this repository.

To start SurVis, open 'src/index.html' in your browser.

The bibliography data is stored in 'bib/references.bib' in BibTeX format.

Supplemental data is contained in 'src/data/':
* 'tag_categories.js': list of special tag categories; they can be used as a prefix for the tags and appear, for instance, 'a:b' refers to tag 'b' in tag category 'a'
* 'authorized_tags.js': tags that are defined through a description (highlighted in SurVis, description appears as a tooltip)
* 'search_stopwords.js': a list of stopwords used to exclude terms from search queries
* 'papers_pdf' (optional): PDF files of the papers, please use the BibTeX id as a file name
* 'papers_img' (optional): PNG thumbnails for the papers, please use the BibTeX id as a file name

Please do not edit the files in 'src/data/generated/' because they are created automatically. 

After completing your changes, just run 'update_data.py' with Python 3. Reload SurVis in the browser to see the changed bibliography. The script will continue to check for updates on the bib file until you stop it.

If the edit mode is activated, BibTeX entries can be modified in the browser, but are not stored in the 'bib' directory. To make those changes persistent, use 'download BibTex' in SurVis and copy the BibTeX data to your bib file in the 'bib' directory. You can also use the features to save and load the data from local storage of the browser; be careful, however, these features are still experimental.

Further properties of SurVis, such as the title of the page, can be modified in the file 'src/properties.js'. For the publication of your literature collection, you should usually deactivate the edit mode in the properties ('editable = false;').

Enjoy SurVis and send feedback if you like.

## Learn more

We've published a paper about SurVis at VAST 2015 - please reference it if you use or want to refer to SurVis in one of your publications. 

Beck, Fabian; Koch, Sebastian; Weiskopf, Daniel: Visual Analysis and Dissemination of Scientific Literature Collections with SurVis. In: IEEE Transactions on Visualization and Computer Graphics (2015).

* DOI: http://dx.doi.org/10.1109/TVCG.2015.2467757
* Preview video: https://vimeo.com/136206061 

## List of Literature Collections Using Survis

* Dynamic Graph Visualization - http://dynamicgraphs.fbeck.com
* Visualizing Group Structures in Graphs - http://go.visus.uni-stuttgart.de/groups-in-graphs/
* Performance Visualization - http://idav.ucdavis.edu/~ki/STAR/
* Visualization for Software Reuse - http://www.cos.ufrj.br/~schots/survis_reuse/
* Set Visualization - http://www.cvast.tuwien.ac.at/~alsallakh/SetViz/literature/www/index.html
* Visualizing High-Dimensional Data - http://www.sci.utah.edu/~shusenl/highDimSurvey/website/

Please contact me (fabian.beck@visus.uni-stuttgart.de) if you know other collections using SurVis.

## Contact

Fabian Beck

VISUS, University of Stuttgart

fabian.beck@visus.uni-stuttgart.de

http://research.fbeck.com





# SurVis -视觉文学浏览器

(截图)! (/ doc / survis.png)

SurVis是一个灵活的在线浏览器，用于呈现和分析科学文献。该系统是为想要以用户友好的方式分享参考文献的调查文章、论文或书籍的作者而设计的。你所需要的只是一个号码布文件和一份论文关键词列表。

测试SurVis与参考文献数据库：http://dynamicgraphs.fbeck.com

如何在你的文学收藏中使用SurVis

下载最新的SurVis版本或派生此存储库。

要启动SurVis，在浏览器中打开‘src/index.html’。

参考书目数据存储在‘bib/references ’中。BibTeX格式的bib。

补充数据包含在‘src/data/’中：

‘tag_categories.js’：特殊标签类别列表；它们可以用作标签的前缀并出现，例如，‘a:b’表示标签类别‘a’中的标签‘b’
‘authorized_tags.js’：通过描述定义的标签（在SurVis中突出显示，描述显示为工具提示）
‘search_stopwords.js’：一个停止词列表，用于从搜索查询中排除术语
* 'papers_pdf'（可选）：论文的PDF文件，请使用BibTeX id作为文件名
* 'papers_img'（可选）：论文的PNG缩略图，请使用BibTeX id作为文件名

请不要编辑‘src/data/generated/’目录下的文件，因为它们是自动创建的。

完成更改后，只需使用Python 3运行‘update_data.py’。在浏览器中重新加载SurVis以查看更改后的参考书目。该脚本将继续检查bib文件上的更新，直到您停止它。

如果激活了编辑模式，则可以在浏览器中修改BibTeX条目，但不存储在‘bib’目录中。要使这些更改持久，在SurVis中使用‘download BibTex’并将BibTex数据复制到‘bib’目录下的bib文件中。您还可以使用这些功能从浏览器的本地存储中保存和加载数据；但是要小心，这些功能还处于实验阶段。

SurVis的其他属性，比如页面的标题，可以在‘src/properties.js’文件中修改。对于文献集的出版，通常应该在属性（'editable = false;'）中禁用编辑模式。

享受SurVis，并发送反馈，如果你喜欢。

##了解更多

我们在VAST 2015上发表了一篇关于SurVis的论文-如果您在您的出版物中使用或想要引用SurVis，请参考它。

贝克,费边;科赫,塞巴斯蒂安;Daniel Weiskopf：《科学文献集合的可视化分析与传播》。见：IEEE可视化与计算机图形学汇刊（2015）。

* DOI: http://dx.doi.org/10.1109/TVCG.2015.2467757
*预览视频：https://vimeo.com/136206061

使用Survis的文学收藏列表

*动态图形可视化- http://dynamicgraphs.fbeck.com
*在图形中可视化组结构- http://go.visus.uni-stuttgart.de/groups-in-graphs/
*性能可视化- http://idav.ucdavis.edu/~ki/STAR/
*可视化软件重用- http://www.cos.ufrj.br/~schots/survis_reuse/
*设置可视化- http://www.cvast.tuwien.ac.at/~alsallakh/SetViz/literature/www/index.html
*可视化高维数据- http://www.sci.utah.edu/~shusenl/highDimSurvey/website/

如果您知道其他使用SurVis的集合，请联系我（fabian.beck@visus.uni-stuttgart.de）。

# #联系

费边贝克

VISUS，斯图加特大学

fabian.beck@visus.uni-stuttgart.de

http://research.fbeck.com



参考网页：http://dynamicgraphs.fbeck.com/
