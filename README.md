# FinTech-Class_C14_emorytk

Tune the Baseline Trading Algorithm

In this section, you’ll tune, or adjust, the model’s input features to find the parameters that result in the best trading outcomes. (You’ll choose the best by comparing the cumulative products of the strategy returns.) To do so, complete the following steps:

    Tune the training algorithm by adjusting the size of the training dataset. To do so, slice your data into different periods. Rerun the notebook with the updated parameters, and record the results in your README.md file. 
    
![Data Offset - 3 months](https://user-images.githubusercontent.com/106201726/188072311-0ba3f576-8623-4c6c-a2da-1c8b0ead9455.png)
![Data Offset - 15 months](https://user-images.githubusercontent.com/106201726/188072319-61f90f01-097a-4082-b546-dc3dff660a69.png)
![Data Offset - 25 months](https://user-images.githubusercontent.com/106201726/188072368-d080f63d-2488-4af9-b236-415e44cbce8a.png)

Answer the following question: What impact resulted from increasing or decreasing the training window? Increasing the size of the training dataset brought the actual and strategy returns closer together, indicationg to me this algorithm is particularly good at predicting performance over the long term. Decreasing the size of the dataset widened the gap between the actual and strategy returns.

    Hint To adjust the size of the training dataset, you can use a different DateOffset value—for example, six months. Be aware that changing the size of the training dataset also affects the size of the testing dataset.

    Tune the trading algorithm by adjusting the SMA input features. Adjust one or both of the windows for the algorithm. Rerun the notebook with the updated parameters, and record the results in your README.md file. 

![short_window-30_long_window-30 Screenshot 2022-09-01 212952](https://user-images.githubusercontent.com/106201726/188072710-0c423ffe-8ae3-4633-9dd4-51b4feb3f5ed.png)
![short_window-30_long_window-250 Screenshot 2022-09-01 212952](https://user-images.githubusercontent.com/106201726/188072753-eff79698-da64-4fad-b7e1-3dca47fed68a.png)
![short_window-250_long_window-250 Screenshot 2022-09-01 212952](https://user-images.githubusercontent.com/106201726/188072786-cb8be8ad-f54f-404c-8045-38166082e4f0.png)
  
    Answer the following question: What impact resulted from increasing or decreasing either or both of the SMA windows? In the short term changing the SMA numbers significantly affected the difference between the actual and strategy returns and increased the volatility. In the long term, there was an increase in the gap between the actual and strategy numbers, decreasing the confidence in the this model for the algorithm and it's predictive ability.

    Choose the set of parameters that best improved the trading algorithm returns. Save a PNG image of the cumulative product of the actual returns vs. the strategy returns, and document your conclusion in your README.md file. 

![Data Offset - 25 months](https://user-images.githubusercontent.com/106201726/188073816-74a0e12a-9103-485e-a184-c8b3f7044372.png)
The set of parameters that shows the closest correlation between the actual and the strategy returns is when the Data Offset is increased. The more data over time, the better the ability to more accurately predict the returns.
