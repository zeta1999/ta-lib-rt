cmake_minimum_required(VERSION 3.10.0)
project(TaLibRtSrc)
set(CMAKE_CXX_STANDARD 17)
include_directories(../include)
include_directories(ta_abstract)
include_directories(ta_abstract/frames)
include_directories(ta_abstract/tables)
include_directories(ta_common)
include_directories(ta_func)

add_library(TaLibRt STATIC 
    ta_abstract/frames/ta_frame.c
    ta_abstract/tables/table_a.c
    ta_abstract/tables/table_b.c
    ta_abstract/tables/table_c.c
    ta_abstract/tables/table_d.c
    ta_abstract/tables/table_e.c
    ta_abstract/tables/table_f.c
    ta_abstract/tables/table_g.c
    ta_abstract/tables/table_h.c
    ta_abstract/tables/table_i.c
    ta_abstract/tables/table_j.c
    ta_abstract/tables/table_k.c
    ta_abstract/tables/table_l.c
    ta_abstract/tables/table_m.c
    ta_abstract/tables/table_m.c
    ta_abstract/tables/table_o.c
    ta_abstract/tables/table_p.c
    ta_abstract/tables/table_q.c
    ta_abstract/tables/table_r.c
    ta_abstract/tables/table_s.c
    ta_abstract/tables/table_t.c
    ta_abstract/tables/table_u.c
    ta_abstract/tables/table_v.c
    ta_abstract/tables/table_w.c
    ta_abstract/tables/table_x.c
    ta_abstract/tables/table_y.c
    ta_abstract/tables/table_z.c
    ta_abstract/ta_abstract.c
    ta_abstract/ta_def_ui.c
    ta_abstract/ta_func_api.c
    ta_abstract/ta_group_idx.c
    ta_common/ta_global.c
    ta_common/ta_retcode.c
    ta_common/ta_version.c
    
ta_func/ta_ACOS.c
ta_func/ta_AD.c
ta_func/ta_ADD.c
ta_func/ta_ADOSC.c
ta_func/ta_ADX.c
ta_func/ta_ADXR.c
ta_func/ta_APO.c
ta_func/ta_AROON.c
ta_func/ta_AROONOSC.c
ta_func/ta_ASIN.c
ta_func/ta_ATAN.c
ta_func/ta_ATR.c
ta_func/ta_AVGPRICE.c
ta_func/ta_BBANDS.c
ta_func/ta_BETA.c
ta_func/ta_BOP.c
ta_func/ta_CCI.c
ta_func/ta_CDL2CROWS.c
ta_func/ta_CDL3BLACKCROWS.c
ta_func/ta_CDL3INSIDE.c
ta_func/ta_CDL3LINESTRIKE.c
ta_func/ta_CDL3OUTSIDE.c
ta_func/ta_CDL3STARSINSOUTH.c
ta_func/ta_CDL3WHITESOLDIERS.c
ta_func/ta_CDLABANDONEDBABY.c
ta_func/ta_CDLADVANCEBLOCK.c
ta_func/ta_CDLBELTHOLD.c
ta_func/ta_CDLBREAKAWAY.c
ta_func/ta_CDLCLOSINGMARUBOZU.c
ta_func/ta_CDLCONCEALBABYSWALL.c
ta_func/ta_CDLCOUNTERATTACK.c
ta_func/ta_CDLDARKCLOUDCOVER.c
ta_func/ta_CDLDOJI.c
ta_func/ta_CDLDOJISTAR.c
ta_func/ta_CDLDRAGONFLYDOJI.c
ta_func/ta_CDLENGULFING.c
ta_func/ta_CDLEVENINGDOJISTAR.c
ta_func/ta_CDLEVENINGSTAR.c
ta_func/ta_CDLGAPSIDESIDEWHITE.c
ta_func/ta_CDLGRAVESTONEDOJI.c
ta_func/ta_CDLHAMMER.c
ta_func/ta_CDLHANGINGMAN.c
ta_func/ta_CDLHARAMI.c
ta_func/ta_CDLHARAMICROSS.c
ta_func/ta_CDLHIGHWAVE.c
ta_func/ta_CDLHIKKAKE.c
ta_func/ta_CDLHIKKAKEMOD.c
ta_func/ta_CDLHOMINGPIGEON.c
ta_func/ta_CDLIDENTICAL3CROWS.c
ta_func/ta_CDLINNECK.c
ta_func/ta_CDLINVERTEDHAMMER.c
ta_func/ta_CDLKICKING.c
ta_func/ta_CDLKICKINGBYLENGTH.c
ta_func/ta_CDLLADDERBOTTOM.c
ta_func/ta_CDLLONGLEGGEDDOJI.c
ta_func/ta_CDLLONGLINE.c
ta_func/ta_CDLMARUBOZU.c
ta_func/ta_CDLMATCHINGLOW.c
ta_func/ta_CDLMATHOLD.c
ta_func/ta_CDLMORNINGDOJISTAR.c
ta_func/ta_CDLMORNINGSTAR.c
ta_func/ta_CDLONNECK.c
ta_func/ta_CDLPIERCING.c
ta_func/ta_CDLRICKSHAWMAN.c
ta_func/ta_CDLRISEFALL3METHODS.c
ta_func/ta_CDLSEPARATINGLINES.c
ta_func/ta_CDLSHOOTINGSTAR.c
ta_func/ta_CDLSHORTLINE.c
ta_func/ta_CDLSPINNINGTOP.c
ta_func/ta_CDLSTALLEDPATTERN.c
ta_func/ta_CDLSTICKSANDWICH.c
ta_func/ta_CDLTAKURI.c
ta_func/ta_CDLTASUKIGAP.c
ta_func/ta_CDLTHRUSTING.c
ta_func/ta_CDLTRISTAR.c
ta_func/ta_CDLUNIQUE3RIVER.c
ta_func/ta_CDLUPSIDEGAP2CROWS.c
ta_func/ta_CDLXSIDEGAP3METHODS.c
ta_func/ta_CEIL.c
ta_func/ta_CMO.c
ta_func/ta_CORREL.c
ta_func/ta_COS.c
ta_func/ta_COSH.c
ta_func/ta_DEMA.c
ta_func/ta_DIV.c
ta_func/ta_DX.c
ta_func/ta_EMA.c
ta_func/ta_EXP.c
ta_func/ta_FLOOR.c
ta_func/ta_HT_DCPERIOD.c
ta_func/ta_HT_DCPHASE.c
ta_func/ta_HT_PHASOR.c
ta_func/ta_HT_SINE.c
ta_func/ta_HT_TRENDLINE.c
ta_func/ta_HT_TRENDMODE.c
ta_func/ta_KAMA.c
ta_func/ta_LINEARREG.c
ta_func/ta_LINEARREG_ANGLE.c
ta_func/ta_LINEARREG_INTERCEPT.c
ta_func/ta_LINEARREG_SLOPE.c
ta_func/ta_LN.c
ta_func/ta_LOG10.c
ta_func/ta_MA.c
ta_func/ta_MACD.c
ta_func/ta_MACDEXT.c
ta_func/ta_MACDFIX.c
ta_func/ta_MAMA.c
ta_func/ta_MAVP.c
ta_func/ta_MAX.c
ta_func/ta_MAXINDEX.c
ta_func/ta_MEDPRICE.c
ta_func/ta_MFI.c
ta_func/ta_MIDPOINT.c
ta_func/ta_MIDPRICE.c
ta_func/ta_MIN.c
ta_func/ta_MININDEX.c
ta_func/ta_MINMAX.c
ta_func/ta_MINMAXINDEX.c
ta_func/ta_MINUS_DI.c
ta_func/ta_MINUS_DM.c
ta_func/ta_MOM.c
ta_func/ta_MULT.c
ta_func/ta_NATR.c
ta_func/ta_NVI.c
ta_func/ta_OBV.c
ta_func/ta_PLUS_DI.c
ta_func/ta_PLUS_DM.c
ta_func/ta_PPO.c
ta_func/ta_PVI.c
ta_func/ta_ROC.c
ta_func/ta_ROCP.c
ta_func/ta_ROCR.c
ta_func/ta_ROCR100.c
ta_func/ta_RSI.c
ta_func/ta_SAR.c
ta_func/ta_SAREXT.c
ta_func/ta_SIN.c
ta_func/ta_SINH.c
ta_func/ta_SMA.c
ta_func/ta_SQRT.c
ta_func/ta_STDDEV.c
ta_func/ta_STOCH.c
ta_func/ta_STOCHF.c
ta_func/ta_STOCHRSI.c
ta_func/ta_SUB.c
ta_func/ta_SUM.c
ta_func/ta_T3.c
ta_func/ta_TAN.c
ta_func/ta_TANH.c
ta_func/ta_TEMA.c
ta_func/ta_TRANGE.c
ta_func/ta_TRIMA.c
ta_func/ta_TRIX.c
ta_func/ta_TSF.c
ta_func/ta_TYPPRICE.c
ta_func/ta_ULTOSC.c
ta_func/ta_VAR.c
ta_func/ta_WCLPRICE.c
ta_func/ta_WILLR.c
ta_func/ta_WMA.c
ta_func/ta_utility.c

)

add_executable(TaLibRtDemo TaLibDemoRt.cpp)
target_link_libraries(TaLibRtDemo PUBLIC TaLibRt)
