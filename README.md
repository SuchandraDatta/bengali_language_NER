<h3>Bengali Language NER</h3>
<br/>
Fine-tuning bert-base-multilingual-cased on Wikiann dataset for performing NER on Bengali language.
<br/>
<ul>
  <li>Model checkpoint initially selected as mbert uncased</li>
  <li>Using mbert uncased, the words passed to encode and the output from decode doesn't match (changed spelling)</li>
  <li>The spelling of words gets changed, due to normalization issues in mbert uncased, so the correct one is mbert uncased 
  <br/>refer<a href="https://github.com/google-research/bert/blob/master/multilingual.md"> https://github.com/google-research/bert/blob/master/multilingual.md</a></li>
</ul>
<h3>Results</h3>

| Name | Overall F1 | LOC F1 | ORG F1 | PER F1 |
| ---- | -------- | ----- | ---- | ---- |
| Train set | 0.997927 | 0.998246 | 0.996613 | 0.998769 |
| Validation set | 0.970187 | 0.969212 | 0.956831 | 0.982079 |
| Test set | 0.9673011 | 0.967120 |  0.963614 | 0.970938 |


Available at https://huggingface.co/Suchandra/bengali_language_NER 

![Untitled](https://user-images.githubusercontent.com/41965125/149657973-2dd50fbb-257f-448b-a592-db2f991b5684.png)
