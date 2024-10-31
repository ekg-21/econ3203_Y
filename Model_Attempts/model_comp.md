# Scale shops and atms and then create interaction variables
## Best model:
Formula is:  Withdraw ~ Shops + ATMs + Downtown + Weekday + Center + High + Downtown_NotWeekday_Center + Shops_DWC + Shops_DT + Weekday__DT + Center_DT
Test MSE:  0.2690572201362564
Train MSE:  0.2715607793268146

# No scaling
## Best model:
Formula is:  Withdraw ~ Shops_DT + Weekday__DT + Center_DT + Shops_DWC + Shops + ATMs + Downtown + Weekday + Center + High
Test MSE:  0.2689971805072948
Train MSE:  0.27161776476251853

# Scale shops, atms, shops_dt, atms_dt, shops_dwc, atms_dwc after defining them
## Best model:
Formula is:  Withdraw ~ Shops + ATMs + Downtown + Weekday + Center + High + Shops_DWC + Shops_DT + Weekday__DT + Center_DT
Test MSE:  0.26899718050733634
Train MSE:  0.2716177647625186

# Scale everything
## Best model:
Formula is:  Withdraw ~ Shops + ATMs + Downtown + Weekday + Center + High + Shops_DWC + Shops_DT + Weekday__DT + Center_DT
Test MSE:  0.2689971805073376
Train MSE:  0.2716177647625185