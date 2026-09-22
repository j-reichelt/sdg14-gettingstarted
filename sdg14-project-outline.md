# SDG Project Plan: Goal 14 — Life Below Water

## 1\. Which of the 17 SDGs will you target?

**SDG 14:** Life Below Water

## 2\. What question will you attempt to answer with your solution?

### Primary question:

What levels of plastic pollution, chemical markers, and pH (acidity) exist in the Hudson River near Newburgh, NY, and how do these levels compare to the marine pollution and ocean acidification trends described in SDG 14?

### Sub-questions:

1. What concentration of microplastic particles exists per liter of river water at different points along the Hudson, and how does that compare to the \~13,000 pieces of plastic litter found per square kilometer of open ocean?
2. What is the pH of the river water at different points, and is it trending more acidic, mirroring the 30% rise in ocean acidification seen globally since the industrial revolution?
3. How do dissolved oxygen levels near Newburgh compare to levels considered safe for aquatic life (relevant to the overexploitation/ecosystem-health side of SDG 14)?
4. Are pollutant levels correlated with proximity to industrial or urban runoff points (land-based sources, which the UN identifies as the primary source of marine pollution)?

## 3\. Where will the data come from for this solution?

1. A water-based drone that travels a fixed route along the Hudson River near Newburgh, stopping every quarter mile to record sensor readings and collect a water sample.
2. Onboard sensor array (mounted to the drone) that continuously logs operational status, GPS coordinates, water chemistry metrics, and categorical hazard warnings as it moves.
3. Lab spectrometer analysis of the physical water samples once returned, to detect microplastic concentration and dominant polymer types.
4. *(Optional expansion)* Stationary buoy sensors anchored at 3–5 fixed points for continuous 24/7 monitoring between drone runs.

## 4\. What will the data look like once it is received?



### Raw data types by sensor / instrument

|Field / Sensor|Raw Data Type|Unit / Format|Example Raw Value|
|-|-|-|-|
|**record\_id**|Integer|Unique identifier|1337|
|**timestamp**|Integer|Datetime yyyy-mm-dd hh:mm:ss|2026-09-19 16:24:33|
|**latitude / longitude**|Array of Decimals (Floats)|degrees (lat, long)|\[42.7523, -73.689]|
|**water\_body\_name**|String|Text descriptor|Hudson River|
|**operational\_status**|Enumerated String (Enum)|Status code|ACTIVE\_SAMPLING|
|**hazard\_flag**|Boolean|True/False alert|false|
|**thermometer\_probe**|Decimal (Float)|°F|9932.0|
|**ph\_sensor**|Decimal (Float)|pH scale (0–14)|7.38|
|**dissolved\_oxygen**|Decimal (Float)|mg/L|6.14|
|**turbidity\_sensor**|Decimal (Float)|NTU|12.87|
|**salinity\_sensor**|Decimal (Float)|ppt (parts per thousand)|3.14|
|**polymer\_type\_detected**|String|Material classification|Polyethylene (PE)|
|**spectrometer\_absorbance**|Decimal (Float)|wavelength (nm), absorbance|0.11235813|
|**microplastic\_particle\_count**|Integer|particle count per 1L sample|47|
|**flow\_rate\_sensor**|Decimal (Float)|m/s|0.89|



