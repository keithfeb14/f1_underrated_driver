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

---
*This is an educational project using publicly available F1 data. Not affiliated with Formula 1 or the FIA.*
