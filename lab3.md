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
example 3:
```
```
```
```
                
