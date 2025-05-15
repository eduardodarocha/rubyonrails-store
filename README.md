# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

1. [ x ] [Introduction](#introduction)
2. [ x ] [Rails Philosophy](#rails-philosophy)
3. [ x ] [Creating a New Rails App](#creating-a-new-rails-app)
  3.1. [ x ] [Prerequisites](#prerequisites)

  3.2. [ x ] [Creating Your First Rails App](#creating-your-first-rails-app)

  3.3. [ x ] [Directory Structure](#directory-structure)

  3.4. [ x ] [Model-View-Controller Basics](#model-view-controller-basics)

4. [ x ] [Hello, Rails!](#hello-rails-bang)
  4.1. [ x ] [Autoloading in Development](#autoloading-in-development)

5. [ x ] [Creating a Database Model](#creating-a-database-model)
  5.1. [ x ] [Database Migrations](#database-migrations)

  5.2. [ x ] [Running Migrations](#running-migrations)

6. [ ] [Rails Console](#rails-console)

7. [ ] [Active Record Model Basics](#active-record-model-basics)
  7.1. [ ] [Creating Records](#creating-records)

  7.2. [ ] [Querying Records](#querying-records)

  7.3. [ ] [Filtering & Ordering Records](#filtering-ordering-records)

  7.4. [ ] [Finding Records](#finding-records)

  7.5. [ ] [Updating Records](#updating-records)

  7.6. [ ] [Deleting Records](#deleting-records)

  7.7. [ ] [Validations](#validations)

8. [ ] [A Request's Journey Through Rails](#a-request-s-journey-through-rails)

9. [ ] [Routes](#routes)
  9.1. [ ] [Parts of a URL](#parts-of-a-url)

  9.2. [ ] [HTTP Methods and Their Purpose](#http-methods-and-their-purpose)

  9.3. [ ] [Rails Routes](#rails-routes)

  9.4. [ ] [Routes Command](#routes-command)

10. [ ] [Controllers & Actions](#controllers-actions)
  10.1. [ ] [Making Requests](#making-requests)

  10.2. [ ] [Instance Variables](#instance-variables)

  10.3. [ ] [CRUD Actions](#crud-actions)

  10.4. [ ] [Showing Individual Products](#showing-individual-products)

  10.5. [ ] [Creating Products](#creating-products)

  10.6. [ ] [Editing Products](#editing-products)

  10.7. [ ] [Deleting Products](#deleting-products)

11. [ ] [Adding Authentication](#adding-authentication)
  11.1. [ ] [Adding Log Out](#adding-log-out)
    
  11.2. [ ] [Allowing Unauthenticated Access](#allowing-unauthenticated-access)
    
  11.3. [ ] [Showing Links for Authenticated Users Only](#showing-links-for-authenticated-users-only)

12. [ ] [Caching Products](#caching-products)

13. [ ] [Rich Text Fields with Action Text](#rich-text-fields-with-action-text)

14. [ ] [File Uploads with Active Storage](#file-uploads-with-active-storage)

15. [ ] [Internationalization (I18n)](#internationalization-i18n)

16. [ ] [Adding In Stock Notifications](#adding-in-stock-notifications)
  16.1. [ ] [Basic Inventory Tracking](#basic-inventory-tracking)

  16.2. [ ] [Adding Subscribers to Products](#adding-subscribers-to-products)

  16.3. [ ] [In Stock Email Notifications](#in-stock-email-notifications)

  16.4. [ ] [Extracting a Concern](#extracting-a-concern)

  16.5. [ ] [Unsubscribe Links](#unsubscribe-links)

17. [ ] [Adding CSS & JavaScript](#adding-css-javascript)
  17.1. [ ] [Propshaft](#propshaft)

  17.2. [ ] [Import Maps](#import-maps)

  17.3. [ ] [Hotwire](#hotwire)

18. [ ] [Testing](#testing)
  18.1. [ ] [Fixtures](#fixtures)

  18.2. [ ] [Testing Emails](#testing-emails)

19. [ ] [Consistently Formatted Code with RuboCop](#consistently-formatted-code-with-rubocop)

20. [ ] [Security](#security)

21. [ ] [Continuous Integration with GitHub Actions](#continuous-integration-with-github-actions)

22. [ ] [Deploying to Production](#deploying-to-production)
  22.1. [ ] [Adding a User to Production](#adding-a-user-to-production)

  22.2. [ ] [Background Jobs using Solid Queue](#background-jobs-using-solid-queue)

23. [ ] [What's Next?](#what-s-next-questionmark)

Sinta-se à vontade para marcar ou atualizar os itens enquanto avança! Se precisar de ajuda com algum dos tópicos, posso oferecer explicações ou orientações. 😉

1. [Introduction](#introduction)
  - Instal Ruby on Ubuntu https://guides.rubyonrails.org/v8.0/install_ruby_on_rails.html#install-ruby-on-ubuntu
  - Install Ruby on Windows https://guides.rubyonrails.org/v8.0/install_ruby_on_rails.html#install-ruby-on-windows
2. [Rails Philosophy](#rails-philosophy)
  - Instal Rails https://guides.rubyonrails.org/v8.0/install_ruby_on_rails.html#install-rails
3. [Creating a New Rails App](#creating-a-new-rails-app)
   - [Prerequisites](#prerequisites)
   - [Creating Your First Rails App](#creating-your-first-rails-app)
   - [Directory Structure](#directory-structure)
   - [Model-View-Controller Basics](#model-view-controller-basics)
4. [Hello, Rails!](#hello-rails-bang)
   - [Autoloading in Development](#autoloading-in-development)
5. [Creating a Database Model](#creating-a-database-model)
   - [Database Migrations](#database-migrations)
   - [Running Migrations](#running-migrations)
6. [Rails Console](#rails-console)
7. [Active Record Model Basics](#active-record-model-basics)
   - [Creating Records](#creating-records)
   - [Querying Records](#querying-records)
   - [Filtering & Ordering Records](#filtering-ordering-records)
   - [Finding Records](#finding-records)
   - [Updating Records](#updating-records)
   - [Deleting Records](#deleting-records)
   - [Validations](#validations)
8. [A Request's Journey Through Rails](#a-request-s-journey-through-rails)
9. [Routes](#routes)
   - [Parts of a URL](#parts-of-a-url)
   - [HTTP Methods and Their Purpose](#http-methods-and-their-purpose)
   - [Rails Routes](#rails-routes)
   - [Routes Command](#routes-command)
10. [Controllers & Actions](#controllers-actions)
    - [Making Requests](#making-requests)
    - [Instance Variables](#instance-variables)
    - [CRUD Actions](#crud-actions)
    - [Showing Individual Products](#showing-individual-products)
    - [Creating Products](#creating-products)
    - [Editing Products](#editing-products)
    - [Deleting Products](#deleting-products)
11. [Adding Authentication](#adding-authentication)
    - [Adding Log Out](#adding-log-out)
    - [Allowing Unauthenticated Access](#allowing-unauthenticated-access)
    - [Showing Links for Authenticated Users Only](#showing-links-for-authenticated-users-only)
12. [Caching Products](#caching-products)
13. [Rich Text Fields with Action Text](#rich-text-fields-with-action-text)
14. [File Uploads with Active Storage](#file-uploads-with-active-storage)
15. [Internationalization (I18n)](#internationalization-i18n)
16. [Adding In Stock Notifications](#adding-in-stock-notifications)
    - [Basic Inventory Tracking](#basic-inventory-tracking)
    - [Adding Subscribers to Products](#adding-subscribers-to-products)
    - [In Stock Email Notifications](#in-stock-email-notifications)
    - [Extracting a Concern](#extracting-a-concern)
    - [Unsubscribe Links](#unsubscribe-links)
17. [Adding CSS & JavaScript](#adding-css-javascript)
    - [Propshaft](#propshaft)
    - [Import Maps](#import-maps)
    - [Hotwire](#hotwire)
18. [Testing](#testing)
    - [Fixtures](#fixtures)
    - [Testing Emails](#testing-emails)
19. [Consistently Formatted Code with RuboCop](#consistently-formatted-code-with-rubocop)
20. [Security](#security)
21. [Continuous Integration with GitHub Actions](#continuous-integration-with-github-actions)
22. [Deploying to Production](#deploying-to-production)
    - [Adding a User to Production](#adding-a-user-to-production)
    - [Background Jobs using Solid Queue](#background-jobs-using-solid-queue)
23. [What's Next?](#what-s-next-questionmark)
