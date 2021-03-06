Gds Pivotal Card Printer
========================

This program generates a PDF file from pivotal tickets in a single iteration. The generated PDF file is A4 format with two cards per page, ready for printing.

Configuration
-------------

To use the program you need to create a configuration file ```~/.pivotal.yml``` containing:

    token: YOUR_API_TOKEN
    project_id: ID_NUMBER_OF_PROJECT
    
The token can be found on the 'profile' page in pivotal at https://www.pivotaltracker.com/profile.

The project ID number appears in the URL when accessing a project, e.g.
https://www.pivotaltracker.com/projects/500023

Usage
-----

First, install the gem dependencies:

    $ bundle install

Then you can print cards from the current iteration:

    $ ./gds_pivotal_card_printer current
    
or print cards from a specific iteration:

    $ ./gds_pivotal_card_printer iteration 5
    
