## COLD: Complex Offensive Language Dataset

If you use this dataset, please cite the following paper (BibTex below):

Alexis Palmer, Christine Carr, Melissa Robinson, and Jordan Sanders. 2020 (to appear). COLD: Annotation scheme and evaluation data set for complex offensive language in English. *Journal of Linguistics and Computational Linguistics*. 

## Overview of data

The COLD data set is intended for researchers to diagnose and assess their automatic hate speech detection systems. The corpus highlights 4 different types of complex offensive language: slurs, reclaimed slurs, adjective nominalization, distancing, and also non-offensive texts. The corpus contains a set of tweets collected from 3 different data sets: Davidson et al (2017), Waseem and Hovy (2016), and Robinson (2017). The data is annotated by 6 annotators, with each instance being annotated by at least 3 different annotators.  

Please note: There are two versions of the data set: COLD-2016, and COLD-all. 

1. **COLD-2016** is the data set used for the analyses and experimental results described in the JLCL paper. This version of the data set contains 2016 instances, selected using filters aiming to capture the complex offensive language types listed above.

2. **COLD-all**: The full COLD data set contains 2500 instances. The instances from COLDID#1 - COLDID#2152 are the original tweets, selected using filters aiming to capture the complex offensive language types listed above. Some instances originally had fewer than three annotations, and we acquired the missing annotations after having finished the work described in the paper. In addition, we randomly selected another 348 tweets from Davidson et al. (2017) to bring the total number of instances in the data set up to 2500. These instances were annotated by three of the original annotators. The randomly-selected data can be found starting with COLDID#2153.

## Format and annotations

The data are made available here as .tsv files. The format consists of eight columns: four informational and four annotation-related.

### Informational columns:

1. **COLDID** - unique number (assigned by us) for each textual instance. Since each instance has been labeled by three different annotators, there are three or more occurrences of each COLDID in the data set.

2. **Annotator** - annotator ID. The six annotators are indicated by the letters A-F.

3. **OriginalID** - information about the original data set and the textual instance's ID from the data set it was extracted from. The OriginalID includes a letter indicating which data set it originates from, followed by a hyphen and the corresponding ID of the instance in the original data set. For example: D-63 means that the instance is from the Davidson et al. (2017) data set, originally with the ID number 63.

4. **Text** - the text of the instance

### Annotation columns:

For each instance, annotators were asked to answer Yes or No to each of four questions. (See the paper for much more detailed discussion, as well as distributions, etc.)

1. **Q1:** Is this text offensive?

2. **Q2:** Is there a slur in the text?

3. **Q3:** Is there an adjectival nominalization in the text?

4. **Q4:** Is there (linguistic) distancing in the text?

## Contact
If you have any questions please contact carrc9953@gmail.com, alexis.palmer@unt.edu, or melissa.robinson@my.unt.edu.

## BibTex

```
@article{cold:2020,
  title = {COLD: Annotation scheme and evaluation data set for complex offensive language in English},
  author = {Palmer, Alexis and Carr, Christine and Robinson, Melissa and Sanders, Jordan}, 
  journal = {Journal of Linguistics and Computational Linguistics, Special Issue},
  year = {2020},
  volume={to appear},
  number={to appear},
  pages = {tbd}
}
```

## References

Davidson, T., Wamsley, D., Macy, M., & Weber, I. (2017). Automated hate speech detection and 
the problem of offensive language. In Eleventh international conference on web and 
social media. <a href="https://aaai.org/ocs/index.php/ICWSM/ICWSM17/paper/view/15665">[the paper]</a>, <a href="https://github.com/t-davidson/hate-speech-and-offensive-language">[the repository]</a>

Robinson, M. (2018). A man needs a female like a fish needs a lobotomy: The role of adjectival 
nominalization in pejorative meaning. Master's thesis, Department of Linguistics, University of North Texas.
<a href="https://digital.library.unt.edu/ark:/67531/metadc1157617/m2/1/high_res_d/ROBINSON-THESIS-2018.pdf">[the thesis]</a>

Waseem, Z., & Hovy, D. (2016). Hateful Symbols or Hateful People? Predictive Features for 
Hate Speech Detection on Twitter. In Proceedings of the NAACL Student Research Workshop. San Diego, California.
<a href="https://www.aclweb.org/anthology/N16-2013/">[the paper]</a>
