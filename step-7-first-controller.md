resoureces :books will give

get     '/api/v1/books'           => "api/v1/books#index",    as: api_v1_books

rails will expect a controller in this path => "api/v1/books#index".

It is throwing error because if is unable to find books controller and index action in it under api/v1 module

let us create api/v1 module first and then create our first controller i.e books controller.rb

EMBED code/books_controller_1.png

Let us run it again

$ rspec spec/requests/api/v1/books_spec.rb

EMBED results/request_spec_result_3.png

The action 'index' could not be found for Api::V1::BooksController

We haven't defined the action index.
Let us do it.

EMBED code/books_controller_2.png

Let us run it again

$ rspec spec/requests/api/v1/books_spec.rb

EMBED request_spec_result_4.png

Missing template api/v1/books/index

