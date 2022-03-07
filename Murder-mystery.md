```.py
select description from crime_scene_report WHERE date = 20180115 and type = 'murder' and city = 'SQL City';
select address_number from person WHERE address_street_name = 'Northwestern Dr' order by address_number asc;
select id, name, address_number from person WHERE address_number = 4919 or address_number = 309;
select transcript from interview WHERE person_id = 14887 or person_id = 80539 or person_id = 85646 or person_id = 87221 or person_id = 87260 or person_id = 89906;
select plate_number, gender, id from drivers_license WHERE plate_number like '%H42W%';
select membership_id from get_fit_now_check_in WHERE check_in_date = 20180109 and membership_id like '48Z%';
select person_id, id from get_fit_now_member WHERE id = '48Z7A';
select person_id, id from get_fit_now_member WHERE id = '48Z55';
select person_id from facebook_event_checkin WHERE event_name = 'SQL Symphony Concert' and date > 20171200 and date < 20180000;
select id, car_model, hair_color from drivers_license WHERE id = 24556;
select id, height, hair_color, gender, car_make, car_model from drivers_license WHERE hair_color = 'red' and gender = 'female' and car_make = 'Tesla';
select name, id from person WHERE id = 99716 or id = 24556;
INSERT INTO solution VALUES (1, 'Miranda Priestly');
select * from person WHERE name = 'Miranda Priestly'
```
