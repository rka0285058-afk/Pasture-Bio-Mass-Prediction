# Pasture-Bio-Mass-Prediction
Australia has two main crop seasons: winter crops are sown in autumn and harvested in spring/summer, and summer crops are sown in spring and harvested in autumn. Winter crops, like wheat, are common in temperate zones and are planted from April to June, while summer crops, like cotton, are grown in warmer regions and are planted later. 

Google Earth Engine platform has been utilized in creating the prediction model for pasture bio mass in Australia. The following setallite imageries considered for modelling:
ee.ImageCollection(
  "projects/global-pasture-watch/assets/ggc-30m/v1/cultiv-grassland_p"
)
 ee.ImageCollection(
  "projects/global-pasture-watch/assets/ggc-30m/v1/grassland_c"
)
ee.ImageCollection("LANDSAT/LC08/C02/T1")

The data of 2000 and 2022 was used in predicting the pasture bio mass for the year 2025.
The dependent variables considered are NDVI,NDWI,BSI and NDMSI. The predictions models were Linear Regression, Cart Regression and Smile Random Forest Regression. The train and test accuracy observed around 90% in all the models. The R squared was 1 and RSME values were less than 1 in all the cases.

The net changes in area(ha) from other to other = 9427636.56
The net changes in area(ha) from cultivated to cultivated =8120351.09
The net changes in area(ha) from natural/semi-natural to  natural/semi-natural = 3353532.08

The above changes are for entire country. The grazing of pasture bio mass may be planned during off crop seasons in the country

