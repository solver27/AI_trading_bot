
# AI trading bot

The aim of the project is to develop an intelligent trading bot for automated trading including cryptocurrencies using state-of-the-art machine learning (ML) algorithms and feature engineering. The project provides the following major functionalities:
* Clear and consistent separation between *offline* (batch) mode for training ML models and *online* (stream) mode for predicting based on the trained models. One of the main challenges here is to guarantee that the same (derived) features are used in both modes
* Extensible approach to defining *derived features* using (Python) functions including standard technical indicators as well as arbitrary custom features
* Providing possibility to work with different *trade frequencies* (time rasters), for example, 1 minute, 1 hour or 1 day
* Customizable functions for sending signals or predictions in online mode, for example, sending to Telegram channels, API end-point, storing in a database or executing real transactions
* Functions for *backtesting* and measuring trade performance on historic data which is more difficult because requires periodic re-train of the used ML models
* *Trading service* for online mode which uses a configuration file to regtularly retrieve data updates, do analysis and send signals or execute trade transactions