
# Room Assignment Optimization

## Project Overview
This project implements a constraint programming solution to optimize room assignments for events. It uses Google's OR-Tools CP-SAT solver to ensure:
- Room capacity is sufficient for each event
- No double-booking of rooms
- Events from the same course (lehrgang) on the same day are assigned to the same room
- Minimizes wasted capacity and the number of rooms used

## Data Files
The program uses two CSV files located in the `data/` directory:
- `data/raeume.csv` - Contains information about available rooms and their capacities
- `data/veranstaltungen.csv` - Contains event information including dates and participant counts

## Setup Instructions

### Prerequisites
- Python 3.7+
- pipenv

### Installation

1. Clone this repository
   ```
   git clone [repository-url]
   cd [repository-directory]
   ```

2. Install dependencies using pipenv
   ```
   pipenv install
   ```

3. Activate the virtual environment
   ```
   pipenv shell
   ```

4. Launch Jupyter Notebook
   ```
   jupyter notebook
   ```

5. Open the optimization notebook and run the cells sequentially

## Dependencies
- pandas - For data manipulation
- ortools - Google's Operations Research Tools for constraint programming
- jupyter - For running the notebook interface
