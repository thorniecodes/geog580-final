# GEOG 580 - Remote Sensing Principles & Applications - Final Project
This repository represents my final project for GEOG 580 - Remote Sensing Principles and Applications I. The assignment required students to select a project topic related to the use of remote sensing techniques to solve problems in their field of study. The two final outputs for this assignment include an oral presentation and a final report.

## Analyzing Land Cover Change and Thermal Impacts of Data Center Development Using Landsat 8 Imagery in Northern Virginia Comparing Changes Between August 2014 & August 2024.

### The Research Explained for a Geographic Information Scientist Community
*Introduction & Objective*

Remote sensing has become an essential tool for monitoring urban expansion and its thermal impact on local environments. Landsat 8 Operational Land Imager (OLI) and Thermal Infrared Sensor (TIRS) provide multispectral and thermal data that enable the analysis of land cover changes and land surface temperature (LST) variations over time. The Normalized Difference Built-up Index (NDBI) derived from Landsat 8's near infrared (Band 5: 0.85-0.88 μm) bands and shortwave infrared (Band 6: 1.57-1.65 μm) has proven effective in identifying urban development patterns and correlates strongly with land surface temperature increases (Guha et al., 2018). Thermal Band 10 (10.60-11.19 μm) allows for precise LST calculations using established retrieval algorithms such as the mono-window method and radiative transfer equation-based approaches (Wang et al., 2015; Yu et al., 2014). Multi-year analyses using these indices have successfully documented the relationship between built-up expansion and temperature changes across various urbanized regions, with studies showing temperature differences of 3-4°C between developed and undeveloped areas (Bayraktar & Turalioglu, 2024; Guha et al., 2018).

This study analyzes the transformation of LST across all of Loudoun County and then the location of a Yondr Group's data center that became operational in 2024. By comparing county-wide urban development before (August 2014) and after construction (August 2024). NDBI will be employed to identify and delineate areas that transitioned from undeveloped or agricultural land to data center facilities, then quantify the change in LST. This direct comparison will isolate the thermal impact of data center development by measuring temperature changes at the same geographic coordinates before and after facility construction. After gathering these results, LST compared 2014 and 2024 changes at the Yondr Group's data center location to show a basic proof of concept that major emissions are projected from data centers.


### The Research Explained for a Publicly Engaged Community Outside of Academia

#About the Research
Outside of Washington D.C. and over the past 5-10 years, Northern Virginia has become the epicenter of America's data center boom. Technology companies like Google are building massive warehouse-like buildings, sometimes called "server farms," to house thousands of computers that power the internet, from social media to cloud storage. But more specifically, to power the computing needs required by artificial intelligence technology advances such as Gemini, ChatGPT, Claude, and CoPilot.

I'm investigating how this explosion of data centers is physically changing the region's land and temperature.

*Here's why this matters:*

The Heat Problem: Data centers generate enormous amounts of heat from all those computers running 24/7. To keep the equipment from overheating, these facilities require intensive cooling systems that draw massive quantities of water from local sources like rivers and aquifers. All this activity—both the heat from the buildings themselves and the energy used for cooling—can raise temperatures in surrounding areas.

