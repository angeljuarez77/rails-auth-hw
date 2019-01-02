# Rails-Auth-HW with Knock

For this assignment, you will be building a simple app with user authorization in Rails. You are only required to implement auth for the model. **As a bonus, incorporate another model, called _Bird_.**

## Getting Started

Fork and clone this repo.

In the terminal, in the directory where you want to create a project, generate a new Rails project and cd in to it:

```shell
rails new birds --api --database=postgresql
cd birds
```

In your Gemfile, make sure you have:

```ruby
gem 'bcrypt', '~> 3.1.7'
gem 'rack-cors'
gem 'knock'
gem 'jwt'
```

AND

```ruby
gem 'pry-rails'
```

In the terminal, from the root of the project, run `bundle install`.

### Scaffolding
Implement Auth based on today's lesson by running:

```
rails generate scaffold User email:string password_digest:string
```

**For the Bonus:**

```
rails generate scaffold Bird name:string color:string can_fly:boolean
```

### Set up DB:
In the terminal, run:

```
rails db:drop db:create db:migrate
```


Refer to [todays lesson](https://git.generalassemb.ly/wdi-nyc-octonion/rails-knock-auth/blob/master/README.md#configure-the-user-model) for setting up the User Model.

# Deliverables
- Complete this assignment with an acceptable commit history.
- Do a PR.

# Bonus
- Incorporate the birds model and check your routes in Insomnia.
