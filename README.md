# nlp_social_robotics
Verbal communication in robotics: a review about fields of applications and trends in the last decades based on computational linguistic analysis.

Dataset:

- Data_VC_AMV contains data divided on publication years or divided in groups (Contrast analysis). The NLP tool T2K has been used to perform this analysis.

- The other three form all together the main corpus (topic mining). data_speech_robot1 has to be merged together with data_speech_robot2000 and data_speech_robot2019. R was used to perform this analysis. 

To merge together the files for the topic mining analysis, you can use these lines of code:

dat = read.csv("data_speech_robot1.csv",stringsAsFactors = FALSE)

dat_miss = read.csv("data_speech_robot_2000.csv",stringsAsFactors = FALSE)

dat_miss1 = read.csv("data_speech_robot_2019.csv",stringsAsFactors = FALSE)

dat1 <- rbind(dat,dat_miss,dat_miss1)

The R script used for the analysis can be asked by sending an e-mail to alessandro17mv@gmail.com
