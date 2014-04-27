## The Path to Enlightenment
============================

### These instructions are for *nix platforms.

* You can run the tests by calling the command `ruby path_to_enlightenment.rb` file.

* In your terminal, while in the ruby_koans directory, type:

* [ path_to_ruby_koans ] $ ruby path_to_enlightenment.rb

Red, Green, Refactor
In test-driven development (TDD) the mantra has always been red: write a failing test and run it, green: make the test pass, and refactor: look at the code and see if you can make it any better.

With the koans, you will need to run the tests and see it fail (red), make the test pass (green), then take a moment and reflect upon the test to see what it is teaching you and improve the code to better communicate its intent (refactor).

The very first time you run it you will see the following output:

* [ ruby_koans ] $ ruby path_to_enlightenment.rb
* (in /Users/person/dev/ruby_koans)
* cd koans

Thinking AboutAsserts
test_assert_truth has damaged your karma.

You have not yet reached enlightenment ...
<false> is not true.

Please meditate on the following code:
* ./about_asserts.rb:10:in `test_assert_truth'
* path_to_enlightenment.rb:27

mountains are merely mountains

You have come to the first error. Notice you are told where to look for the error:

Please meditate on the following code:
./about_asserts.rb:10:in `test_assert_truth'
path_to_enlightenment.rb:27

You then open up the about_asserts.rb file in your text editor and look at line 10:

# We shall contemplate truth by testing reality, via asserts.
`def test_assert_truth'
  'assert false # This should be true'
'end`

You then change false to true and run the tests again. You should get a new error.

Before moving on, think about what you are learning.

In this specific case, ignore everything except the method name (test_assert_truth) and the parts inside the method (everything before the end). The goal is for you to see that if you pass a value to the assert method, it will either ensure it is true and continue on, or fail if in fact the statement is false.