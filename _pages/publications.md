---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
pubs:
  - author: "Jingjing Chen, **Liangming Pan**, Zhipeng Wei, Xiang Wang, Chong-Wah Ngo, Tat-Seng Chua"
    title: "Zero-shot Ingredient Recognition by Multi-Relational Graph Convolutional Network"
    keywords: "AAAI20"
    month: "February"
    year: "2020"
    booktitle: "*The 34th AAAI Conference on Artificial Intelligence* **(AAAI 2020)**"
    address: "New York, USA"
    url: "/publications/AAAA20_Paper.pdf"

  - author: "**Liangming Pan**, Wenqiang Lei, Tat-Seng Chua, Min-Yan Kan"
    title: "Recent Advances in Neural Question Generation"
    keywords: "QG_survey"
    year: "2019"
    booktitle: "arXiv preprint"
    url: "https://arxiv.org/abs/1905.08949"

  - author: "Yahui An, **Liangming Pan**, Min-Yen Kan, Qiang Dong, and Yan Fu (Corresponding Author)"
    title: "Resource Mention Extraction for MOOC Discussion Forums"
    keywords: "IEEE_Access19"
    journal: "IEEE Access 7 (2019): 87887-87900"
    type: "Journal"
    year: "2019"
    url: "/publications/IEEE_Access.pdf"

  - author: "Jifan Yu, **Liangming Pan**, Juanzi Li, and Xiaoping Du"
    title: "Predicting Concept-based Research Trends with Rhetorical Framing"
    keywords: "CCKS18"
    month: "August"
    year: "2018"
    booktitle: "*The 3th China Conference on Knowledge Graph and Semantic Computing* **(CCKS 2018)**"
    address: "Tianjin, China"
    url: "/publications/CCKS18_Paper.pdf"

  - author: "**Liangming Pan**, Xiaochen Wang, Chengjiang Li, Juanzi Li, and Jie Tang"
    title: "Course Concept Extraction in MOOCs via Embedding-Based Graph Propagation"
    keywords: "IJCNLP17"
    month: "December"
    year: "2017"
    booktitle: "*The 8th International Joint Conference on Natural Language Processing* **(IJCNLP 2017)**"
    address: "Taipei, Taiwan"
    pages: " Pages 875--884"
    url: "/publications/IJCNLP17_Paper.pdf"
    slides: "/publications/IJCNLP17_Slides.pdf"

  - author: "**Liangming Pan**, Chengjiang Li, Juanzi Li, and Jie Tang"
    title: "Prerequisite Relation Learning for Concepts in MOOCs"
    keywords: "ACL17"
    month: "July"
    year: "2017"
    address: "Vancouver, Canada"
    booktitle: "*The 55th Annual Meeting of the Association for Computational Linguistics* **(ACL 2017)**"
    pages: " Pages 1447--1456"
    url: "/publications/ACL17_Paper.pdf"
    slides: "/publications/ACL17_Slides.pdf"

  - author: "**Liangming Pan**, Zhigang Wang, Juanzi Li and Jie Tang"
    title: "Domain Specific Cross-Lingual Knowledge Linking Based on Similarity Flooding"
    keywords: "KSEM16"
    month: "October"
    year: "2016"
    address: "Passau, Germany"
    booktitle: "*The 9th International Conference on Knowledge Science, Engineering and Management* **(KSEM 2016)**"
    pages: "Pages 426--438"
    url: "/publications/KSEM16_Paper.pdf"
    slides: "/publications/KSEM16_Slides.pdf"

  - author: "Yan Zhang, Hailong Jin, **Liangming Pan** and Juanzi Li"
    title: "RiMOM results for OAEI 2016"
    keywords: "OAEI16"
    month: "October"
    year: "2016"
    address: "Kobe, Japan"
    booktitle: "*The 11th International Workshop on Ontology Matching co-located with the 15th International Semantic Web Conference* **(OM@ISWC 2016)**"
    pages: "Pages 210--216"
    url: "/publications/OAEI16_Paper.pdf"

  - author: "Zhigang Wang, **Liangming Pan**, Juanzi Li, Shuangjie Li, Mingyang Li and Jie Tang"
    title: "Boosting to Build a Large-Scale Cross-Lingual Ontology"
    keywords: "CCKS2016"
    month: "September"
    year: "2016"
    address: "Beijing, China"
    booktitle: "*The 1th China Conference on Knowledge Graph and Semantic Computing* **(CCKS 2016)**"
    pages: "Pages 41--53"
    url: "/publications/CCKS16_Paper.pdf"
    slides: "/publications/CCKS16_Slides.pdf"

  - author: "王巍巍, 王志刚, **潘亮铭**, 刘阳, 张江涛"
    title: "双语影视知识图谱的构建研究"
    keywords: "BMKG"
    journal: "北京大学学报(自然科学版)"
    type: "Journal"
    number: "1"
    pages: "25--34"
    volume: "52"
    year: "2016"
    month: "January"
    url: "/publications/BMKG_Paper.pdf"
    hidden: "True"

time:
  - year: "2020"
    name: "2020"

  - year: "2019"
    name: "2019"

  - year: "2018"
    name: "2018"

  - year: "2017"
    name: "2017"

  - year: "2016"
    name: "2016 and Before"
---

<!-- # Publications
<hr>
## Selected Publications -->

{% for year in page.time %}
### {{year.name}}
{% for pub in page.pubs %}
{% if pub.year == year.year %}
{% unless pub.hidden %}
  - {% if pub.url %} [{{pub.title}}]({{pub.url}}).
    {% else %} {{pub.title}}
    {% endif %}{% if pub.type %}({{pub.type}})
    {% endif %}<br>
    {{pub.author}}<br>
    {{pub.booktitle}}{{pub.school}}{{pub.journal}}<br>
    {% if pub.month %}
    {% if pub.pages %} {{pub.pages}}. {% endif %} 
    {% if pub.address %}{{pub.address}}.
    {% endif %} {{pub.month}}, {{pub.year}}.
    {% endif %}<br>
    {% if pub.url %}[[Paper]]({{pub.url}}).{% endif %}
    {% if pub.slides %}[[Slides]]({{pub.slides}}).{% endif %}
    {% if pub.key %}[Bibtex](http://groups.csail.mit.edu/commit/bibtex.cgi?key={{pub.key}}).
    {% endif %}{% if pub.bibtex %}[Bibtex]({{pub.bibtex}}).
    {% endif %}
{% endunless %}
{% endif %}
{% endfor %}
{% endfor %}


<!-- ---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}

---
layout: page
permalink: /publications/index.html
title: Publications -->
