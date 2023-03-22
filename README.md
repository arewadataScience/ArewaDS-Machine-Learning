[![GitHub license](https://img.shields.io/github/license/microsoft/ML-For-Beginners.svg)](https://github.com/microsoft/ML-For-Beginners/blob/master/LICENSE)
[![GitHub contributors](https://img.shields.io/github/contributors/microsoft/ML-For-Beginners.svg)](https://GitHub.com/microsoft/ML-For-Beginners/graphs/contributors/)
[![GitHub issues](https://img.shields.io/github/issues/microsoft/ML-For-Beginners.svg)](https://GitHub.com/microsoft/ML-For-Beginners/issues/)
[![GitHub pull-requests](https://img.shields.io/github/issues-pr/microsoft/ML-For-Beginners.svg)](https://GitHub.com/microsoft/ML-For-Beginners/pulls/)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)

[![GitHub watchers](https://img.shields.io/github/watchers/microsoft/ML-For-Beginners.svg?style=social&label=Watch)](https://GitHub.com/microsoft/ML-For-Beginners/watchers/)
[![GitHub forks](https://img.shields.io/github/forks/microsoft/ML-For-Beginners.svg?style=social&label=Fork)](https://GitHub.com/microsoft/ML-For-Beginners/network/)
[![GitHub stars](https://img.shields.io/github/stars/microsoft/ML-For-Beginners.svg?style=social&label=Star)](https://GitHub.com/microsoft/ML-For-Beginners/stargazers/)

# Machine Learning for Beginners - A Curriculum

> 🌍 Travel around the world as we explore Machine Learning by means of world cultures 🌍

Arewa Datascience presents this 10-week online course, as part of the Arewa Datascience Fellowship. The contents of the course are adopted from Microsoft's ['ML-For-Beginners'](https://github.com/microsoft/ML-For-Beginners) and ['DS-For Beginners'](https://github.com/microsoft/Data-Science-For-Beginners) courses. In this curriculum, you will learn about **data manipulation (preprocessing and visualization)** and **classical machine learning**, using pandas and Scikit-learn libraries. The curriculum does not include deep-learning, as it is anticipated to be covered in the future (during the second cohort).

We acknowledge the content creators in [THANKS.md](THANKS.md)

# Getting Started

**[Fellows](https://arewadatascience.org/fellows.html)**, to use this curriculum, fork the entire repo to your own GitHub account and complete the exercises on your own or with a group:

- Start with a pre-lecture quiz.
- Read the lecture and complete the activities, pausing and reflecting at each knowledge check.
- Try to create the projects by comprehending the lessons rather than running the solution code; however that code is available in the `/solution` folders in each project-oriented lesson.
- Take the post-lecture quiz.
- Complete the challenge.
- Complete the assignment.
- After completing a lesson group, visit the [Telegram Group](https://t.me/c/1892169859/1) and "learn out loud" by writing about the new knowledge you gained. Don't forget to write a [medium](https://medium.com) blog post at the end of this course.

**Teachers**, we have [included some suggestions](for-teachers.md) on how to use this curriculum.

---

## Pedagogy

We have chosen two pedagogical tenets while building this curriculum: ensuring that it is hands-on **project-based** and that it includes **frequent quizzes**. In addition, this curriculum has a common **theme** to give it cohesion.

By ensuring that the content aligns with projects, the process is made more engaging for students and retention of concepts will be augmented. In addition, a low-stakes quiz before a class sets the intention of the student towards learning a topic, while a second quiz after class ensures further retention. This curriculum was designed to be flexible and fun and can be taken in whole or in part. The projects start small and become increasingly complex by the end of the 12-week cycle. This curriculum also includes a postscript on real-world applications of ML, which can be used as extra credit or as a basis for discussion.

> Find our [Code of Conduct](CODE_OF_CONDUCT.md), [Contributing](CONTRIBUTING.md), and [Translation](TRANSLATIONS.md) guidelines. We welcome your constructive feedback!

## Each lesson includes:

- optional sketchnote
- optional supplemental video
- pre-lecture warmup quiz
- written lesson
- for project-based lessons, step-by-step guides on how to build the project
- knowledge checks
- a challenge
- supplemental reading
- assignment
- post-lecture quiz

> **A note about languages**: These lessons are primarily written in Python, but many are also available in R. To complete an R lesson, go to the `/solution` folder and look for R lessons. They include an .rmd extension that represents an **R Markdown** file which can be simply defined as an embedding of `code chunks` (of R or other languages) and a `YAML header` (that guides how to format outputs such as PDF) in a `Markdown document`. As such, it serves as an exemplary authoring framework for data science since it allows you to combine your code, its output, and your thoughts by allowing you to write them down in Markdown. Moreover, R Markdown documents can be rendered to output formats such as PDF, HTML, or Word.

> **A note about quizzes**: All quizzes are contained [in this app](https://gray-sand-07a10f403.1.azurestaticapps.net/), for 52 total quizzes of three questions each. They are linked from within the lessons but the quiz app can be run locally; follow the instruction in the `quiz-app` folder.

| Week | Topic | Lesson Grouping | Learning Objectives | Linked Lesson | Author |
| :-------: | ------------- | --------------- | -------------------- | --------------------- | ------------------ |
|      01       |                Introduction to machine learning                |      [Introduction](1-Introduction/README.md)       | Learn the basic concepts behind machine learning | <ul> <li>[Introduction](1-Introduction/1-intro-to-ML/README.md)</li> <li>[History](1-Introduction/2-history-of-ML/README.md)</li> <li>[Fairness](1-Introduction/3-fairness/README.md)</li> <li>[Techniques](1-Introduction/4-techniques-of-ML/README.md)</li> </ul> | <ul><li>Muhammad</li><li>Jen </li><li> Amy</li><li>Tomomi</li><li>Chris</li></ul>                       |
| 02 | Working with Data | [Working With Data](2-Working-With-Data/README.md) | Introduction to relational data and non-relational data, pandas and data preparation | <ul><li>[Relational data](2-Working-With-Data/05-relational-databases/README.md)</li><li>[Non-Relational data](2-Working-With-Data/06-non-relational/README.md)</li><li>[Python libraries](2-Working-With-Data/07-python/README.md) </li><li>[lesson](2-Working-With-Data/08-data-preparation/README.md)</li></ul> | <ul><li>Christopher</li><li>Jasmine</li><li>Dmitry</li></ul> |
| 03 | Data Visualization | [Data Visualization](3-Data-Visualization/README.md) | Introduction to Matplotlib, Data Distributions, Proportions and Relationships and Meaningful Visualizations - bird data 🦆 | <ul><li>[Quantities](3-Data-Visualization/09-visualization-quantities/README.md)</li> <li>[Distributions](3-Data-Visualization/10-visualization-distributions/README.md)</li><li>[Proportions](3-Data-Visualization/11-visualization-proportions/README.md)</li><li>[Relationships](3-Data-Visualization/12-visualization-relationships/README.md)</li><li>[Meaningful Visualizations](3-Data-Visualization/13-meaningful-visualizations/README.md)</li></ul> | <ul><li>Jen</li></ul> |
| 04 | Regression | [Regression](2-Regression/README.md) | Tools, Data Visualization and Regression Models - North American pumpkin prices 🎃 | <ul><li>[Tools](2-Regression/1-Tools/README.md)</li><li>[Data preprocessing](2-Regression/2-Data/README.md)</li><li>[Linear Regression](2-Regression/3-Linear/README.md)</li><li>[Logistic Regression](2-Regression/4-Logistic/README.md) </li></ul> | <ul><li>Jen </li><li> Dmitry</li></ul> |
| 05 | Classification | [Classification](4-Classification/README.md)     | Data preprocessing, classifiers - Delicious Asian and Indian cuisines 🍜 | <ul><li> [Introduction](4-Classification/1-Introduction/README.md) </li> <li> [Classifiers 1](4-Classification/2-Classifiers-1/README.md)</li> <li> [Classifiers 2](4-Classification/3-Classifiers-2/README.md)</li> <li> [Recommender App](4-Classification/4-Applied/README.md) </ul> </ul> | <ul><li>Jen </li><li> Cassie</li></ul> |
| 06 | Clustering | [Clustering](5-Clustering/README.md) | Data preprocessing, clustering - Exploring Nigerian Musical Tastes 🎧 | <ul><li> [Data Visualization](5-Clustering/1-Visualize/README.md)</li> <li> [K-Means](5-Clustering/2-K-Means/README.md)</li> </ul> | <ul><li>Jen</li></ul> |
| 07 | Natural language processing ☕️ |   [Natural language processing](6-NLP/README.md)    | Learn the basics about NLP by building a simple bot | <ul> <li> [Introduction](6-NLP/1-Introduction-to-NLP/README.md) </li> <li> [Common Tasks](6-NLP/2-Tasks/README.md) </li> <li> [Translation](6-NLP/3-Translation-Sentiment/README.md) </li> </ul> | <ul> <li> Stephen </li> </ul> |
| 08 | Sentiment Analysis | [Natural language processing](6-NLP/README.md) | Sentiment analysis with hotel reviews | <ul> <li> [Hotel Reviews 1](6-NLP/4-Hotel-Reviews-1/README.md) </li> <li> [Hotel Reviews 2](6-NLP/5-Hotel-Reviews-2/README.md) </li> </ul> | <ul> <li> Stephen </li> </ul> |
| 09 | Time Series Forecasting | [Time series](7-TimeSeries/README.md) | Introduction, ARIMA, Support Vector Regressor (SVR) - ⚡️ World Power Usage ⚡️ | <ul><li> [Introduction](7-TimeSeries/1-Introduction/README.md) </li> <li> [ARIMA](7-TimeSeries/2-ARIMA/README.md) </li> <li> [SVR](7-TimeSeries/3-SVR/README.md) </li> </ul> | <ul> <li> Francesca </li> <li> Anirban </li> </ul> |
| 10 | Reinforcement Learning | [Reinforcement learning](8-Reinforcement/README.md) | Introduction, Reinforcement learning with Q-Learning and Gym | <ul><li>[Q-Learning](8-Reinforcement/1-QLearning/README.md)</li> <li>[Gym](8-Reinforcement/2-Gym/README.md)</li></ul> | <ul> <li> Dmitry </li> </ul> |
| Projects | Real-World ML scenarios and applications | [ML in the Wild](9-Real-World/README.md) | Interesting and revealing real-world applications of classical ML | [Lesson](9-Real-World/1-Applications/README.md) | <ul> <li> Team  </li> </ul> |

## Offline access

You can run this documentation offline by using [Docsify](https://docsify.js.org/#/). Fork this repo, [install Docsify](https://docsify.js.org/#/quickstart) on your local machine, and then in the root folder of this repo, type `docsify serve`. The website will be served on port 3000 on your localhost: `localhost:3000`.

## PDFs

Find a pdf of the curriculum with links [here](https://microsoft.github.io/ML-For-Beginners/pdf/readme.pdf).

## Help Wanted!

Would you like to contribute a translation? Please read our [translation guidelines](TRANSLATIONS.md) and add a templated issue to manage the workload [here](https://github.com/microsoft/ML-For-Beginners/issues).
