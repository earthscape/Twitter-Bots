

Haiyan (Yolanda) - 
Tacloban City Impact: 2013-11-08 04:00:00


Unique bots in ph2013_tacloban_33day - none
SELECT DISTINCT ph2013_tacloban_33day.twitter_uid FROM ph2013_tacloban_33day JOIN twitter_bots_uids ON ph2013_tacloban_33day.twitter_uid = twitter_bots_uids.twitter_uid

-- Count Tacloban days after storm: 168
SELECT * FROM ph2013_tacloban_33day where localdate between '2013-11-09' and '2013-11-25 23:59:59+00'




-- Count Tacloban days - None on day of storm in ph2013_tacloban_33day table.
SELECT day, count(*) FROM ph2013_tacloban_33day 
where day between '2013-11-08 00:00:00+00' and '2013-11-25 23:59:59+00'
GROUP BY Day 
ORDER BY Day


-- Count Entire Philippines: 1,162,438
SELECT count(*) FROM ph2013 
-- Limit to 270
WHERE (ST_DWithin(the_geom::geography,ST_GeomFromText('POINT(124.9617 11.2543)', 4326)::geography, 11000))
AND localdate between '2013-11-09' and '2013-11-25 23:59:59+00'



-- Counts per day for Tacloban, two cities
SELECT day, city, count(*) FROM all_33day 
where day between '2013-10-01 00:00:00+00' and '2013-11-25 23:59:59+00'
AND step_type = 0
GROUP BY Day,city 
ORDER BY Day