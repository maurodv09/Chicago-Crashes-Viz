# Data Cleaning Documentation
1. Remove unnecessary columns: `CRASH_DATE_EST_I` `LANE_CNT` `ALIGNMENT` `CRASH_TYPE` `ROAD_DEFECT` `REPORT_TYPE` `TRAFFICWAY_TYPE` `STREET_NO` `STREET_DIRECTION` `BEAT_OF_OCCURRENCE` `PHOTOS_TAKEN_I` `STATEMENTS_TAKEN_I` `WORK_ZONE_I` `WORK_ZONE_TYPE` `WORKERS_PRESENT_I` `crash_date_dt` `CRASH_HOUR` `CRASH_MONTH`
2. Remove columns with a high percentage of null values: `INTERSECTION_RELATED_I`, `NOT_RIGHT_OF_WAY_I` `HIT_AND_RUN_I` `DOORING_I`
3. Filter out rows with null values: `INJURIES_TOTAL` `LATITUD`.
4. Clean all text columns:
    - Convert to lowercase.
    - Trim whitespace.
    - Capitalize:  `STREET_NAME`
5. Format date columns:
      - Separate date and time.
      - Change date format from mm/dd/yyyy to dd/mm/yyyy.
