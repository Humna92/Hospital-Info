#convert missing data to National Average or 3/5 rating
HospInfo$`Meets criteria for meaningful use of EHRs`[HospInfo$`Meets criteria for meaningful use of EHRs` %in% c(NA)] <- TRUE
HospInfo$`Hospital overall rating`[HospInfo$`Hospital overall rating` %in% c("Not Available")] <- 3
HospInfo$`Mortality national comparison`[HospInfo$`Mortality national comparison` %in% c("Not Available")] <- "Same as the National average"
HospInfo$`Safety of care national comparison`[HospInfo$`Safety of care national comparison` %in% c("Not Available")] <- "Same as the National average"
HospInfo$`Readmission national comparison`[HospInfo$`Readmission national comparison` %in% c("Not Available")] <- "Same as the National average"
HospInfo$`Patient experience national comparison`[HospInfo$`Patient experience national comparison` %in% c("Not Available")] <- "Same as the National average"
HospInfo$`Effectiveness of care national comparison`[HospInfo$`Effectiveness of care national comparison` %in% c("Not Available")] <- "Same as the National average"
HospInfo$`Timeliness of care national comparison`[HospInfo$`Timeliness of care national comparison` %in% c("Not Available")] <- "Same as the National average"
HospInfo$`Efficient use of medical imaging national comparison`[HospInfo$`Efficient use of medical imaging national comparison` %in% c("Not Available")] <- "Same as the National average"
