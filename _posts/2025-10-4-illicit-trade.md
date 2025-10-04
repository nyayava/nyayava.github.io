---
title: OECD and illicit trade detection 
date: 2025-10-04 03:00:00 -0500
year: 2025
layout: post
categories: [research]
tags: [policy]
languages: [en]
--- 


A [study](https://www.oecd.org/en/publications/global-trade-in-fakes_74c81154-en.html) based on 2021 global customs seizure data studied key characteristics of trade in counterfeit goods and estimated its scale, impact, and effects on the EU. 

The findings indicate that counterfeit and pirated goods accounted for **2.3%** of global trade (equivalent to USD 467 billion or 約69兆円). Within the EU, fake goods made up 4.7% of total imports. In terms of product categories, 50 out of 96 categories are affected. High-value goods such as clothing, footwear, leather products, and electronics are the top targets. The data also highlights the presence of dangerous counterfeit items, including automotive parts and pharmaceuticals. Trade routes are continuously evolving, as counterfeiters increasingly exploit international shipping channels and adopt localization strategies to produce fake goods closer to end markets. The General Trade-Related Index of Counterfeiting (GTRIC) estimates the likelihood of specific countries being major sources of counterfeit exports, with China, Bangladesh, Lebanon, the Syrian Arab Republic, and Turkey ranking high. 


<div style="margin-top: 40px;"></div>


#### How are illicit trades detected? 
Ideally, if the goal is to prevent illicit trade, all packages would be inspected, but this isn’t possible due to the sheer volume of global trade. Instead, only a small share of shipments are inspected based on risk targeting by customs officers who flag items as suspicious through documentation, profiling, or physical inspection. The study mentions some characteristics that signal suspicious shipment: 

- **Small parcels**: 79% of seizures in 2020-2021  involved parcels with fewer than 10 items. This is extremely hard to detect because invoices are vague (e.g. “stuff” or “daily necessities”) and air cargo hubs are not equipped to screen them. 

- **Localisation tactics**: Counterfeiters often ship packaging and component parts separately, or they assemble goods inside FTZs or near the destination. This strategy reduces the chance of detection and avoids scrutiny. 
There may be other signals, such as suspicious route that detours through FTZs, unusually low declared value, mismatch between reported product and image scanned product, history of sender, and so on. 


As for **risk indices** to target inspection, the GTRIC-e and GTRIC-p indices are used. GTRIC-e (economies) measures a country's (economy’s) propensity to be a source of counterfeit exports. GTRIC-p (products) measures a product category’s propensity to be prone to counterfeiting. 

From what I understand, these indices are not estimated based on statistical models, but are estimated based on summary statistics of observed data. For example, for GTRIC-p, the counterfeiting factor index is calculated based on data as the proportion of seizures of a particular product relative to the total trade volume of that product across countries. This is calculated for all product categories, so we get a sampling distribution of proportions across categories. The distribution is highly right-skewed to the right, with most products having a small index, so a log transformation is applied. A left-truncated normal distribution is then assumed to estimate the probabilities of counterfeiting a given product. 

The study use two datasets: trade data and seizure data. 
- In the trade data, each observation is defined by a product category, country pair, and year. Variables include the product code, origin and destination countries, and the value of imports. 
- The seizure data includes around 297,000 records from 2020–2021. Variables cover product category, country of origin, transport mode, value of goods, and quantity. However, there are coverage gaps, as not all customs authorities share data, and enforcement levels vary across regions. 

The report calls for improved risk profiling through the use of AI, enhanced data sharing, and closer collaboration with industries and rights holders who have expertise in identifying counterfeit goods. 


<div style="margin-top: 40px;"></div>

#### Improving detection accuracy 
It seems there are opportunities to improve detection accuracy from a data collection and modeling perspective. 

What kinds of data would be most useful to collect? Currently, they have access to basic variables like origin, destination, product type, declared value, quantity, and transport mode. Perhaps adding more granular socioeconomic indicators of the source region, beyond just the country level, could help? 

As for modeling, using statistical models to estimate the probability of a shipment being illicit based on combinations of these variables might improve accuracy. However, this is a probably very hard detection problem, regardless of additional variables we collect and refinement of modeling. Given the occurrence rate of about 2%, within the context of massive trade volumes, this is a rare event modeling. The prediction accuracy is only going to be so high. On top of that, customs officials are already stretched thin, inspecting drugs, weapons, terrorism, and other risks. 


#### Holding counterfeiter accountable 
Instead of treating this solely as a prediction or detection problem, could we also approach it from the perspective of accountability? For example, even if a small number of counterfeiters are identified, making sure that they face real consequences, such as fines, penalties, or bans from trading, could act as a deterrent and also partially address the revenue losses caused by illicit trade. We can measure the effect of such implementation. 

#### Incentives for supply and demand of counterfeit goods 
Another perspective is the incentives structure that drive counterfeiters to engage in illicit trade, as well as the demand for counterfeit goods—both intentional and unintentional. The [report](https://www.oecd.org/en/publications/why-do-countries-import-fakes_8a4a4508-en.html) examines the demand side, distinguishing between two types of consumers. Unintentional demand comes from consumers who are deceived; this group accounts for 46% of counterfeit and pirated imports. Intentional demand involves consumers who knowingly purchase counterfeits, often due to price or accessibility; this accounts for approximately 54% of counterfeit and pirated imports between 2017 and 2019. The report also identifies several factors correlated with the value of counterfeit imports. Countries with higher GDP per capita tend to import fewer fakes, while countries with better trade and transport infrastructure, and greater internet use, tertiary education, are positively correlated with higher volumes of counterfeit imports (possibly by the ability to search for good bargains online). 


#### Fake goods and fake information 
There appears to be a connection between the challenge of detecting fake products and the broader issue of fake information on digital platforms. This raises more philosophical questions: What does it mean for something to be fake, and why do fakes emerge in the first place? How are fakes detected and confirmed in each case? What is the required cost for detecting and proving something as fake? How are those responsible held accountable? And why do people buy, see value, or even spread fake goods or information—whether knowingly or not? 

