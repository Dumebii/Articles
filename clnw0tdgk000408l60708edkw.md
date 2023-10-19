---
title: "An Introduction to Ruby"
seoTitle: "A guide to learning Ruby programming language"
seoDescription: "Learn Ruby development, data types in Ruby, string methods, operators in Ruby and build cool beginner projects in Ruby."
datePublished: Wed Oct 18 2023 17:22:07 GMT+0000 (Coordinated Universal Time)
cuid: clnw0tdgk000408l60708edkw
slug: an-introduction-to-ruby
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1697649624663/46e5a6fe-a42a-4e7f-9e25-992b691e37f9.png
tags: newbie, ruby, web-development, ruby-on-rails, beginners

---

Hello and welcome to my Ruby chronicles👋🏾

![welcome](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/gdia2a8s3vc5a5xobu1e.gif align="left")

I am going to chronicle my Ruby learning journey here. I am starting my learning using this [tutorial](https://www.youtube.com/watch?v=MXlZCgh2M6A&t=39s&pp=ygUbcnVieSB0dXRvcmlhbCBmb3IgYmVnaW5uZXJz) I found on YouTube.

## What is Ruby?

Ruby, a dynamic, high-level, and object-oriented programming language, is about to take you on an exhilarating journey into the world of software development. Picture a world where coding is not just a task but a creative adventure, and Ruby is your trusty companion. **Developed by the visionary Yukihiro "Matz" Matsumoto in the mid-1990s**, Ruby has become synonymous with elegance and flexibility in the programming universe.

In this article, I'll give a brief but insightful introduction to get you started coding in Ruby. We will also be completing two coding exercises in this article. Prepare to be awestruck by the simplicity and readability of Ruby as it empowers you to unlock your coding potential and embark on a thrilling journey in the ever-evolving landscape of programming. Let's get started on this exciting ride!

## Why should you learn Ruby

* **Elegant and Readable Code:** Ruby's clean and human-readable syntax makes it an excellent choice for beginners and seasoned programmers alike.
    
* **Versatile Language:** Ruby can be used for web development, scripting, game development, and more, offering a wide range of applications.
    
* **Strong Community:** There's a supportive and active Ruby community that provides ample resources and assistance for learners.
    
* **Ruby on Rails:** Ruby is the language behind Ruby on Rails, a popular web framework that simplifies web application development.
    
* **Object-Oriented:** Ruby is a pure object-oriented language, which encourages good programming practices and code reusability.
    
* **Productivity:** Ruby's focus on developer productivity means you can build applications faster, making it a valuable skill in the workforce.
    
* **Market Demand:** Ruby developers are in demand, and learning Ruby can open up job opportunities in the tech industry.
    
* **Integration:** Ruby easily integrates with other technologies, making it a valuable addition to a programmer's toolkit.
    
* **Fun and Creative:** Ruby encourages a playful and creative approach to programming, making it an enjoyable language to work with.
    
* **Continuous Evolution:** Ruby continues to evolve with new versions and updates, ensuring its relevance in modern software development.
    

## Difference between Ruby and Ruby on Rails

![Ruby vs rails](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/fkk2xgivfrnb4cjp0fzr.jpg align="left")

Ruby and Ruby on Rails are often mentioned together, but they serve different purposes in the world of web development.

**Ruby:**

* Ruby is a dynamic, high-level programming language.
    
* It's the foundation upon which Ruby on Rails is built.
    
* Used for various types of software development beyond web applications.
    
* Known for its elegant and human-friendly syntax.
    
* Offers flexibility and ease of learning.
    

**Ruby on Rails:**

* Ruby on Rails, often referred to as Rails, is a web application framework.
    
* Built using the Ruby language, it's designed specifically for creating web applications.
    
* Provides a structured and opinionated framework for developing web apps.
    
* Offers features like an ORM (Object-Relational Mapping), routing, and MVC (Model-View-Controller) architecture to streamline development.
    
* Known for its "convention over configuration" approach, which simplifies development
    

## Setting up Ruby

To download Ruby on your local computer, visit the [installation page](https://rubyinstaller.org/downloads) to download and setup Ruby.

### Setting up the Ruby environment

So far in my learning journey, this has been the most challenging obstacle I encountered.

In the tutorial I highlighted earlier, [Aptana studios](https://github.com/aptana/studio3/releases) is the IDE (development environment) being used to execute Ruby files. I, however, had issues running Aptana on my Windows laptop, as the tutorial only covered getting Aptana for MacOS. I ended up not using it.

I tried running Ruby on VS Code, but I was not getting the proper installation or configuration needed for the `rbenv`.

I eventually settled for [RubyMine](https://www.jetbrains.com/ruby/promo/?source=google&medium=cpc&campaign=EMEA_en_AFRICA_RubyMine_Search&term=ruby%20programming&content=603029164739&gad=1&gclid=Cj0KCQjwsp6pBhCfARIsAD3GZubLOZvEt98iiDN2G8wPj9TjubsKHzipSo730cUOZcKieSZl4-WFDK0aAtP7EALw_wcB) from @jetbrains.

### Interactive Ruby Shell (IRB)

![Interactive Ruby Shell](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/2os5gr9ehhii5u6seqab.png align="left")

The Ruby Interactive Shell, often abbreviated as IRB, is a powerful and versatile tool for developers working with the Ruby programming language. It provides an interactive environment for writing and executing Ruby code snippets, making it an indispensable resource for learning, testing, and experimenting with Ruby. IRB is a valuable tool for both beginners and experienced Ruby developers. It offers a playground for experimenting with code, testing ideas, and gaining a deeper understanding of the Ruby language and its features. Whether you're a seasoned developer or just starting your coding journey, IRB is a handy companion for your Ruby programming adventures.

#### How to Use IRB:

Using IRB is straightforward. Here are the basic steps:

* Open a terminal or command prompt depeneind on your operating system.
    
* Type `irb` and press the `Enter` key. This launches the Ruby Interactive Shell.
    
* Start entering Ruby code, and IRB will execute it immediately and display the results.
    
* You can exit IRB by typing exit or pressing `Cmd+D` (Ctrl+Z on Windows) or simply typing `quit` on the terminal.
    

## Data types in Ruby

Imagine that data types in Ruby are like different kinds of toys. Each toy is used for something special.

1. **Strings:** They are like your favorite storybook. They have letters and words.
    
2. **Integers:** These are like your counting blocks. They are just numbers you can count on.
    
3. **Floats:** These are like your toys that have numbers with dots, like 1.5. They're for numbers with parts like a half.
    
4. **Booleans:** They are like a yes/no button. You can say 'yes' or 'no' to them.
    
5. **Arrays:** Imagine you have a box of crayons. It's like an array of colors. Each crayon is a different color.
    
6. **Hashes:** They are like a special box with labels. You put things in boxes and label them to find them easily.
    
7. **Symbols:** They are like little flags. You use them to show special things, like a flag for your favorite color.
    
8. **Nil:** It's like when you don't have any toys at all. There's nothing there.
    
9. **Regular Expressions:** These are like magic patterns. You can use them to find things that look a certain way in your toys or stories.
    
10. **Ranges:** They are like numbers in a line. You can say, "I want numbers from 1 to 10," and you get all the numbers in between.
    

## Ruby Nuggets

This is a compilation of things I have learned in Ruby that I don't know how to group.

* Ruby files are saved with the extension `.rb`
    
* Comments in Ruby are made using the `#` sign.
    
* To output or display Ruby code on the console/terminal, we use `puts`, `print`, or `p`.
    
    ```ruby
    puts 'This is a line of code.'
    #output
    >>ruby: "This is a line of code."
    
    print 'This is a line of code.'
    #output
    >>ruby: "This is a line of code."
    ```
    
* `gets.chomp` is used to receive input.
    
    ```ruby
    print 'What is your message?'
    message = gets.chomp
    
    #output
    >>ruby: What is your message?_
    ```
    
* The difference between `puts` and `print` is that `puts` adds a new line character at the end of the printed value, while `print` doesn't add anything.
    
* Ruby is case-sensitive.
    
* Variable names cannot start with numbers but can contain numbers at the end.
    
* Signs are not allowed in variable names, except the underscore.
    
* Ruby supports parallel assignments.
    
    ```ruby
    a, b = 1,2
    
    puts a
    #output 
    >>ruby: 1
    
    puts b
    #output
    >>ruby: 2
    ```
    
* Ruby is an OOP (Object Oriented Programming) language, which means that everything in Ruby is an object.
    
* `<<` is used to append data types to each other.
    

## Operators in Ruby

`+` -- Addition

`-` -- subtraction

`*` -- multiplication

`/` -- division

`**` -- exponent

`%` -- modulus

## String properties in Ruby

We have a sample string, `message = "John is a boy.`

* `.length`: this returns the number of characters contained in the string.
    

`message.length = 14`

* `.upcase`: this converts all the letters in the string to the upcase.
    

`message.upcase = "JOHN IS A BOY."`

* `.downcase`: this converts all the letters in the string to the lowercase.
    

`message.downcase = "john is a boy.`

* `.capitalize`: this capitalizes the first letter in a string.
    
* `.swapcase`: this inverts the capitalization of the string. That is, if a letter is in the uppercase, it changes it to the lowercase.
    

`message.swapcase = "jOHN IS A BOY."`

* To convert a string to an integer, we use [`string.to`](http://string.to)`_i`.
    
* To convert an integer to a string, we use [`integer.to`](http://integer.to)`_s`.
    
* To convert an integer/string to a float, we use [`integer.to`](http://integer.to)`_f` or [`string.to`](http://string.to)`_f`.
    

## Project 1

### Build a BMI calculator with Ruby

In this project, we will be building a simple BMI calculator taking into effect all that we have learnt so far. *please do not mind my BMI range 🤣🤣*

```ruby
 puts 'BMI calculator'
 puts 'This is the BMI range'
 puts '=<18 -- underweight'
 puts '>=40 -- overweight'
 puts 'Anywhere in between is good enough for me.'
 print 'Height(cm):'
 height = gets.chomp.to_f
 print 'Weight(kg):'
 weight = gets.chomp.to_f
 BMI = weight/(height/100)**2
 puts "BMI is #{BMI}"
```

This is a sample of the code being run in the RubyMine IDE.

![Ruby input and output](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/e1fdqhqxfbek94d4h8yj.png align="left")

## Project 2

### Build a Company Email Creator in Ruby

In this project, we will write a script that will automate the creation of company emails for employees at Netflix.

```ruby
 puts 'Hello world!'
 puts 'Company Email Generator'
 print 'Employee firstname:'
 firstname = gets.chomp
 print 'Employee lastname:'
 lastname = gets.chomp
 print 'Input company name:'
 company_name = gets.chomp
 employee_email = firstname.downcase << '.' << lastname.downcase 
 << '@' << company_name.downcase << '.com'
 puts employee_email
```

![employee email](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/6r17tz3abi2xm4r48znk.png align="left")

Notice that in this last example, we used some string properties like the `.downcase` to ensure that regardless of what our user inputs, it will return the desired outcome in uppercase. We also used the `<<` append method.

That will be all for today! See you next time.

![goodbye gif](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/4fbpoc88su194bommwfw.gif align="left")

[Cover image](https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.devopsschool.com%2Fblog%2Fwhat-is-ruby-and-how-it-works-an-overview-and-its-use-cases%2F&psig=AOvVaw2YtN8vEWoCu8ce_0R9FPo0&ust=1697732516581000&source=images&cd=vfe&opi=89978449&ved=0CBMQjhxqFwoTCKD5zdSAgIIDFQAAAAAdAAAAABAR)

[Ruby vs Ruby on Rails](https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.appventurez.com%2Fblog%2Fruby-vs-ruby-on-rails&psig=AOvVaw1E8h4Rx_IEiny0dFVADJfO&ust=1697732641521000&source=images&cd=vfe&opi=89978449&ved=0CBMQjhxqFwoTCOjf8I6BgIIDFQAAAAAdAAAAABAE)