<h3>Bengali Language NER</h3>
<br/>
Fine-tuning bert-base-multilingual-cased on Wikiann dataset for performing NER on Bengali language.
<br/>
<h5>Model available on Huggingface Model Hub at https://huggingface.co/Suchandra/bengali_language_NER  </h5>
<ul>
  <li>Model checkpoint initially selected as mbert uncased</li>
  <li>Using mbert uncased, the words passed to encode and the output from decode doesn't match (changed spelling)</li>
  <li>This is due to normalization issues in mbert uncased, so the correct one is mbert cased 
  <br/>refer<a href="https://github.com/google-research/bert/blob/master/multilingual.md"> https://github.com/google-research/bert/blob/master/multilingual.md</a></li>
</ul>
<h3>Results</h3>

| Name | Overall F1 | LOC F1 | ORG F1 | PER F1 |
| ---- | -------- | ----- | ---- | ---- |
| Train set | 0.997927 | 0.998246 | 0.996613 | 0.998769 |
| Validation set | 0.970187 | 0.969212 | 0.956831 | 0.982079 |
| Test set | 0.9673011 | 0.967120 |  0.963614 | 0.970938 |

![pic_hugginggface](https://user-images.githubusercontent.com/41965125/163574848-1941d84a-8a79-468a-9616-c404def73301.png)

![Untitled](https://user-images.githubusercontent.com/41965125/149658411-ce096279-ccc9-46a3-b4f3-aa0bafc6bf14.png)
