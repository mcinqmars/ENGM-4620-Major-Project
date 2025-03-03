# ENGM-4620-Major-Project
Travel Expense Calculator

Overview
The Travel Expense Calculator is a Python-based tool that helps users estimate the cost of a trip, including flight expenses and hotel costs. It reads flight data from a CSV file and calculates the cheapest available travel route (direct, one-stop, or two-stop flights). The program then estimates accommodation costs and provides a total estimated travel expense.

How It Works
1.	User Input:
  o	The user enters a departure city and destination city.
  o	Specifies the number of nights for hotel accommodation.
  o	Chooses whether a return flight is needed.
2.	Flight Data Processing:
  o	The program loads flight data from a CSV file.
  o	Searches for the cheapest direct flight first.
  o	If no direct flight is available, it attempts to find a one-stop connection.
  o	If no one-stop flight is found, it searches for a two-stop connection.
  o	If no flights are found, an error message is displayed.
3.	Hotel Cost Calculation:
  o	The script assumes a fixed rate of $100 per night for accommodation.
  o	Multiplies the number of nights by the nightly rate to get the total hotel cost.
4.	Expense Calculation and Display:
  o	The total flight and hotel costs are calculated and displayed. 
3. How to Use the Program
  3.1 Requirements
  Ensure the following are installed before running the script:
    •	Python 3.x
    •	pandas library (Install with pip install pandas)
    •	CSV file containing flight data (Updated_Flight_Data_Short.csv)
