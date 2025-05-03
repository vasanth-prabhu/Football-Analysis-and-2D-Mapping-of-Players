# Football Analysis and 2D Mapping of Players

This project performs advanced football match analysis by processing video footage to track players and the ball, estimate camera movement, assign teams, and calculate speed and distance metrics. The output is a video with annotated player and ball movements, team assignments, and other insights.

## How It Works
1. **Training**: First we train the YOLOv8 model with the football dataset from roboflow. This is done in Football_Analysis.ipynb file. From that we obtain our best.pt model and last.pt model. We use best.pt model for our project.
2. **Input Video**: The script reads the input video from the input directory.
3. **Object Tracking**: Tracks players and the ball using a trained model.
4. **Camera Movement Estimation**: Adjusts player and ball positions based on camera movement.
5. **2D View Transformation**: Transforms positions to a 2D plane for better analysis.
6. **Speed and Distance Estimation**: Calculates speed and distance covered by players.
7. **Team Assignment**: Identifies and assigns players to their respective teams.
8. **Ball Possession Assignment**: Determines which player and team have ball possession.
9. **Annotated Output Video**: Generates a video with all the above insights visualized.
10. **Graph Output**: Plot generates graph for heatmap and average speed and distance .

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/vasanth-prabhu/Football-Analysis-and-2D-Mapping-of-Players.git
   cd Football-Analysis-and-2D-Mapping-of-Players
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
3. Place your input video in the input directory.
4. Run the main.py file.

## Dependencies 
The techstack used in the project are:
1. Python 3.12.9
2. OpenCV
3. Numpy
4. Pandas
5. Supervision
6. Ultralytics
7. Scikit Learn
