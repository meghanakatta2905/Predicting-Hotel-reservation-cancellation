Hotel Reservation Cancellation Prediction

This project uses machine learning to predict whether a hotel reservation will be canceled. By analyzing historical booking data, the goal is to help hotels reduce revenue loss, improve occupancy planning, and make smarter decisions about overbooking and promotions.

Objective
	•	Predict the likelihood of reservation cancellations using historical booking data
	•	Identify key factors that contribute to cancellations
	•	Provide insights to support hotel revenue and booking strategy optimization

Dataset Overview

The dataset includes information on past hotel reservations with various features:
	•	Reservation_ID – Unique ID for each booking
	•	Booking_Date – Date when reservation was made
	•	Checkin_Date / Checkout_Date – Scheduled stay dates
	•	Hotel_Type – Type of hotel (e.g., city, resort)
	•	Number_of_Nights – Total nights booked
	•	Number_of_Guests – Guest count per booking
	•	Lead_Time – Days between booking and check-in
	•	Room_Type – Category of room booked
	•	Reservation_Status – Target label (Confirmed, Canceled)

Project Workflow

Data Preprocessing
	•	Handled missing values, incorrect formats, and duplicate entries
	•	Parsed dates and calculated useful time-based fields (e.g., lead time)
	•	Encoded categorical variables for modeling

Feature Engineering
	•	Created new features such as booking month, weekday of check-in, and guest-to-room ratio
	•	Analyzed cancellation trends by hotel type, lead time, and seasonality

Model Training
	•	Trained and compared multiple models:
	•	Logistic Regression
	•	Random Forest
	•	Gradient Boosting Classifier

Evaluation
	•	Used Accuracy, Precision, Recall, and F1-score for model assessment
	•	Performed confusion matrix analysis to understand false positives/negatives

Results and Insights
	•	Models successfully identified bookings with high cancellation risk
	•	Longer lead times and weekend check-ins were linked to higher cancellation rates
	•	Random Forest and Gradient Boosting provided the best performance balance
	•	Results can help hotels take preventive actions such as deposit policies or reminders

Tools and Technologies
	•	Language: Python
	•	Libraries: pandas, numpy, scikit-learn, matplotlib, seaborn
	•	Development Environment: Jupyter Notebook, PyCharm / VS Code

Future Enhancements
	•	Incorporate external features like weather, holidays, or promotions
	•	Build a web dashboard using Streamlit to test live predictions
	•	Apply time-series models for cancellation trend forecasting
