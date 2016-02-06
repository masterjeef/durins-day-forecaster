# Durin's Day Forecaster

An extremely useful tool that will predict Durin's Day.

>The first day of the dwarves� New Year is, as all should know, 
>the first day of the last moon of Autumn on the threshold of 
>Winter. We still call it Durin�s Day when the last moon of Autumn 
>and the sun are in the sky together.But this will not help us 
>much, I fear, for it passes our skill in these days to guess 
>when such a time will come again.
>� Thorin Oakenshield (The Hobbit)

It turns out that Tolkien never created a dwarvish calendar. However, we do know that the first day of winter according to the dwarves is November 1st. We also know that it's the last moon of autumn where the sun and the moon can both be seen in the sky. Unfortunately, calculating the latter can be very difficult so most Tolkien fans settle for the last new moon of Autumn.

This is exactly how my alogirthm works. Using the last new moon of autumn guarantees better foresight and accuracy.

### Get The Code

Run the following in your Nuget Package Manager:

    Install-Package DurinsDayForecaster

### Use The Code

    var durinsDay = new DurinsDayCalculator().GetDurinsDay(2016);
    
    var daysUntilDurinsDay = new DurinsDayCalculator().DaysUntilDurinsDay();

### Testing

In 2014, the following author calculated October 24. I ran that year through my tool and got the same output. So I'm assuming that with the logic stated above my calculator is fairly accurate.

http://askmiddlearth.tumblr.com/post/73200106670/how-to-predict-durins-day
