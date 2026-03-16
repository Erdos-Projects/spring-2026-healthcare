# Documentation
 **MODEL**: LR
 **TARGET**: 'Log_Tot_Mdcr_Pymt_Amt_current'
 **METHOD**: Walkforward validation
 **METRIC**: $R^2(log) = 1 - \frac{\sum(\text{log_actual} - \text{log_pred})^2}{\sum(log_actual - \text{mean}(log_actual))^2}$ for feature selection
 **NOTE**:
   1. At number of feature = 10, the best $R^2(log)$ model is with features ['Log_Tot_Mdcr_Pymt_Amt','current_year','Log_Tot_Mdcr_Alowd_Amt','Tot_HCPCS_Cds','Type_Anesthesia','Bene_Avg_Age','Log_Tot_Benes','Type_MedicalSpecialtyOther','Type_OBGYN',*'Tot_Mdcr_Alowd_Amt'*]; however, it performs badly on the $R^2$ of the actual prediction (un-logged) due to the feature *'Tot_Mdcr_Alowd_Amt'*. Thus we choose the second best $R^2(log)$ features - ['Log_Tot_Mdcr_Pymt_Amt','current_year','Log_Tot_Mdcr_Alowd_Amt','Tot_HCPCS_Cds','Type_Anesthesia','Bene_Avg_Age','Log_Tot_Benes','Type_MedicalSpecialtyOther','Type_OBGYN',*'Type_Cardiology'*]