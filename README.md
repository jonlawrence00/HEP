# HEP
HEP
Order of Operations:

step #1: Download "pfClusters_tree_noPU_withRegression.root" locally
    - location: /cms/data/jolawren/ana/CMSW_10_5_0/src/RegressionTrainer
    
step #2: run Read_Root.ipynb
    - Produces four pickle files:
        - "eventsWithReg_ZS_EB.pkl"
        - "eventsWithReg_FULL_PT1_EB.pkl"
        - "eventsWithReg_FULL_PT2_EB.pkl"
        - "eventsWithReg_FULL_PT3_EB.pkl"

step #3: run Training_Models.ipynb with FULL PT3 files only:
    Produces:
      'XGBR_model_FULL_PT3_tgt.sav'
      'ETR_model_FULL_PT3_tgt.sav'
      'NSVR_model_FULL_PT3_tgt.sav'
      'SVR_model_FULL_PT3_tgt.sav'
      'HGBR_model_FULL_PT3_tgt.sav'
      'ADA_model_FULL_PT3_tgt.sav'
      'KNR_model_FULL_PT3_tgt.sav'
      'RFR_model_FULL_PT3_tgt.sav'

      "xtest_FULL_PT3_tgt.pkl"
      "ytest_FULL_PT3_tgt.pkl"
      "events_FULL_PT3_test_tgt.pkl"

step #4: run Fit_Plot.ipynb with FULL PT3 files only
    Produces: Plots and fits
