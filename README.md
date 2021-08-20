# Pump-repairability-preciction-classification-using-4-models
## Pump repairability (Ministry of Africa) prediction/classification using RandomForest, Decision Tree, Gradient boost, Line search CV

## DATSET :
 Input features are 40
 id 	amount_tsh 	date_recorded 	funder 	gps_height 	installer 	longitude 	latitude 	wpt_name 	num_private 	basin 	subvillage 	region 	region_code 	district_code 	lga 	ward 	population 	public_meeting 	recorded_by 	scheme_management 	scheme_name 	permit 	construction_year 	extraction_type 	extraction_type_group 	extraction_type_class 	management 	management_group 	payment 	payment_type 	water_quality 	quality_group 	quantity 	quantity_group 	source 	source_type 	source_class 	waterpoint_type 	waterpoint_type_group
 
 the total no of points is 40k+
 the target variable is a multiclasss classification having targets:
 1. Functional
 2. Non-functional 
 3. functional but needs repair
 ![image](https://user-images.githubusercontent.com/87943264/130183010-1fd9fa8e-d288-4cc0-8919-320e4a75b0de.png)

## DATA PREPROCESSING AND CLEANSING 
  Removing the unnecessary features and finally after cleansing
   	amount_tsh 	funder 	gps_height 	installer 	basin 	subvillage 	population 	public_meeting 	scheme_management 	scheme_name 	permit 	construction_year 	extraction_type 	payment_type 	water_quality 	quantity_group 	source_type 	source_class 	waterpoint_type 	waterpoint_type_group
 ## Feature Importance 
 ![image](https://user-images.githubusercontent.com/87943264/130183605-57ffd2de-3f3f-4fae-ae02-919d0cb0ff8f.png)

RESULTS:
1. RandomForest Classifier :
   ![image](https://user-images.githubusercontent.com/87943264/130183731-aa181b53-1f91-4397-92ad-8de583a6c60b.png)
2. Decision Tree Classifier :
   ![image](https://user-images.githubusercontent.com/87943264/130183793-f6a811fc-f4a1-497c-afc2-93a754ed6936.png)
3. Extra Tree Classifier :
   ![image](https://user-images.githubusercontent.com/87943264/130183833-a3d08bd2-8434-4bd3-9742-3e74d425006e.png)
4. Gradient Boost :
   ![image](https://user-images.githubusercontent.com/87943264/130183918-8d55a1ed-fd60-40a9-921e-cc8a0eef4954.png)


## CONCLUSION:
Out of all the ML Models Random Forest performs bettter and gives an accuracy of 93.% on train data and 78.8% on test data
