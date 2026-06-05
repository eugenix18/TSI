# AI Smart Urban Gardening Assistant (Умный городской сад)

Final project for the Building AI course

## Summary

AI Smart Urban Gardening Assistant is an app that helps city people successfully grow plants and vegetables at home. Using computer vision and analytics, the system identifies plant diseases from smartphone photos and creates watering schedules based on local microclimate data.

## Background

Many people from cities want to grow their own food to improve their well-being and environment. However, a lot number of people give up because:
* They struggle to identify plant diseases or nutrient deficiencies early enough.
* They overwater or underwater their plants, leading to plant death.

Personally, I am motivated by the idea of making cities greener.

## How is it used?

The solution is used via a simple smartphone app.

1. **Diagnosis:** A user notices yellowing leaves on their tomato plant, opens the app, and takes a photo. The AI immediately identifies the issue.

2. **Predictive Watering:** The app connects to a small, cheap soil moisture sensor and local weather forecasts to send push notifications.

![Smart Garden Concept](https://images.unsplash.com/photo-1585320806297-9794b3e4eeae?w=500)

## Data sources and AI methods

The project relies on two main types of data:
1. **Image Dataset:** Open-source datasets of plant diseases, such as the [PlantVillage Dataset](https://github.com/spMohanty/PlantVillage-Dataset), to train the computer vision model.
2. **Environmental Data:** Real-time and historical weather data fetched via APIs like the [OpenWeatherMap API](https://openweathermap.org/api), combined with user-inputted plant types.

**AI Techniques:**
* **Computer Vision (Convolutional Neural Networks - CNN):** Used for image classification to detect specific leaf diseases from user photos.
* **Regression Models / Linear Regression:** Used to predict soil drying rates based on temperature, humidity, and plant size to forecast optimal watering times.

## Challenges

What this project does notd solve:
* It cannot save a plant that is already completely dead or structurally ruined.
* Computer vision accuracy heavily depends on lighting conditions and camera quality; poor photos might lead to wrong diagnoses.

## What next?

The project could grow into a fully automated smart-home ecosystem:
* Integrating with automated water pumps (IoT) to water plants without human intervention.