# Durin's Day Forecaster

Extremely useful tool for predicting Durin's Day.

>The first day of the dwarves’ New Year is, as all should know,
>the first day of the last moon of Autumn on the threshold of
>Winter. We still call it Durin’s Day when the last moon of Autumn
>and the sun are in the sky together.But this will not help us
>much, I fear, for it passes our skill in these days to guess
>when such a time will come again.
>– Thorin Oakenshield (The Hobbit)

It turns out that Tolkien never created a dwarvish calendar. However, we do know that the first day of winter according to the dwarves is November 1st. We also know that it's the last moon of autumn where the sun and the moon can both be seen in the sky. Unfortunately, calculating the latter can be very difficult so most of us Tolkien fans settle for the last new moon of Autumn.

This is exactly how my alogirthm works. Using the last new moon of autumn guarantees better foresight and accuracy.

### Get The Code

Run the following in your Nuget Package Manager:

    Install-Package DurinsDayForecaster

### Use The Code

    var durinsDay = new DurinsDayCalculator().DurinsDay(2016);

### Testing

In 2014, the author of askmiddlearth.tumblr.com (Who apparently is *not* Stephen Colbert) calculated October 23rd. I passed 2014 into my tool and got the correct output (See the `Testing` project).

A link to the post, for anyone who is interested.

http://askmiddlearth.tumblr.com/post/73200106670/how-to-predict-durins-day

Many other dates have been tested, and so far the dates I checked are accurate (Again see the `Testing` project).

#### Durin's Day Cheatsheet 2014 - 2024

For those of you who do not care about the code, and only want an answer.

| Year | Durin's Day |
| ---- | ----------- |
| 2014 | 10/23/2014  |
| 2015 | 10/13/2015  |
| 2016 | 10/30/2016  |
| 2017 | 10/20/2017  |
| 2018 | 10/9/2018   |
| 2019 | 10/28/2019  |
| 2020 | 10/16/2020  |
| 2021 | 10/6/2021   |
| 2022 | 10/25/2022  |
| 2023 | 10/14/2023  |
| 2024 | 10/2/2024   |

### Release Notes

#### Version 1.0.0.2

- Fixes never ending loop when start date happens to land on Durin's Day (Durin's Day 2024)
- Additional test coverage added

#### Version 1.0.0.1

- Removes unnecessary visibility

#### Version 1.0.0.0

- Initial release
