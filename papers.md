   Related works about QA and Rule Mining.

# Outline:
   Two types of solutions for multi-hop KBQA.
   
    1. natual language question -> semantic graph -> query graph (~~ SPARQL);
    
    2. entity in question -> an entity centric graph from KB -> some candidates answers -> select by embedding space.

# Papers of KBQA:
  notes: Specifically, we focus on the task of multi-hop QA over KB.
  
1. ### SPARQA: Skeleton-Based Semantic Parsing for Complex Questions over Knowledge Bases. AAAI 2020. [code](https://github.com/nju-websoft/SPARQA)
2. ### Stepwise Reasoning for Multi-Relation Question Answering over Knowledge Graph with Weak Supervision. WSDM2020
3. ### Hierarchical Query Graph Generation for Complex Question Answering over Knowledge Graph. CIKM 2020
4. ### Multi-hop Knowledge Base Question Answering with an Iterative Sequence Matching Model. ICDM 2019
5. ### A State-transition Framework to Answer Complex Questions over Knowledge Base. ALC 2018
6. ### Answering Questions with Complex Semantic Constraints en Knowledge Bases on Open KB. CIKM 2015
7. ### Improving Multi-hop Question Answering over Knowledge Graphs using Knowledge Base Embeddings. ACL 2020
----------
1. ### SPARQL QUERY GENERATION FOR COMPLEX QUESTION ANSWERING WITH BERT AND BILSTM-BASED MODEL.
   Given a complex natural language question as an input, this work first detects the template of this question. then, entity linking and relation linking, then path ranking (for the complex logic in the query triples). finally, generate a sparql query which can used execute over a kb to answer the question.
  
   Dataset: LC-QUAD 1.0 and LC-QUAD 2.0
  
2. ### Learning to Rank Query Graphs for Complex Question Answering over Knowledge Graphs. ** [code][https://github.com/AskNowQA/KrantikariQA]
   given a natural language question (complex), to get the query patterns for generating a sparql query. they generate candidate chains by enumerate all 1 and 2 hop paths around the entity of the question, and then use a bert-based model to score the paths. 
   ！！！！rule generation, and efficiency time,
   Dataset: LC-QUAD 1.0, QALD-7
  
3. ### Formal Query Building with Query Structure Prediction for Complex Question Answering over Knowledge Base.
    it argues 2[link](https://github.com/Rebaccamin/QA-rule_mining/blob/main/papers.md#:~:text=Learning-,to,-Rank%20Query%20Graphs)

# Papers of semantic graph and theoretical proof.

1. ### A Note on the Budgeted Maximization of Submodular Functions. [source](http://reports-archive.adm.cs.cmu.edu/anon/cald/CMU-CALD-05-103.pdf)
2. ### LSQ: The Linked SPARQL Queries Dataset [source](https://aidanhogan.com/docs/LSQ_ISWC2015.pdf)







# Datasets of QA.


**We list the complex questions dataset.** (the password is KBQA)
1. ### KQA Pro.[source](https://github.com/shijx12/KQAPro_Baselines).
   This dataset contains 117970 complex questions, each question has two formats, Logic form and Natural language. The target KB is wikidata. 
   
   
2. ### GraphQuestions. [source](https://pan.baidu.com/s/1N_WBCmoQIvNCk_W4oFHeKA).
   This dataset contains 5166 questions, 2558 for training and 2608 for testing. The target KB is [Freebase](https://pan.baidu.com/s/1FWwv1R_7JtO_mpk_6pL_TQ) (version June 2013). Logic Form (SPARQL) & NL.
3. ### ComplexWebQuestion. [source](https://pan.baidu.com/s/106vC73W9WKXyuuFcaoPIuQ)
   This dataset contains 34689 questions with a split of 80-10-10 for training, validation and test sets. Logic Form (SPARQL) & NL. The target KB is [Freebase](https://pan.baidu.com/s/1CCxljj_yH9S3Y4Zeh6epmw) (version 2015-08-09)

4. Lcquad1.0 which contains 5000 questions and 2.0 contains 30000 questions.

6. QALD-7


# Preliminaries.
   For the task of KBQA, as we need to fetch answers from a Knowledge Base. We always use a SPARQL to evaluate over a KB. From the begining of the task, we need to build a local KB. 
   1. Instructions for build a local KB. Most of existing works choose to use . 


# Some definitions:
   logic forms: SPARQL, -DCS
