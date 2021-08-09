   Related works about QA and Rule Mining.

# Papers of KBQA:
  notes: Specifically, we focus on the task of multi-hop QA over KB.
  
1. ### SPARQA: Skeleton-Based Semantic Parsing for Complex Questions over Knowledge Bases. AAAI 2020. [code](https://github.com/nju-websoft/SPARQA)
   This paper uses bert to do many works. They split the construction task of a SPARQL language for an input natural language question into two parts. First, they decompose the complex question using four bert-based nlp models, and generate a set of subqueries. Then, they use two models to score a complete query which is a combination of the subqueries set. 
2. 






# Datasets of QA.
**We list the complex questions dataset.**
1. ### KQA Pro.[source](https://github.com/shijx12/KQAPro_Baselines).
   This dataset contains 117970 complex questions, each question has two formats, Logic form and Natural language. The target KB is wikidata. 
   
   
2. ### GraphQuestions. [source](https://pan.baidu.com/s/1N_WBCmoQIvNCk_W4oFHeKA).
   This dataset contains 5166 questions, 2558 for training and 2608 for testing. The target KB is [Freebase](https://pan.baidu.com/s/1FWwv1R_7JtO_mpk_6pL_TQ) (version June 2013). Logic Form (SPARQL) & NL.
3. ### ComplexWebQuestion. [source](https://pan.baidu.com/s/106vC73W9WKXyuuFcaoPIuQ)
   This dataset contains 34689 questions with a split of 80-10-10 for training, validation and test sets. Logic Form (SPARQL) & NL. The target KB is [Freebase](https://pan.baidu.com/s/1CCxljj_yH9S3Y4Zeh6epmw) (version 2015-08-09)


# Preliminaries.
   For the task of KBQA, as we need to fetch answers from a Knowledge Base. We always use a SPARQL to evaluate over a KB. From the begining of the task, we need to build a local KB. 
   1. Instructions for build a local KB. Most of existing works choose to use . 
