 python3 main.py general     # All NSE stocks — fundamentals + regime + backtest built in                                                                                                                     
  python3 main.py intraday    # All NSE stocks — entry/stop/target for swing trades                                                                                                                            
                                                                                                                                                                                                               
  Optional filters still available if needed:                                                                                                                                                                  
  python3 main.py general --top 20                                                                                                                                                                             
  python3 main.py general --sector Banking                                                                                                                                                                     
  python3 main.py general --index nifty50   # faster, NIFTY 50 only                                                                                                                                          
  python3 main.py intraday --top 10                                
  python3 main.py general --no-cache        # force fresh data                                                                                                                                                 
                                                              
  What runs automatically in each mode:                                                                                                                                                                        
                                                                                                                                                                                                               
  ┌──────────────────────────────────┬────────────────────┬─────────────────────┐                                                                                                                              
  │                                  │      general       │      intraday       │                                                                                                                              
  ├──────────────────────────────────┼────────────────────┼─────────────────────┤                                                                                                                            
  │ Data                             │ Daily candles, 6mo │ Hourly candles, 1mo │
  ├──────────────────────────────────┼────────────────────┼─────────────────────┤
  │ Fundamentals (P/E, debt, growth) │ ✓ always           │ —                   │                                                                                                                              
  ├──────────────────────────────────┼────────────────────┼─────────────────────┤                                                                                                                              
  │ Regime detection (ADX)           │ ✓ always           │ —                   │                                                                                                                              
  ├──────────────────────────────────┼────────────────────┼─────────────────────┤                                                                                                                              
  │ Entry / Stop / Target            │ ✓                  │ ✓                   │                                                                                                                            
  ├──────────────────────────────────┼────────────────────┼─────────────────────┤                                                                                                                              
  │ Backtest (Sharpe, win rate)      │ ✓ always           │ —                   │                                                                                                                            
  ├──────────────────────────────────┼────────────────────┼─────────────────────┤                                                                                                                              
  │ Stochastic + VWAP                │ —                  │ ✓                   │
  └──────────────────────────────────┴────────────────────┴─────────────────────┘     
