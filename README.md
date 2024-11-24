This report provides a systematic analysis of the **Smart Health Advisory System** using the **Software Development Life Cycle (SDLC)**, including verification of each phase to ensure the project adheres to standard practices and meets user requirements. ![](Aspose.Words.e82a6ad3-3ab1-47f7-9f47-21c8ddea358f.001.png)

1. Project Overview

**Smart Health Monitoring and Advisory System** is a Java-based GUI application designed to calculate key health metrics such as **Body Mass Index (BMI)**, **Basal Metabolic Rate (BMR)**, **calorie requirements** and macronutrient recommendations (protein, fats, carbohydrates). Based on these metrics, it provides personalized health advice to users. This system leverages the SDLC methodology to ensure a structured, efficient, and user-centered development process. ![](Aspose.Words.e82a6ad3-3ab1-47f7-9f47-21c8ddea358f.002.png)

2. SDLC Phases with Verified Implementation 

Phase 1: Planning


Objective Verification:

The project aims to provide an easy-to-use tool for calculating health metrics. This aligns with the need for accessible health advice. 

Verified Target Audience: 

Individuals seeking fitness advice with no prior technical expertise. 

Verified Goals: 

Provide an accurate health metric calculator. 

Display results in a clear and user-friendly format.

Ensure robustness against incorrect inputs. 

Outcome:
The planning stage successfully defined measurable and achievable objectives.

Phase 2: Requirement Analysis 

Functional Requirements: 

1. Input height, weight, age, gender, and activity level.
 
2. Calculate BMI, BMR, daily caloric requirements, and macronutrient needs.
 
3. Provide health advice based on BMI.
 
Non-Functional Requirements: 

1. The system should be responsive and easy to use.
 
2. Ensure accurate and efficient calculations.
 
3. Compatible with modern operating systems (Windows, macOS).

 
Constraints: 

Input values must be within a valid range to ensure accuracy. 
Users must be at least 18 years old.

Phase 3: System Design 

Architecture: 

The application follows a modular design to separate input handling, processing, and output generation. 

Components: 

1. Input Panel:
 
Fields for height, weight, age, gender, and activity level. 

2.Processing Logic:

Algorithms for BMI, BMR, and macronutrient calculations. 

3.Output Panel: 

Displays results and recommendations. 

UI Design Verified: 

Color Scheme: The professional mix of blue and white ensures readability.

Font Choices: Arial fonts provide a clean and modern look. 

Layout: Logical arrangement of inputs and results enhances user interaction. 

Outcome: The design ensures both functionality and a polished user experience.



Phase 4: Implementation 

Implemented in Java using Swing for GUI.

Key Features: 

1.BMI Calculation:  

  BMI = Weight(kg) / Height(m)2. 

2.BMR Calculation: 

 Male: 88.362 + (13.397 X Weight) + (4.799 X Height) – (5.677 X Age). 
 
 Female: 447.593 + (9.247 X Weight) + (3.098 X Height) – (4.330 X Age).  

Activity Level Multipliers: 

Calories adjusted based on user- selected activity level. 

Figure 4: 
Code Structure of the Application 

Modern look-and-feel achieved with the Nimbus theme. 

Encapsulation of logic within the calculateHealth() method ensures maintainability. 

3.Daily Calories: Adjusted BMR based on activity level. 

4.Macronutrients: 

Protein: 0.8 X Weight (kg) 

Fats: 25% of daily calories ÷ 9. 

Carbs: 45% of daily calories ÷ 4. 

5.Suggestion Logic: 

Underweight: "Increase nutritious food intake." 

Healthy: "Maintain current lifestyle." 

Overweight: "Reduce calorie intake and exercise." 

Obese: "Seek medical advice." 

Underweight: "Increase nutritious food intake." 

Healthy: "Maintain current lifestyle." 

Overweight: "Reduce calorie intake and exercise." 

Obese: "Seek medical advice."


Phase 5: Testing

Test Plan: 

1. Input various combinations of height, weight, age, and activity levels.
 
2. Validate results against manual calculations.
 
3. Ensure meaningful suggestions for all BMI ranges.

  
Testing Results: 

|Test Case|Input(Height,Weight,Age,Gender,Activity)|Expected Output|Actual Output|Status|

|TC1|170, 70, 25, Male,Moderately Active|BMI: 24.22,Healthy BMI|Same|Pass|

|TC2|160, 45, 30, Female, Sedentary |BMI: 17.58, Underweight|Same|Pass|

|TC3|180, 85, 40, Male, Very Active |BMI: 26.23, Overweight |Same|Pass|


Phase 6: Deployment 

Platform: 
The application was packaged into an executable **JAR file** for deployment on systems with a Java runtime environment. 

User Guide: 

1.Launch the application by double-clicking the JAR file. 

2.Enter your height (in cm), weight (in kg), age, gender, and activity                       level. 

3.Click the "Calculate" button to view results and suggestions.

Phase 7: Maintenance 

Regular updates will address: 

1. Enhancements to calculation formulas based on the latest health guidelines.
  
2. Additional features like goal setting (weight gain/loss).
 
3. Bug fixes based on user feedback.
 
4. Figures:
   
System Architecture Diagram:

                           |User Input Panel|
                           
          |Height|Weight|Age|Gender|Activity Level Dropdown |
          
                                   |                                                                                    v 
                                   
                          |Processing Module|
                          
   |BMI Calculation|BMR Calculation|Caloric Needs and Suggestions|
   
                                   |                                                                                    v 
                                   
                            |Output Display|
                            
               |BMI, BMR, Calories, Macros Health Advice|
               

UI Mockup: 

                |Smart Health Monitoring and Advisory System|
                
     |[Height] [Weight] [Age] [Gender Dropdown] [Activity Level Dropdown]|
     
                             |[Calculate] |
                             
                          |[Result Display] |

5.Conclusion->

Smart Health Monitoring and Advisory System successfully combines user- friendly design with scientifically backed calculations to provide personalized health insights. Using the SDLC methodology ensured a systematic approach to development, from requirement analysis to implementation and testing. Future iterations may incorporate additional features, such as diet plans or exercise recommendations. 

EXAMPLE OF THE PROJECT:

Input: 


Height: 170 cm 

Weight: 70 kg 

Age: 25 years 

Gender: Male 

Activity Level: Moderately Active 


Output:

BMI: 24.22 

BMR: 1696.00    

Calories needed per day: 2628.80   

Protein: 56.00 g/day 

Carbohydrates: 295.80 g/day 

Fats: 73.02 g/day                                                                   Suggestion:  You are in a healthy weight range. Maintain your current lifestyle! 
