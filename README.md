# Airline-Price-Dynamics

### <span style="color:#00008B;">Introduction</span>

<p style="font-size: 1.1em; line-height: 1.6;">
The objective of this study is to analyze the flight booking dataset obtained from the “Ease My Trip” website and <br> to conduct various statistical hypothesis tests to extract meaningful insights from it.
</p>
<hr>

### <span style="color:#00008B;">Research Questions</span>

<p style="font-size: 1.1em; line-height: 1.6;">
The aim of our study is to answer the following research questions:
</p>

1. <span style="color:#3498db;">**Does price vary with Airlines?**</span>
2. <span style="color:#3498db;">**How is the price affected when tickets are bought just 1 or 2 days before departure?**</span>
3. <span style="color:#3498db;">**Does ticket price change based on the departure time and arrival time?**</span>
4. <span style="color:#3498db;">**How does the price change with the Source and Destination?**</span>
5. <span style="color:#3498db;">**How does the ticket price vary between Economy and Business class?**</span>
<br>

<hr>

### <span style="color:#00008B;">Data Collection and Methodology</span>

<p style="font-size: 1.1em; line-height: 1.6;">
The<strong>Octoparse</strong> scraping tool was used to extract data from the website. Data was collected in two parts: one for economy class tickets and another for business class tickets. A total of <strong>300,261</strong> distinct flight booking options were extracted from the site. Data collection spanned <strong>50 days</strong>, from <strong>February 11th to March 31st, 2022.</strong> <br> Dataset contains information about flight booking options from the website “Ease My Trip” for flight travel between India's top 6 metro cities. There are 300261 datapoints and 11 features..
</p>


<hr>

### <span style="color:#00008B;">Features</span>

<ol style="font-size: 1.1em; line-height: 1.6;">
  <li><strong>Airline:</strong> The name of the airline company.</li>
  <li><strong>Flight:</strong> Stores information regarding the plane's flight code.</li>
  <li><strong>Source City:</strong> The city from which the flight takes off.</li>
  <li><strong>Departure Time:</strong> The departure time, categorized into 6 unique time labels.</li>
  <li><strong>Stops:</strong> The number of stops between the source and destination cities.</li>
  <li><strong>Arrival Time:</strong> The arrival time, also categorized into 6 unique time labels.</li>
  <li><strong>Destination City:</strong> The city where the flight will land.</li>
  <li><strong>Class:</strong> Either Business or Economy.</li>
  <li><strong>Duration:</strong> The overall time it takes to travel between cities, measured in hours.</li>
  <li><strong>Days Left:</strong> The number of days left, calculated by subtracting the trip date from the booking date.</li>
  <li><strong>Price:</strong> The ticket price.</li>
</ol>
<br>
<hr>


<div style="background-color: #e0f7fa; padding: 10px; border-radius: 5px;">
    <h2 style="color: #00796b;">Random Forest Regressor Performance</h2>
    <ul>
        <li><strong>Random Forest Regressor</strong> is the <strong>best model</strong> with the <strong>highest accuracy of 98%</strong>.</li>
        <li>It also achieved the <strong>lowest RMSE of 2,179</strong>.</li>
    </ul>
</div>


# <span style="color:#00008B;">Answers Research Questions</span>

1. <span style="color:#3498db;">**Does price vary with Airlines?**</span><br>
**Yes It Does.**<br>**Vistara** and **Air India** are notably more expensive compared to other airlines.
  
2. <span style="color:#3498db;">**How is the price affected when tickets are bought just 1 or 2 days before departure?**</span><br>
**1 Day Before:** Potential for a price drop(same as 15 days Before).<br>
**2 Days Before:** Prices typically increase due to high demand and limited availability.
   
4. <span style="color:#3498db;">**Does ticket price change based on the departure time and arrival time?**</span><br>
 **Late-Night Flights:** Typically have the **lowest prices**.<br>
 **Afternoon Flights:** Generally have the **second lowest prices**.<br>
 **Other Times:** Prices are **almost equal** across different times of the day.<br><br>
 This pricing trend reflects the demand for flight times, with late-night and afternoon departures often being less desirable for most travelers.




5. <span style="color:#3498db;">**How does the price change with the Source and Destination?**</span><br>
Ticket prices **do not significantly change** based on the source and destination.<br>
Prices **do change** based on the **distance traveled**.
6. <span style="color:#3498db;">**How does the ticket price vary between Economy and Business class?**</span><br>
**Business class flights** are **obviously more expensive** than Economy class flights.<br><br>

- **Business Class:**
   - For flight durations between **1 to 5 hours**, prices **grow sharply**.
   - For durations **more than 5 hours**, prices remain within a **range of 45,000 to 60,000**.<br><br>
   
- **Economy Class:**
   - Price shows a **linear growth** with increasing flight duration.
   - A **sharp price increase** is observed for flights with a duration of **47 hours**.





