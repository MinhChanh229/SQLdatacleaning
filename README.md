# SQLdatacleaning
This is an educational project on data cleaning and preparation using SQL. The original database in CSV format is located in the file club_member_info.csv. Here, we will explore the steps that need to be applied to obtain a cleansed version of the dataset
|full_name|age|martial_status|email|phone|full_address|job_title|membership_date|
|---------|---|--------------|-----|-----|------------|---------|---------------|
|      Nelson Sellwood|28|married|nsellwoodiw@vinaora.com|626-679-7205|61336 Bashford Pass,Pasadena,California|Senior Financial Analyst|1/12/2015|
|      ROCK CRADICK|46|married|rcradick1@newsvine.com|910-566-2007|4 Harbort Avenue,Fayetteville,North Carolina|Programmer III|5/27/2018|
|     Filberto Dalman|37|single|fdalman7a@dailymotion.com|214-761-5800|288 Meadow Valley Parkway,Dallas,Texas|Internal Auditor|2/17/2019|
|     Ilyse Heeley|52|single|iheeleyl0@deviantart.com|484-332-6118|5 Susan Place,Reading,Pennsylvania|Administrative Assistant III|11/29/2015|
|     Jenn McNeillie|50|married|jmcneillie5a@diigo.com|850-676-5843|2587 Stoughton Terrace,Tallahassee,Florida|Sales Representative|9/30/2014|
|     Pippo MacGeffen|36|single|pmacgeffenhr@de.vu|707-233-6862|2659 Mesta Avenue,Santa Rosa,California|Marketing Assistant|2/19/2012|
|     maire perrie|56|single|mperriekh@tinyurl.com|208-674-0036|5879 Lindbergh Center,Boise,Idaho|Quality Engineer|9/7/2019|
|    Brock Wooldridge  |41|married|bwooldridge5s@wsj.com|202-601-2814|13 Rowland Center,Washington,District of Columbia|Engineer II|1/21/2022|
|    CESARO HARDES|53|married|chardesfo@army.mil|760-170-8812|42091 Rutledge Point,San Bernardino,California|Senior Developer|7/17/2012|
|    Dottie Cribbott|65|divorced|dcribbottmf@rambler.ru|212-113-0379|4890 Bluestem Lane,Brooklyn,New York|Structural Engineer|6/12/2018|

CREATE TABLE club_member_info_cleaned (
	full_name VARCHAR(50),
	age INTEGER,
	martial_status VARCHAR(50),
	email VARCHAR(50),
	phone VARCHAR(50),
	full_address VARCHAR(50),
	job_title VARCHAR(50),
	membership_date VARCHAR(50)
);

INSERT INTO club_member_info_cleaned
SELECT * FROM club_member_info 
