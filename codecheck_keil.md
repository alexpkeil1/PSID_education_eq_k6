Code review (Keil)

KEY:
  P: comment pertains to potential problem
  S: suggestion, efficiency/general programming comment
  N: personal note with descriptions
  R: note to re-visit (shouldn't be any of these at the end)

Files

- README.txt
- causal_DAG_05012021.PNG
  - N: ignored this - simplified version of more recent DAG
  
- causal_DAG_05052021.PNG
  - P: Why does M0 affect nearly everything in future, but M1 does not? (this doesn't agree with code)
  - P: Why is Markov-1 (Markov-2?) assumption made? Is this out of convenience or was model fit used?
  - S: Don't do linear DAG, structure left to right in terms of time and up and down in terms of assumed order within each time point
  
- dataset_build_04302021.R
  - N: did not check for bugs. Just got basic idea of data.
  
- eq_build_021721.R
  - N: did not check for bugs. Just got basic idea of how EQ was generated.
  
- medgformula_script_05012021.R
  - N: ignored this file in favor of updated version
  
- medgformula_script_05052021.R
  
- medgformula_script_template.R
  - P: bootstrap estimates given, but where is estimate for original data?
  - S: parallel processing of bootstrap samples could save a lot of time
  - R: lime 103, pM_0a1 - is prediction interval appropriate here? 
  
- medgformula_script_template_061121.R
  - N: ignored this file. Did not find functional differences between this file and previous verion
 
- template_data.csv
  - N: used this to run sample code
