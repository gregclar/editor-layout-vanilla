# A static Editor interface built with plain HTML and CSS.

The immediate goal is to recreate the existing Editor GUI layout and components in static files.

This GUI includes the following layout elements:

  - Header, footer, and main results area
  - Navbar with drop down menus
  - Header search form with characteristic multi-target search field and widgets
  - Tabs for the main search results area
  - Record details overlay area, which appears and disappears as required
  - Tabs for the record details overlay area
  - Appropriate scrolling and non-scrolling blocks

The GUI also needs to be responsive - within realistic limits, because we do not expect users to run the Editor on tablets or phones.

The current trial does not include our typeahead dropdowns - I think they will be a separate experiment.


## Broader Goal

In the current Editor the layout was created and runs under Bootstrap 3.

Bootstrap is now at version 5 and appears to have changed greatly since version 3, in part to take advantage of new and improved CSS features.

One option is to upgrade the Editor to Bootstrap 5.  I'm not doing that immediately, partly because there's a learning curve to Bootstrap 5, but also because Bootstrap 5 wraps up many CSS features and locks you into a set of Bootstrap conventions, decisions and commitments which bring their own costs.  That might be necessary, but it's not my first choice.

I'd like to find out how hard it is do what I've previously done with Bootstrap 3 but with plain HTML and CSS.  That's the option I'm exploring here. It is an experiment to see how feasible it now is to do that in 2024.  It is also a chance for me to learn and understand the features of CSS in 2024.

Overall, I'd like to reduce the Editor's reliance on non-essential 3rd Party frameworks and libraries wherever possible - every 3rd party library brings an upgrade burden - sometimes that burden is justified, but for long term maintainability I'd like to minimise that burden.

I am literally following a current thread towards plain HTML and CSS.  For that reason I'm not using TailWind CSS in this experiment.

### Advantages of creating a static design separate from the Rails framework

One thing I've noticed doing this is that having a dedicated and simple-as-possible static site to set up the layout means I can concentrate purely on the HTML and CSS mechanics of the layout.

I don't have to worry about anything in Rails and I have to look at any problems as purely HTML/CSS problems.

This results in clearer lines of responsibility in the code.


### Useful CSS Features So Far

  - grid layout
  - nesting
  - variables (custom properties)
  - :has()

### Libraries or Frameworks used

Currently just:
  - fontawesome 6 free

### JavaScript

At this stage the static layout runs perfectly with JavaScript disabled - and that's a good way to test it.

I may need some JavaScript at some stage - that will be part of the trial.

If and when that happens I'd like to see how far I can go without JQuery.

JQuery was wonderful in its heyday, but again, JavaScript has evolved a lot in the last 10 years, and either plain JavaScript or a lightweight JQuery replacement library might be sufficient.

One of our JavaScript libraries requires a specific version of JavaScript and that's a dependency I'd like to remove.



