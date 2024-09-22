# Vehicle-Turning-Pattern-Prediction
This project focuses on Vehicle Turning Pattern Detection, aimed at analyzing traffic flow at road junctions, identifying crucial vehicle turning patterns, and forecasting traffic behavior 30 minutes into the future. The system supports traffic management systems in optimizing traffic flow and preventing congestion.
The system utilizes state-of-the-art deep learning and statistical methods to detect, track, and predict vehicle movements at road junctions. By incorporating real-time detection, vehicle tracking, lane detection, and time series prediction, the system provides valuable insights into traffic behavior for efficient traffic management.

# Features
## 1. YOLO v10-based Traffic Analysis
 <b> Model: </b> YOLO v10 (You Only Look Once) <br/>
<b> Purpose: </b> Efficient and real-time object detection. <br/>
<b> Customization: </b> Fine-tuned to detect various types of vehicles, such as cars, trucks, buses, and motorcycles. <br/>
<b> Benefit: </b> High accuracy and speed in detecting vehicles at road junctions. <br/>
## 2. Vehicle Counting and Tracking
<b> Module: </b> ByteTrack <br/>
<b> Function: </b> After vehicle detection, the system counts and tracks vehicles in real-time. <br/>
<b> Data Collection: </b> Collects detailed movement data of vehicles as they pass through the junction, enabling the system to gather historical information. <br/>
<b> Tracking: </b> Maintains consistent tracking of each vehicle, which is vital for understanding traffic patterns. <br/>
## 3. Lane Detection
<b> Algorithm: </b> Random Sample Consensus (RANSAC) <br/>
<b> Purpose: </b> Detect lanes and segment the junction into distinct lanes. <br/>
<b> Vehicle Categorization: </b> Categorizes vehicles based on the lane they occupy, providing insight into vehicle turning patterns when combined with tracking information. <br/>
<b> Benefit: </b> Enhances understanding of the flow of vehicles across different lanes at the junction. <br/>
## 4. Time Series Prediction
<b> Model: </b> ARIMA (Auto-Regressive Integrated Moving Average) <br/>
<b> Purpose: </b> Predicts future traffic flow patterns 30 minutes into the future based on historical traffic data. <br/>
<b> Historical Data: </b> Utilizes data gathered from vehicle tracking and lane detection modules. <br/>
<b> Forecasting: </b> Helps anticipate potential congestion, supporting proactive traffic management decisions. <br/>
# How It Works
<b> Detection: </b> The YOLO v10 model is deployed to detect vehicles in real-time at the junction. <br/>
<b> Tracking:  </b> ByteTrack maintains a consistent tracking of each detected vehicle, allowing for accurate tracking of their movements across the junction. <br/>
<b> Lane Detection: </b> RANSAC is applied to identify and categorize lanes, determining the path and turning pattern of each vehicle. <br/>
<b> Prediction: </b> ARIMA uses the collected historical data to predict future traffic patterns, forecasting vehicle behavior and potential congestion 30 minutes into the future.
