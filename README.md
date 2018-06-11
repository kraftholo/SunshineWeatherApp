# SunshineWeatherApp
WeatherApp making use of a variety of android features.

The app starts with the main screen having a recyclerview displaying the weather data (Description,Max&Min Temp)queried from our SQLiteDatabase using a custom made Content Provider. The menu has two options - Map Location and Settings

Map Location - Fires an intent to open the preferred location on a map (like google maps)
Settings     - Opens the settings implemented by PreferenceFragment

On clicking of any item of the recyclerview it takes us to the Details(Humidity,Pressure,Wind etc.) of that day's weather.
The Details activity has a menu which has two options - Share and Settings

Share    - It is set to "show always" as an icon on the actionbar . Fires an intent created using ShareCompat to share the                day's weather.
Settings - Opens the settings implemented by PreferenceFragment

Apart from this , the FirebaseJobDispatcher has been used to schedule the "fetching" of weather data every 3-4 hours.

IMPORTANT CONCEPTS USED - 

.RecyclerView 
.Intents 
.AsyncTask 
.Json and Json Parsing 
.Data Persistence (Shared Preferences,SQLiteDatabase) 
.PreferenceFragment 
.Content Provider 
.Services 
.JobScheduler (FirebaseJobScheduler) 
.Responsive Design 
.Material Design Guidelines 
