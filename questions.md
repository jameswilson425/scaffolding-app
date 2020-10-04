# Step 6 files not located

app/assets/javascripts/posts.js.coffee
app/assets/stylesheets/posts.css.scss
app/assets/stylesheets/scaffolds.css.scss

# Step 6.2 no home folder found

app/views/home/index.html.erb

# Step 6.5 error in rails console. removed attr_accessible and worked fine after

Traceback (most recent call last):
4: from (irb):4
3: from (irb):5:in `rescue in irb_binding' 2: from app/models/post.rb:1:in `<main>'
1: from app/models/post.rb:2:in `<class:Post>' NoMethodError (undefined method `attr_accessible' for #<Class:0x00007f9682831f60>)
Did you mean? attr_accessor

# ^tried installing these gems but no success^

gem 'protected_attributes_continued'
gem 'strong_parameters'

# Step 6.8

<%= javascript_include_tag "application" %>

# ^caused error in browser^. updated application.html.erb with just the line:

<body style="background: #EEEEEE;">
