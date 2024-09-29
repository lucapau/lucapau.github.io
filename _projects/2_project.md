---
layout: page
title: Restaurant Review App
description: A full-stack web application for browsing, reviewing, and managing restaurants.
img: assets/img/RestaurantReview.PNG
importance: 1
category: work
related_publications: false
---

The Restaurant Review App is a dynamic platform built with Django, designed to connect users and restaurant owners. Whether you're looking for a place to eat, writing a review, or managing your restaurant's page, the app offers tailored features for each type of user.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Indexpage.PNG" title="Browse Restaurants" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/restaurantpage.PNG" title="Restaurant Page" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Showcase of features: Left - Browse Restaurants, Right - Individual Restaurant Pages with Reviews and Details.
</div>

### Key Features

- **Browse Restaurants**: View all restaurants, with a filter to refine results by cuisine type.
- **Restaurant Pages**: Each restaurant has its own page showing reviews, location (with an interactive map), menu, and other relevant details.
- **User Reviews**: Registered users can write one review per restaurant. Reviews are visible to all users to aid decision-making.

### User Roles

- **No Account**: Guests can browse restaurants and view details like reviews and location, but can't leave reviews.
- **User Account**: Users can sign in to write reviews, limited to one per restaurant, and save favorite restaurants.
- **Owner Account**: Restaurant owners can manage their restaurant's page by updating menu, location, details, and responding to reviews.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/userreviewpage.PNG" title="User Reviews" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/ownerreviewresponse.PNG" title="Restaurant Management" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left - User Reviews, Right - Restaurant Management for Owners.
</div>

### Additional Features

- **Main Window**: A central list of restaurants with an easy-to-use filter for cuisine type.
- **Restaurant Creation**: Restaurant owners can create and manage restaurant profiles, including menu, location, and responding to customer reviews.

```html
<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/restaurantsignup.PNG" title="Restaurant Signup" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/ownerreviewresponse.PNG" title="Owner Response" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
