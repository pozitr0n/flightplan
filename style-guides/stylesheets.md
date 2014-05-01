#### General

* Put spaces after `:` in property declarations.
* Put spaces before `{` in rule declarations.
* Write multilines with tabulation.

#### Anatomy of rulesets

```css
selector {
  property: value;
  }
```

Properties of children:

```css
selector {
  property: value;
  }
  children {
    property: value;
    }
```

#### Naming conventions

* `a_b` - the separator between the selector and the modifier
* `a-b` - the separator between two selectors

#### File structure

We use __SCSS__ and include all our styles with `@import` in _application.css_. For all modules (html blocks) create new file.

```
stylesheets/
  modules/
    [modulname].scss
  additional.scss - additional properties (clearfix, mixins)
  application.scss - including all styles with @import
  common.scss - common styles (properties of tags by default, headers...)
  layout.scss - base elements of markup
  params.scss - definitions
  reset.scss - reset css (Eric Meyer)
```
