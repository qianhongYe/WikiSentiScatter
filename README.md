# WikiSentiScatter

## Introduction

This widget is used to show sentiment score including positive score and negative score for Wikipedia entities (concepts) verying with time.

Wikipedia entities contains entities in Wikipedia Article and Wikipedia Talk. Talk page is an area for editors to discuss about corresponding article, which can be visited from upper left side of article page.

This widget includes entities both People and Events. The date for people indicates birth date, while the date for events indicates occurrance date.

The text of Articles and Talks is extracted from Wikipedia Dump, and time stamps are extracted from DBPedia.

The scores are calculated with term frequency for sentiment words based on certain lexicons (OL, MPQA, LIWC, ANEW). For ANEW we take valency into account too.

## How to use it

1. You can use the link below to run this jupyter notebook with mybinder.

https://mybinder.org/v2/gh/qianhongYe/WikiSentiScatter/master

It takes around 10 mins to prepare the environment.

2. Click time_widgets_2.ipynb in the home page to open the notebook.

3. You can open Appmode to ignore the codes by clicking "Appmode" in toolbar (recommended for general user). Alternatively, you can choose "Run All" inside Cell menu without entering appmode (recommended for programmer).

Now you can operate with the widget.

## What can be seen with the widget

After selecting value for Lexicon, Group, Domain, Geolocation, Time field and click "Go" button, it comes up with plot.

For each run it plots sentiment for every entity fitting the time and area range as one circle.

Value in x-axis indicates the date (united by month) and y-axis indiates neutralized score, which means to subtract entity's negative_score from positive_score.

The size and color of the circle indicates its total score. Total score is the sum of  means sum up positive_score and negative_score. The color bar shows the the corresponding color for total score.

You can check which entity the circle present for and what its positive and negative scores are by hovering the mouse on it.

In the bottom you will get the data characteristics for the current run.

The time is splited with month as unit.

## Run it locally

If you want to run it locally, you need to install libraries listed in environment.yml with version showed in requirements.txt. Dataset can download dataset in the following link.

https://www.dropbox.com/sh/mt7by5f1wgl6n3z/AACddwkFPq5lPpH3ry83MgSDa?dl=0
