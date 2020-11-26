# Rails Textbook 

## Online Question and Asnwers

* Question <br/>

    What are the ERB tags that are used the most in rails?
    
* Answer

    - There are two ERB tags that you need to remember:<br/>
    > ```ruby
    > <%= ruby_code %>
    >```
    Example : 
    
    >```ruby 
    >  <%= @product.price %> 
    >```
    >It runs the Ruby code and inserts the result to the HTML at that position. You can put any kind of Ruby code between `<%= and %>`, for instance, `<%= 9 * 3 %>` will translate to 27 in the page that the user is viewing. However, typically this tag is used to display some data from a model, such as the price of a product, as shown in the example here.

    **and**
    
    > ```ruby
    > <% ruby_code %>
    >```
    Example : 
    
    >```ruby
    >   <% if user.admin? %>
    >     <p>Hello Admin!</p>
    >   <% end %>
    >```
    >The Ruby code between the delimiters `<%` and `%>` is run but the result will not be inserted at this point in the HTML. Therefore these tags are most commonly used for control flow structures such as an if statement in the example, or loops.

    Notice that the difference is the = in the first tag. <br/>

* Question <br/>

    How does Ruby on Rails use the Model View Controller (MVC) framework?

* Answer <br/>

    - Web development can often be divided into three separate but closely integrated subsystems:<br/>

    >**Model (Active Record)**: The model handles all the data logic of the application. In Rails, this is handled by the Active Record library, which forms the bridge between the Ruby program code and the relational database.

    >**View (Action View)**: The view is the part of the application that the end user sees. In Rails, this is implemented by the Action View library, which is based on Embedded Ruby (ERB) and determines how data will be presented.

    >**View (Action View)**: The view is the part of the application that the end user sees. In Rails, this is implemented by the Action View library, which is based on Embedded Ruby (ERB) and determines how data will be presented.    

* Question <br/>

    What is a Rails Migration? <br/>
    Write up a short example of a simple Rails Migration with a table called customers, a string column called name, and a text column called description.

* Answer <br/>
    - A Rails Migration can be used to create, drop, or remove tables and columns.
    - To generate a migration file `rails generate migration table_name` will create it.

    >```ruby
    >    class CreateCustomers < ActiveRecord::Migration
    >        def up
    >            create_table :customers do |t|
    >            t.string :name
    >            t.text :description
    >        
    >            t.timestamps
    >            end
    >        end
    >        
    >        def down
    >            drop_table :customers
    >        end
    >    end
    >```