The Space Problem: Each data center campus can sprawl across dozens or even hundreds of acres. What was once farmland or forest is now covered with concrete and buildings. This dramatic change in land cover affects everything from local weather patterns to wildlife habitats. [To put the scale in perspective: Google is expanding its data center footprint this year with a new facility close to Richmond, VA.)1,200 acres in total or 909 football fields, is the expected expansion size.](https://www.datacenterdynamics.com/en/news/google-to-invest-9bn-in-virginia-data-centers-plans-new-campus-in-chesterfield-county/)

*Why Northern Virginia? I chose this region for three key reasons:*

- It's ground zero for data center growth: This area has seen explosive construction of data centers in recent years, often built in previously rural communities that are now grappling with this industrial transformation.
- It's the birthplace of the modern internet: Northern Virginia is home to the internet's original infrastructure and remains its most critical hub today.
- Northern Virigina makes up 25% of World’s computer processing power: Although Northern Virigina is small in comparison to how many data centers exist in one geographic location. It makes up a huge chunk of the entire world’s combined computer processing energy needs.

*2 Ways to Visually Represent Change Caused by Data Center Development*
I use pictures of the Earth taken by satellites put up in the sky by NASA  to understand what had changed about the land and temperature changes in Loudon County and Prince William County, VA using images from August 2019 and August 2024 to compare. I am expecting there to less green spaces and a raise in local temperatures. Additionally, I'll show urban development within Loudoun County to highlight the massive growth within this time period.

Visit [https://thorniecodes.github.io/geog580-finalproject/](https://thorniecodes.github.io/geog580-finalproject/) to read my work.

---------

------
# The Minimal theme

[![.github/workflows/ci.yaml](https://github.com/pages-themes/minimal/actions/workflows/ci.yaml/badge.svg)](https://github.com/pages-themes/minimal/actions/workflows/ci.yaml) [![Gem Version](https://badge.fury.io/rb/jekyll-theme-minimal.svg)](https://badge.fury.io/rb/jekyll-theme-minimal)

*Minimal is a Jekyll theme for GitHub Pages. You can [preview the theme to see what it looks like](http://pages-themes.github.io/minimal), or even [use it today](#usage).*

![Thumbnail of Minimal](thumbnail.png)

## Usage

To use the Minimal theme:

1. Add the following to your site's `_config.yml`:

    ```yml
    remote_theme: pages-themes/minimal@v0.2.0
    plugins:
    - jekyll-remote-theme # add this line to the plugins list if you already have one
    ```

2. Optionally, if you'd like to preview your site on your computer, add the following to your site's `Gemfile`:

    ```ruby
    gem "github-pages", group: :jekyll_plugins
    ```

## Customizing

### Configuration variables

Minimal will respect the following variables, if set in your site's `_config.yml`:

```yml
title: [The title of your site]
description: [A short description of your site's purpose]
```

Additionally, you may choose to set the following optional variables:

```yml
show_downloads: ["true" or "false" (unquoted) to indicate whether to provide a download URL]
google_analytics: [Your Google Analytics tracking ID]
```

### Stylesheet

If you'd like to add your own custom styles:

1. Create a file called `/assets/css/style.scss` in your site
2. Add the following content to the top of the file, exactly as shown:
    ```scss
    ---
    ---

    @import "{{ site.theme }}";
    ```
3. Add any custom CSS (or Sass, including imports) you'd like immediately after the `@import` line

*Note: If you'd like to change the theme's Sass variables, you must set new values before the `@import` line in your stylesheet.*

### Layouts

If you'd like to change the theme's HTML layout:

1. For some changes such as a custom `favicon`, you can add custom files in your local `_includes` folder. The files [provided with the theme](https://github.com/pages-themes/minimal/tree/master/_includes) provide a starting point and are included by the [original layout template](https://github.com/pages-themes/minimal/blob/master/_layouts/default.html).
2. For more extensive changes, [copy the original template](https://github.com/pages-themes/minimal/blob/master/_layouts/default.html) from the theme's repository<br />(*Pro-tip: click "raw" to make copying easier*)
3. Create a file called `/_layouts/default.html` in your site
4. Paste the default layout content copied in the first step
5. Customize the layout as you'd like

### Customizing Google Analytics code

Google has released several iterations to their Google Analytics code over the years since this theme was first created. If you would like to take advantage of the latest code, paste it into `_includes/head-custom-google-analytics.html` in your Jekyll site.

### Overriding GitHub-generated URLs

Templates often rely on URLs supplied by GitHub such as links to your repository or links to download your project. If you'd like to override one or more default URLs:

1. Look at [the template source](https://github.com/pages-themes/minimal/blob/master/_layouts/default.html) to determine the name of the variable. It will be in the form of `{{ site.github.zip_url }}`.
2. Specify the URL that you'd like the template to use in your site's `_config.yml`. For example, if the variable was `site.github.url`, you'd add the following:
    ```yml
    github:
      zip_url: http://example.com/download.zip
      another_url: another value
    ```
3. When your site is built, Jekyll will use the URL you specified, rather than the default one provided by GitHub.

*Note: You must remove the `site.` prefix, and each variable name (after the `github.`) should be indent with two space below `github:`.*

For more information, see [the Jekyll variables documentation](https://jekyllrb.com/docs/variables/).

## Roadmap

See the [open issues](https://github.com/pages-themes/minimal/issues) for a list of proposed features (and known issues).

## Project philosophy

The Minimal theme is intended to make it quick and easy for GitHub Pages users to create their first (or 100th) website. The theme should meet the vast majority of users' needs out of the box, erring on the side of simplicity rather than flexibility, and provide users the opportunity to opt-in to additional complexity if they have specific needs or wish to further customize their experience (such as adding custom CSS or modifying the default layout). It should also look great, but that goes without saying.

## Contributing

Interested in contributing to Minimal? We'd love your help. Minimal is an open source project, built one contribution at a time by users like you. See [the CONTRIBUTING file](docs/CONTRIBUTING.md) for instructions on how to contribute.

### Previewing the theme locally

If you'd like to preview the theme locally (for example, in the process of proposing a change):

1. Clone down the theme's repository (`git clone https://github.com/pages-themes/minimal`)
2. `cd` into the theme's directory
3. Run `script/bootstrap` to install the necessary dependencies
4. Run `bundle exec jekyll serve` to start the preview server
5. Visit [`localhost:4000`](http://localhost:4000) in your browser to preview the theme

### Running tests

The theme contains a minimal test suite, to ensure a site with the theme would build successfully. To run the tests, simply run `script/cibuild`. You'll need to run `script/bootstrap` once before the test script will work.
