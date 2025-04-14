# F1 Driver Rating Analysis: Finding Underrated Performers

## Overview
This machine learning project analyzes Formula 1 driver performance to identify underrated drivers. By comparing predicted points (based on raw performance) against actual points scored, we can see which drivers are performing better than their championship position suggests.

## 🏎️ What Makes This Special
Unlike traditional F1 statistics, this model:
- Removes team/car advantage from the equation
- Focuses on pure driver performance metrics
- Uses machine learning to predict "deserved" points
- Identifies hidden talent in the field

## 📊 How It Works
The model analyzes:
- Qualifying performance vs teammate
- Race positions gained/lost
- Finish position vs teammate
- DNF rates
- Fastest lap achievements
- Pit stop efficiency

## 🤖 Technical Details
The project uses:
- Random Forest Regression model
- FastF1 API for data collection
- Multiple races for consistent analysis
- Performance-only metrics (no team bias)

## 📈 Visualizations
Two main graphs show:
1. **Points Difference Trend**
   - Shows how under/overrated status changes over races
   - Tracks consistency of performance

2. **Total Points Difference**
   - Green bars = Underrated drivers
   - Red bars = Overrated drivers
   - Height shows magnitude of rating difference

## 🏆 Key Findings
The model reveals:
- Which drivers consistently outperform their machinery
- Who's really making the most of their equipment
- Hidden performance not reflected in championship points

## 🛠️ Requirements
- Python 3.7+
- FastF1
- pandas
- scikit-learn
- matplotlib/seaborn

## 🔄 Future Updates
Planning to add:
- More historical race data
- Weather impact analysis
- Qualifying session type consideration
- Interactive data visualizations
- Race strategy effectiveness metrics

## 👨‍💻 Usage
Run `f1_driver_rating.py` to:
1. Fetch recent F1 race data
2. Process driver performance metrics
3. Generate prediction model
4. View underrated/overrated analysis

## 🏁Results 

🏆 TOP 3 MOST UNDERRATED DRIVERS:
--------------------------------------------------

Oscar Piastri (McLaren):
  Average Points per Race: 7.5
  Average Predicted Points: 7.9
  Total Points: 75.0
  Total Predicted: 79.4
  Underrated by: 4.4 points total
  (0.4 points per race)

Lance Stroll (Aston Martin):
  Average Points per Race: 3.6
  Average Predicted Points: 4.0
  Total Points: 36.0
  Total Predicted: 40.1
  Underrated by: 4.1 points total
  (0.4 points per race)

Guanyu Zhou (Alfa Romeo):
  Average Points per Race: 0.2
  Average Predicted Points: 0.4
  Total Points: 2.0
  Total Predicted: 4.2
  Underrated by: 2.2 points total
  (0.2 points per race)

📉 TOP 3 MOST OVERRATED DRIVERS:
--------------------------------------------------

Carlos Sainz (Ferrari):
  Average Points per Race: 10.1
  Average Predicted Points: 10.0
  Total Points: 91.0
  Total Predicted: 90.2
  Overrated by: 0.8 points total
  (0.1 points per race)

Esteban Ocon (Alpine):
  Average Points per Race: 2.2
  Average Predicted Points: 2.1
  Total Points: 22.0
  Total Predicted: 20.6
  Overrated by: 1.4 points total
  (0.1 points per race)

Sergio Perez (Red Bull Racing):
  Average Points per Race: 9.8
  Average Predicted Points: 9.6
  Total Points: 98.0
  Total Predicted: 96.3
  Overrated by: 1.7 points total
  (0.2 points per race)

Interestingly Max Verstappen is severely underrated in the model, the model consistently predicted that Max should have scored fewer points than he actually did — and he outperformed its expectations by a large margin.

In simpler terms:
The model underrated Max Verstappen's performance.

---
*This is an educational project using publicly available F1 data. Not affiliated with Formula 1 or the FIA.*
