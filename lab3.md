example 1:
```
(base) chenxiaojie@chenxiaojiedeMacBook-Air technical % grep -l "bar" 911report/*
911report/chapter-1.txt
911report/chapter-11.txt
911report/chapter-12.txt
911report/chapter-13.1.txt
911report/chapter-13.2.txt
911report/chapter-13.3.txt
911report/chapter-13.4.txt
911report/chapter-13.5.txt
911report/chapter-2.txt
911report/chapter-3.txt
911report/chapter-5.txt
911report/chapter-6.txt
911report/chapter-7.txt
911report/chapter-8.txt
```
```
(base) chenxiaojie@chenxiaojiedeMacBook-Air technical % grep -l "interesting" 911report/*
911report/chapter-11.txt
911report/chapter-13.5.txt
911report/chapter-3.txt
```
-l option: This option stands for "files with matches" and causes grep to print only the names of the files that contain the pattern. For example, if you want to find all files in the current directory that contain the word "bar," you can use the following command: grep -l "bar" *.

example 2:
```
(base) chenxiaojie@chenxiaojiedeMacBook-Air technical % grep -i "CLINICAL" biomed/1468-6708-3-1.txt
        decreased mortality. Clinical trials powered to detect
        whom risk factors, subclinical disease, and morbidity are
          baseline. Clinical covariates include hypertension,
        significantly greater than zero. A clinical trial of a
          Implications for clinical trials
          YHL, but not YOL. Clinical trials of weight modification
          found for underweight older adults. Clinical trials whose
          outcome measure. Both YOL and YHL would be clinically
        YHL as the outcome measure in clinical trials involving
```
```
(base) chenxiaojie@chenxiaojiedeMacBook-Air technical % grep -i "millennium" 911report/chapter-11.txt   
                controls, and flown the aircraft into the sea. After the 1999-2000 millennium
                2000, as part of a millennium after-action review. President Clinton and his
                millennium alert.
            The Millennium Exception
                with terrorism-the last weeks of December 1999 preceding the millennium.
                millennium and possible computer programming glitches ("Y2K") that might obliterate
            After the millennium alert, the government relaxed. Counterterrorism went back to
                millennium phenomenon was not repeated. FBI field offices apparently saw no abnormal
```
grep -i: This option enables case-insensitive searching. By default, grep is case-sensitive, meaning that it distinguishes between uppercase and lowercase letters. However, if you use the -i option, grep will treat all letters as if they were lowercase, allowing you to find matches regardless of the case of the letters. For example, the command grep -i "apple" fruits.txt will find all instances of "apple" in the fruits.txt file, regardless of whether it is capitalized or not.

example 3:
```
(base) chenxiaojie@chenxiaojiedeMacBook-Air technical % grep -v "a" biomed/1468-6708-3-1.txt   

  
    
      
        Introduction
        elderly [ 9 ] .
      
      
        
          Study
        
        
        
        
          ] .
          (for persons who were never in excellent, very good, or
          report results using only the simpler definition.
          findings.
        
        
        
        
        
      
      
        Results
        likely.
        from 25 to 29.9. The second column, which shows results
        under 20.
        groups.
        YOL or YHL.
      
      
        Discussion
        
        
        
          YHL.
        
        
        
      
      
        Conclusion
        'overweight' by the NHLBI guidelines. This suggests using
      
      
        Competing interests
      
      
        CESD Center for Epidemiologic Studies Depression
        poor?
      
    

```
```
(base) chenxiaojie@chenxiaojiedeMacBook-Air technical % grep -v "s" biomed/1468-6708-3-1.txt   

  
    
      
        Introduction
        elderly [ 9 ] .
        they were evaluated on improved health, rather than on
      
      
        
          Study
        
        
          above.
        
        
          ] .
          throughout). Since people reported their health every 6
        
        
        
        
        
      
      
        likely.
        to age 73. For example, black women averaged 6.3 YOL, but
        were healthy.
        under 20.
        between BMI and YOL for BMI above 20. Underweight women
        averaged about .25 fewer YOL than other women (p < .05
        women and men. Women who were normal or overweight averaged
        being compared. For example, underweight women averaged
        4.50 YHL compared to 4.92 for normal women, and the common
        treatment to help underweight women achieve normal weight
        expected to have 80% power with N = (1.96+.84) 2/.29 2=
        about 93 women per treatment arm, if 7-year YHL were the
        an intervention to improve the health of underweight women
        YOL or YHL.
      
      
        
          Optimal weight and overweight
          older men and 30-35 for older women. In Figure 1, the
          quality of life into account.
        
        
          would probably not have a direct effect on either YOL or
          YHL.
          mortality.
        
        
        
      
      
      
      
        None declared
      
      
        Scale
        poor?
      
    
  
```
grep -v: This option is used to invert the match, meaning that it will print all lines that do not match the specified pattern. For example, the command grep -v "apple" fruits.txt will print all lines in the fruits.txt file that do not contain the word "apple".

example 4:
```
base) chenxiaojie@chenxiaojiedeMacBook-Air technical % grep -c "and" 911report/chapter-1.txt
243
```
```
(base) chenxiaojie@chenxiaojiedeMacBook-Air technical % grep -c "in" 911report/chapter-11.txt
553
```
grep -c: This option counts the number of matches instead of printing the matching lines. For example, the command grep -c "apple" fruits.txt will print the number of times the word "apple" appears in the fruits.txt file, without printing the actual lines that contain the word.
                