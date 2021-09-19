# School_District_Analysis

## Project Overview
The purpose of this analysis is to provide statistics metrics based on the school state-testing results. The raw data was presented in two tables:

1. School data : School type, size, budget. 
2. Student data: Student ID, name, gender , grade , school name , reading and math scores.

After the first statistic results, the board notified about the evidence of academic dishonesty in one school. We decided to remove the data related to the school involved in this issue. 

## Results
In order to explain the new results obtained, we are going to address a group of questions as bullet points. For an additional precision during the analysis, all the numeric results were rounded to the nearest 10th. For all the screenshot, the original result will be displayed before the new ones. 

1. How is the district summary affected?: The values from the original results and the new one are very similar. The only parameter affected was the *Overall Passing percentage*, which decrease in 0.3%. 

   -Original results
   <p align="center"><img src="https://user-images.githubusercontent.com/88695570/133708516-fd8d6fdf-5d3d-4dee-b970-1859a43ca075.png">
    
   -New results
    <p align="center"><img src="https://user-images.githubusercontent.com/88695570/133708516-fd8d6fdf-5d3d-4dee-b970-1859a43ca075.png">

2. How is the school summary affected? The school summary was affected only on the Thomas High School section. The other school's results were not modified.  
        
3. How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

   - Math Results: To present how the Thomas High school's results were affected, the school summary was sorted descending based on the percentage of students who passed the Math evaluation (**%Passing Math**). As you can see the ranking position was modified from 6th to the 7th position.
       
        <p align="center"><img src="https://user-images.githubusercontent.com/88695570/133724675-2002b538-fa45-4522-a87e-0cb01b05cd99.png">
            
   - Reading results: Similar as the previous analysis, the reading result was impacted. Consequently, Thomas High school lost the first position. 
           
        <p align="center"><img src="https://user-images.githubusercontent.com/88695570/133724721-ab438b08-af0d-41d8-ad86-7c0654c58c02.png">
        
4. How does replacing the ninth-grade scores affect the following:

   - Math and reading scores by grade: Only the ThomaS High school's results for the 9th grade were affected. After we decided eliminated the 9th grade score for math and reading, it was expected display only **null** values for those two columns. This is the screenshot for the new results: 
           
         <p align="center"><img src="https://user-images.githubusercontent.com/88695570/133724807-4db6e651-bf05-457e-b4f9-6466653507cc.png">    
                 
   - Scores by school spending: Thomas High school belongs to the spending range of **$630-644**, which was the only section imptacted. The **%Passing Math results** was affected in 1%. The other metric data results remains the same.  
            
        - Original results:
              <p align="center"><img src="https://user-images.githubusercontent.com/88695570/133724944-5f388603-b8c0-41cd-82f3-2969652a400c.png">
                 
        - New results
              <p align="center"><img src="https://user-images.githubusercontent.com/88695570/133725012-bb7cf9b8-7c96-4e1e-840f-f797f2c95c93.png">

   - Scores by school size: Based on this screenshot from the original and new results, we can conclude that the scores based on the schools size were not impacted.
                 
        - Original results
              <p align="center"><img src="https://user-images.githubusercontent.com/88695570/133725050-f33676af-914c-4c70-aab5-6e74774f9d69.png">
      
        - New results
              <p align="center"><img src="https://user-images.githubusercontent.com/88695570/133725058-dbabacca-164c-4995-85ac-471f3ca3ee9a.png">
    
   - Scores by school type: There is a slighlty difference on the **Charter** results, to be more specific only on the **%Passing Reading** parameter. This small variation (around 0.1%) was expected considered the portion of data removed. 
                 
        - Original results
              <p align="center"><img src="https://user-images.githubusercontent.com/88695570/133725072-922cc9f5-ff81-41b1-a22e-a22c8c5683ec.png">

        - New results
              <p align="center"><img src="https://user-images.githubusercontent.com/88695570/133725090-ad83cf23-0638-4222-b0d6-41847e0ca2b9.png">

## Summary
After the Thomas High School scores were replaced with **NaN** values, some statistic parameters were affected. I will summarize those new results in 4 items:

1. #### No statistic data for 9th grade: By removing the score from the analysis the final chart does not shows any metric for the 9th grade. This could represent a potential issue for the school in the future.
                 
!<p align="center"><img src="https://user-images.githubusercontent.com/88695570/133910920-dc4de4d8-b72d-42bc-a172-de7111315f2a.png">
                 
2. #### Ranking position was affected (percentage results): This result was analyzed in a previous section (Results - 3). Removing the 9th grade socres caused an impact in the school ranking for both assignatures. 
   
3. #### Overall percentage has reduction: If we compare the original **% Overall Passing** parameter with the new results, we can identify a reduction of 0.3% (from 90.9% to 90.6%).

!<p align="center"><img src="https://user-images.githubusercontent.com/88695570/133910940-9b39ab45-eabe-4ac7-b59a-6604b7d4dbd6.png">
   
4. #### Average reading score increased: Despite of the other statistic results, the **Average reading score** has a small increment of 0.1%. It does not represent a big difference but it should be considered for analytics purposes. 

!<p align="center"><img src="https://user-images.githubusercontent.com/88695570/133910952-b22904d6-c6a2-4159-9320-0d0fec0aba84.png">
                
5. #### Total of students who passed math and reading test decreased: Before removing the 9th grade score ,the school obtained a total of 1487 students who pass both assignatures (math and reading). After the cleaning process this value decreased considerable to 1064. This measure was reflected in the **% Overall Passing** results mentioned on the item 3 in this section.
   
!<p align="center"><img src="https://user-images.githubusercontent.com/88695570/133910958-9988c94d-b264-4fd8-ba26-4770b8fd09d5.png">

  
                 
