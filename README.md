# comp7607_group_project

## For replication of results - 28 November 2022
Run script in PrefixTuning.ipynb

Program files can be found at https://drive.google.com/drive/folders/1IgMrhAJ9YoCbrZBl2mgdpWRARJ-47y7d?usp=sharing

To run the program, you should:

1) Modify the file path to the Google Drive folder above
2) Connect to the Google Colaboratory Pro amd "Change Runtime" to GPU and High RAM for reproduction of similar results
3) Run the command lines until the "Default" setting "!python /content/drive/MyDrive/Colab_Notebooks/PrefixTuning-cleaned/gpt2/train_e2e.py"
4) Modify the parameters in the following command line to initiate by kaiming, xavier or random alongside other hyperparameters such as prefix length, learning rate, epochs and batch size
5) Review the metric scores by the end of the output

## 27 Oct 2022 
Below papers are suggested: (bold in reading list)

1) ACL 2021 Prefix-Tuning: Optimizing Continuous Prompts for Generation <br>
-Method/Dataset Analysis study

2) EMNLP 2021 Improving and Simplifying Pattern Exploiting Training <br>
-Method/Dataset Analysis study

3) NAACL 2021 Low-Complexity Probing via Finding Subnetworks <br>
-Model/Dataset Analysis study

4) ACL 2022 BitFit: Simple Parameter-efficient Fine-tuning for Transformer-based Masked Languagemodels <br>
-Model/Dataset Analysis study

Please state your preference on or before 28 Oct 22 8pm in group chat so that we can start on the proposal. Thanks.



-------------------------------------------------------------------------------------
# Reading list 
> Please 1) Make sure dataset is public dataset and accessible 2) Remark if code is available
## Frankie
- **ACL 2021 Prefix-Tuning: Optimizing Continuous Prompts for Generation**
    - **Model: GPT-2, BART**
    - **Dataset: Yes (total 3)**
    - **Task: prefix-tuning and fine-tuning on table-to-text generation for increasing efficiency**
- ACL 2021 SimCSE: Simple Contrastive Learning of Sentence Embeddings
    - Model: BERT
    - Dataset: Yes
    - Task: improve performance in classifying ‘entailment’ or ‘contraction’ from previous sentences using supervised/unsupervised SimCSE model
- ACL 2021 Implicit Representations of Meaning in Neural Language Models
    - Model: BART, T5transformer LM
    - Dataset: Yes (total 2)
    - Task: proving feasibility of Neural Language Models for contextual word representations
- ACL 2021 Self-Attention Networks Can Process Bounded Hierarchical Languages
    - Model: Dyck(k,D), seems no available package
    - Dataset: random dataset from HuggingFace
    - Task: proving feasibility of self-attention networks for hierarchical languages
## Eugene
- **EMNLP 2021 Improving and Simplifying Pattern Exploiting Training**
    - **Model: ADAPET (have code)**
    - **Dataset: SuperGLUE, data split as Schick and Schütze (2021b)**
    - **Task: verify ADAPET has better performance than PET**
- EMNLP 2021 ExpBERT: Representation Engineering with Natural Language
    - Model: ExpBERT (got code)
    - Dataset: 3 databset
    - Task: vertify if ExpBERT outperform other version of BERT
- **NAACL 2021 Low-Complexity Probing via Finding Subnetworks**
    - **Model: bert-base-uncased**
    - **Dataset: 1 dataset for each task (total 3)**
    - **Task: vertify if subtractive pruning-based probe is more efficient than common method**
- NAACL 2021 Reading and Acting while Blindfolded: The Need for Semantics in Text Game Agents
## Stephy
- **ACL 2022 BitFit: Simple Parameter-efficient Fine-tuning for Transformer-based Masked Languagemodels**
    - **Model: BERT(base), BERT(large), RoBERTa(base) - using Huggingface interface**
    - **Dataset: GLUE **
    - **Task: compare GLUE task performances of the below**
        **- full fine-tuning**
        **- BitFit: fine-tuning on bias parameter OR fine-tuning on partial bias parameter**
- EMNLP 2021 Generating Datasets with Pretrained Language Models
    - Model: 
        - Dataset generateion:GPT2? 
        - Performance evaluation: S-BERT(base)/ S-RoBERTa(base)
    - Dataset: original dataset is not provided, but dataset generated by DINO provided
    - Task: use DINO to create labeled datasets automatically for fine tuningm and test performance onSTS12-16, STSb, SICK task
- NAACL 2021 On the Inductive Bias of Masked Language Modeling
    - Model: 
    - Dataset: SST2 (need to label ground truth)
- ACL 2021 Modeling Fine-Grained Entity Types with Box Embeddings
