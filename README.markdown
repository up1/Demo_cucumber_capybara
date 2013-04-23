# Testing a remote app with Cucumber+Capybara

Instruction

    git clone https://github.com/up1/Demo_cucumber_capybara.git
    cd Demo_cucumber_capybara
    bundle install
    cucumber features
	
If you not install gem bundler
	
	gem install bundler
	

Which should produce output that looks something like:

    Feature: Using Google

      Scenario: Searching for a term # features/google.feature:3
        Given I am on google.com     # features/step_definitions/google_steps.rb:1
        When I enter "pizza"         # features/step_definitions/google_steps.rb:5
        Then I should see results    # features/step_definitions/google_steps.rb:9

    1 scenario (1 passed)
    3 steps (3 passed)
    0m4.550s

    
The project is currently configured to use `:selenium` as the default driver, but that can be changed in `/features/support/env.rb`.
