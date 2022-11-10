# README

### TEA SUBSCRIPTION

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-this-project">About This Project</a>
      <ul>
        <li><a href="#tools-used">Tools Used</a></li>
      </ul>
    </li>
    <li>
      <a href="#how-to-use-tea-subscription">How to Use Tea Subscription Service</a>
      <ul>
        <li><a href="#download-this-repo">Download this Repo</a></li>
        <li><a href="#api-endpoints">API Endpoints</a></li>
        <li><a href="#testing">Testing</a></li>
      </ul>
  </ol>  
</details>

<!-- ABOUT THIS PROJECT -->
### About This Project
---
Tea Subscription Service is a Service Oriented Architecture, a Ruby on Rails program built to demo RESTful routes and simple database API solutions. It gives three endpoints and utilizes three separate tables. This current program can curretnly allow us to view all subscriptions and allows users to create a new subscription annd cancel a subscription.

TABLES AND ATTRIBUTES </br>

![Screenshot 2022-11-09 at 2 55 40 PM](https://user-images.githubusercontent.com/102835975/200950755-6c897088-6ede-497c-9932-e9a6de5b23a6.png)


To learn more about how to use Tea Subscription, read the "How to Use Tea Subscription Service" section below. 

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- TOOLS USED -->
### Tools Used 
---

BUILT WITH 
* [<img src="https://img.shields.io/badge/Ruby-CC342D?style=for-the-badge&logo=ruby&logoColor=white"/>](https://www.ruby-lang.org/en/) <br>
* [<img src="https://img.shields.io/badge/Ruby_on_Rails-CC0000?style=for-the-badge&logo=ruby-on-rails&logoColor=white"/>](https://rubyonrails.org/) <br>
* [<img src="https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=Postman&logoColor=white"/>](https://www.postman.com/product/what-is-postman/)<br>


TESTED WITH
* [<img src="https://img.shields.io/badge/-RSpec-red"/>](https://rspec.info/) <br>
* [<img src="https://img.shields.io/badge/-pry-brightgreen"/>](https://pry.github.io/)
* [<img src="https://img.shields.io/badge/-SimpleCov-yellow"/>](https://github.com/simplecov-ruby/simplecov)

GEMS 

* [<img src="https://img.shields.io/badge/-jsonapi--serializer-brightgreen"/>](https://github.com/jsonapi-serializer/jsonapi-serializer)
* [<img src="https://img.shields.io/badge/-Factory__Bot-brightgreen"/>](https://github.com/thoughtbot/factory_bot_rails)
* [<img src="https://img.shields.io/badge/-Faker-brightgreen"/>](https://github.com/faker-ruby/faker)

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- HOW TO USE TEA SUBSCRIPTION -->
### How to Use Tea Subscription
---

#### Download this Repo 
To install Tea Subcription locally, in your terminal run: </br>
* `git clone git@github.com:Ethan-t-n/tea_subscription.git`
* `cd tea_subscription` 
* `bundle install`

#### API Endpoints 
Tea Subscription provides three API endpoints: </br>

The first endpoint can be used for retreiving all of a customers subscription, reguardless of the status. </br>
The customer's ID must be included in the params.</br>

- `get '/api/v1/subscriptions', params: { customer_id: <customer_id> }`

The second endpoint can be used for creating a new subscription. </br>
  Subscription params are :title, :price, :status, :frequency, :tea_id, :customer_id.</br>

- `post '/api/v1/subscriptions', params: { <subscription_params> }`

The last endpoint can be used to cancel a customer's subscription, or change any other attribute of the subscription except the id. A subscription ID must be included in the params. </br>

- `patch '/api/v1/subscriptions/cancel', params: { id: <subscription_id>, status: "Cancelled" }` 

#### Testing 
To run the Tea Subscription testing suite, in your terminal run: 
* `bundle exec rspec`

<p align="right">(<a href="#top">back to top</a>)</p>


