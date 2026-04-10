# LabReport01- [C program to input the number of days and convert it into years, months, and days]
## STudent Information
Name:Tasmim Jannat
ID:26002159
Course:BSC in CSE

## Experiment Title
Converting a number into years,monthsand days.

## Objective
1.	To design and implement a C program that processes a single integer input representing a total count of days.  
2.	To apply arithmetic operators (division and modulus) to decompose a large unit of time into sub-units (years and months).  
3.	To demonstrate the practical use of integer division where decimal remainders are discarded in favor of whole units.  
4.	To practice proper output formatting to present data in a userfriendly manner.  

## Algorithm
Step 1: Start  
Step 2: Declare variables: total days, years, months, days  
Step 3: Read total days from the user  
Step 4: Calculate years = total days / 365  
Step 5: Calculate the remaining days after years: temp days = total days % 365  
Step 6: Calculate months = temp days / 30  
Step 7: Calculate the final remaining days = temp days % 30  
Step 8: Display the results  
Step 9: End  

## Code
#include<stdio.h>
int main()
{
    int total_days,years,months,days;
    printf("Enter the total number of days:");
    scanf("%d",&total_days);

    years=total_days/365;
    months=(total_days%365)/30;
    days=(total_days%365)%30;

    printf("\n%d days is equivalent to:\n", total_days);
    printf("Years : %d\n", years);
    printf("Months: %d\n", months);
    printf("Days  : %d\n", days);

    return 0;

}

## Output
Input: Enter the total number of days: 1320 Output: 1320 days is equivalent to:  
Years : 3  
Months: 7  
Days : 15    

## Conclusion
The program successfully fulfills the requirement of converting a  number of days into a hierarchical format. This exercise reinforces the importance of the modulus operator in unit conversion tasks and highlights the precision required in sequential mathematical logic.  

