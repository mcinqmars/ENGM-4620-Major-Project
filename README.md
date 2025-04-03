Travel Expense Calculator
Overview
The Travel Expense Calculator is a Python-based tool that helps users estimate the total cost of a trip, including flight and hotel expenses. It reads flight data from a CSV file, identifies the cheapest available travel route (direct or with one stop), and computes the total cost based on user input.

How It Works
1. User Input
The user provides:
- A departure city or airport code
- A destination city or airport code
- The number of nights they plan to stay
- The nightly hotel rate
- Whether a return flight is required
- An optional maximum budget

2. Flight Data Processing
The program reads flight data from a CSV file using pandas.

It searches for:
- The cheapest direct flight first
- If unavailable, it checks for one-stop connections
- Two-stop flights are not supported in the current version.
- If no valid route is found, the user is informed with a clear error message.

3. Hotel Cost Calculation
Calculates hotel expenses by multiplying the number of nights by the provided nightly rate.
Users can input any hotel rate; it is not fixed at $100.

4. Expense Calculation and Display
Summarizes:
- Flight route(s) (including connection info)
- Total flight cost (one-way or round-trip)
- Total hotel cost
- Final estimated travel expense
- If a budget is provided, the tool checks whether the trip is within that limit.
- Offers to export a summary of the trip to a CSV file.

How to Use the Program
Requirements:
- Python 3.x
- pandas library (Install with: pip install pandas)
- A CSV file containing flight data (e.g., Updated_Flight_Data_Short.csv)

Running the Program:
- The script is designed to run as a standalone terminal/command-line application.
- Follow the prompts to input trip details.
- Review the output or export it as a CSV summary.
