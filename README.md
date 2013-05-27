<div id="table-of-contents">
<h2>Table of Contents</h2>
<div id="text-table-of-contents">
<ul>
<li><a href="#sec-1">1. Rails 4 to Heroku Step by Step</a></li>
<li><a href="#sec-2">2. <code>[2/2]</code> </a></li>
<li><a href="#sec-3">3. Reference</a>
<ul>
<li><a href="#sec-3-1">3.1. How Heroku Works</a></li>
</ul>
</li>
<li><a href="#sec-4">4. Learning</a></li>
<li><a href="#sec-5">5. Common Tasks</a>
<ul>
<li><a href="#sec-5-1">5.1. Deploying with Git</a></li>
<li><a href="#sec-5-2">5.2. Changelog</a></li>
</ul>
</li>
<li><a href="#sec-6">6. Documentation ( Heroku Dev Center )</a>
<ul>
<li><a href="#sec-6-1">6.1. Getting started</a></li>
</ul>
</li>
<li><a href="#sec-7">7. Apps</a></li>
<li><a href="#sec-8">8. Help &amp; Support</a></li>
</ul>
</div>
</div>
# Rails 4 to Heroku Step by Step

1.  [-] [Write the application](https://devcenter.heroku.com/articles/rails3#write-your-app)
    
    1.  [ ] Create a new Rails application using postgresql
        
            rails new app_name --database postgresql
    
    2.  [X] Change into the application directory
    
    3.  [X] Use PostgreSQL
        
            # Specify PostgeSQL in Gemfile
            gem 'pg'
    
    4.  [ ] Gemfile ( <https://devcenter.heroku.com/articles/rails4> )
        
            gem 'rails_log_stdout',           github: 'heroku/rails_log_stdout'
            gem 'rails3_serve_static_assets', github: 'heroku/rails3_serve_static_assets'
    
    5.  [X] Re-install dependencies to generate a new Gemfile.lock
        
            bundle install

2.  [X] Store the application in Git
    
        git init
        git add .
        git commit -m "init"

3.  <code>[2/2]</code> Deploy the application to Heroku
    
    1.  [X] Create the application on Heroku
        
            # http://murmuring-bastion-5947.herokuapp.com/ | git@heroku.com:murmuring-bastion-5947.git
            heroku create
    
    2.  [X] Deploy the code
        
            git push heroku master

4.  [ ] Visit the application

5.  [ ] View the logs

# <code>[2/2]</code> <https://devcenter.heroku.com/articles/custom-domains>

1.  [X] heroku domains:add www.example.com
        # Adding www.example.com to example... done

2.  [X] CNAME (Alias)
    
    <table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">
    
    
    <colgroup>
    <col class="left"/>
    
    <col class="left"/>
    
    <col class="left"/>
    </colgroup>
    <thead>
    <tr>
    <th scope="col" class="left">HOST NAME</th>
    <th scope="col" class="left">IP ADDRESS/URL</th>
    <th scope="col" class="left">RECORD TYPE</th>
    </tr>
    </thead>
    
    <tbody>
    <tr>
    <td class="left">weightloss</td>
    <td class="left">warm-citadel-7982.herokuapp.com.</td>
    <td class="left">CNAME (Alias)</td>
    </tr>
    </tbody>
    </table>

# Reference

## How Heroku Works

# Learning

# Common Tasks

## Deploying with Git

## Changelog

# [Documentation](https://devcenter.heroku.com/) ( Heroku Dev Center )

## [Getting started](https://devcenter.heroku.com/articles/quickstart)

1.  [ ] [Sign up](https://devcenter.heroku.com/articles/quickstart#step-1-sign-up)

2.  [ ] [Install the Heroku Toolbelt](https://devcenter.heroku.com/articles/quickstart#step-2-install-the-heroku-toolbelt)

3.  [ ] [Login](https://devcenter.heroku.com/articles/quickstart#step-3-login)

4.  [ ] [Deploy an application](https://devcenter.heroku.com/articles/quickstart#step-4-deploy-an-application)

# Apps

# Help & Support
