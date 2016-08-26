# Friendly Options

This is an open source web app designed to make it easy to compare and understand stock option grants.  The web app is designed to work best for companies where stock options are not liquid (there isn't a market for buying or selling shares of the company), which generally means early or mid stage startups.  Stock option grants generally because less complicated when the value of the shares goes up.

# How to use

## Online

There is a live, up-to-date version running at https://friendlyoptions.org/

There is no tracking on the live site, nor is any of the information you enter ever sent back to the server.  The information is all stored on the client side and in the url hash.  This means you can "save" or share your page by copying the URL, however none of the information is ever sent to the server, it is only updated and parsed on the client side.

Here is [an example](https://friendlyoptions.org/#%7B%22numOptions%22%3A100000%2C%22strikePrice%22%3A0.05%2C%22numDilutedShares%22%3A10000000%2C%22numVestingMonths%22%3A48%2C%22numVestingCliff%22%3A12%2C%22optionType%22%3A%22ISO%22%2C%22optionsExpireValue%22%3A90%2C%22optionsExpireScale%22%3A%22days%22%2C%22optionsExpireEmployeeFriendly%22%3Afalse%2C%22earlyExercise%22%3Atrue%2C%22totalValuation%22%3A1.5%2C%22companyStage%22%3A%22seed%22%7D) of a Friendly Options results page representing a sample offer you might get from an early stage startup. 

## Locally

Clone this repo, run an in-place webserver and then load it up in your browser.  Here is a sample method:

    # git clone git@github.com:danbirken/friendlyoptions.git
    # cd friendlyoptions
    # python -m SimpleHTTPServer
      Serving HTTP on 0.0.0.0 port 8000 ...
      
Then open http://localhost:8000/ in your browser
