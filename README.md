# CoinCap_Crypto


Weather API Practice
Introduction
API stands for Application Programming Interface.  They enable 2 software components to communicate with each other using a set number of protocols (AWS, 2022). To accomplish this task several tools were selected. They include Openweather.com servers for API, Jupiter notebook, citify module,  date time module, matplot module, pandas module among others.
Steps and guidelines
All the data can easily be accessed through this GitHub link. The API key is stored in the config.py file while all the workings are shown in the city_weather_api.ipynb file.
Steps
The following steps were followed, 
1.	Import dependencies and create an endpoint url to test the working of the API calls with a sample city in this case Kansas.
 ![image](https://user-images.githubusercontent.com/89704371/187543485-5531b906-24e2-4600-a658-02fe6d8114c7.png)

Figure 1: Test URL with Kansas city
The code returned a response of 200 meaning it’s working correctly.
2.	Create a list of fields that you would like to query in an API call for Kansas City weather. In this case, the following were selected as fields of interest. Coordinates, Max Temp among other fields were returned successfully .
 ![image](https://user-images.githubusercontent.com/89704371/187543523-bdab33ef-e930-4133-a830-a8939889641c.png)

Figure 2: Data query for Kansas City
3.	Generate random cities from the NumPy library and install citypy module to generate cities based on randomly selected cities. A list of cities through a for loop the reason for adding counters is create a delay since the open weather website place a limit to the number of calls you can make withing certain durations of time.
 
![image](https://user-images.githubusercontent.com/89704371/187543559-3e917a55-812b-4466-915d-f3cd5db4e831.png)

4.	Create a dataframe for the cities and only select the first 20 and save them into data frame ..repeat the process to produce a second csv 
 ![image](https://user-images.githubusercontent.com/89704371/187543657-9d1be610-4dbf-49e1-a7b8-931cd2c6f148.png)


 ![image](https://user-images.githubusercontent.com/89704371/187543635-a8e51b70-6784-45d2-a110-37c62e2cbfd6.png)

Figure 3:save to the second csv file

 
5.	Load both csv files and perform calculations, merge, and plot graphs and save images.
 
 ![image](https://user-images.githubusercontent.com/89704371/187543744-3dbe0c6b-0621-44a4-b5d3-bab11043b51a.png)

Figure 4:Load both csv
 ![image](https://user-images.githubusercontent.com/89704371/187543772-78f52093-72ec-40aa-aa84-5f6f5e400c3f.png)

Figure 5: Merge csv 1 and csv2, list column names

![image](https://user-images.githubusercontent.com/89704371/187543797-e8c86f42-7692-4cc7-a921-2c6893e19017.png)

 
Figure 6: join temp_change _df with final_complete_cities_df

6.	Plot charts and save images
 ![image](https://user-images.githubusercontent.com/89704371/187543811-074fa756-20e6-4827-8a9d-4adf0c42b78e.png)

Figure 7: line graph, and a bar graph showing Citys against their temp change

Images
![image](https://user-images.githubusercontent.com/89704371/187543841-c961cc37-9873-4abe-9d4d-e127bd2c4b59.png)

![image](https://user-images.githubusercontent.com/89704371/187543868-7cb49d62-e6eb-47ce-af32-ad2e25fa7cc9.png)

 
Conclusion
There was a temperature change in all the cities within the two different times the API was queried.
References
AWS. (2022). What is an API? Retrieved from https://aws.amazon.com: https://aws.amazon.com/what-is/api/
 https://openweathermap.org/


