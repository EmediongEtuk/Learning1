# Learning1
Machine Learning with Sentiment ML.NET


﻿using Learning1;


var sampleData = new Sentiment.ModelInput()
{
     Col0 = "shotup hmm",
};


var result =  Sentiment.Predict(sampleData);


var sentiment = result.PredictedLabel == 1 ? "Postive" : "Negative";



Console.WriteLine(sentiment);
