#Working with turn gem
This project is to explore by ability to bring the turn gem up to date.  The turn gem only supports minitest up to version 4.7.5.  Minitest 5.x is not supported by turn.

##Run rake tests
To run the rake test tasks, use the following syntax
<pre>
  $ rake euler20
</pre>

###Minitest output without the turn gem

```
susanmaclaptop:euler_ruby susan$ rake euler20
/Users/susan/.rvm/rubies/ruby-2.1.4/bin/ruby test/euler_20_test.rb

Factorial of 100 is: 93326215443944152681699238856266700490715968264381621468592963895217599993229915608941463976156518286253697920827223758251185210916864000000000000000000000000
The sum of those digits is: 648

Run options: --seed 50507

# Running:

...

Finished in 0.008894s, 337.2969 runs/s, 337.2969 assertions/s.

3 runs, 3 assertions, 0 failures, 0 errors, 0 skips
```

###Minitest output with the turn gem
```
susanmaclaptop:euler_ruby susan$ rake euler20
/Users/susan/.rvm/rubies/ruby-2.0.0-p247/bin/ruby test/euler_20_test.rb

Factorial of 100 is: 93326215443944152681699238856266700490715968264381621468592963895217599993229915608941463976156518286253697920827223758251185210916864000000000000000000000000
The sum of those digits is: 648

Loaded Suite test

Started at 2015-10-23 19:31:22 -0700 w/ seed 16299.

TestFindFactorial
     PASS (0:00:00.002) test_find_factorial_euler_example

TestFindFactorialSum
     PASS (0:00:00.004) test_find_factorial_sum_euler_challenge
     PASS (0:00:00.004) test_find_factorial_sum_euler_example

Finished in 0.004963 seconds.

3 tests, 3 passed, 0 failures, 0 errors, 0 skips, 3 assertions
```


##Code used for testing
The code used for testing out turn is my solution to the Project Euler problem #20.  Project Euler is a web site for practicing programming by using your language of choice to solve math problems.  Project Euler can be found here: http://projecteuler.net/problems.  My solutions can be found here: https://github.com/sprestage/euler_ruby.

