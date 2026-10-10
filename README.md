Portfolio Optimization with Monte Carlo Simulation

This project is a Python-based financial analytics tool that applies Modern Portfolio Theory. It uses historical stock data to run Monte Carlo simulations, calculates risk and return metrics, and identifies optimal asset allocations.

Project Structure

The project is divided into modular Python scripts to separate concerns:

main.py: The entry point that runs the entire analysis pipeline.

data_loader.py: Fetches historical stock prices using the Yahoo Finance API and saves them locally.

data_processor.py: Reads the raw data, calculates daily percentage changes, expected annual returns, and the covariance matrix.

portfolio_optimizer.py: Runs 50,000 Monte Carlo simulation iterations to find the portfolio with the maximum Sharpe ratio and the minimum risk.

analytics_report.py: Prints a structured text summary of the optimization results and asset weights to the terminal.

visualizer.py: Generates an Efficient Frontier scatter plot using Matplotlib to visualize risk-return trade-offs.

Requirements

To run this project, you need Python and the following libraries installed:

pip install yfinance pandas numpy matplotlib


How to Run

Clone or download the repository to your local machine.

Run the main script from your terminal or IDE:

python main.py


The program will automatically download the required CSV data if it does not exist locally, execute the simulation, print the report, and display the visualization window.
