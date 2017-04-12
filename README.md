# drops-query-and-timeline

A Polymer Element that does an elasticsearch query and uses the results to create a timeline display.

Example:
```html
  <drops-query-and-timeline
    data="[[data]]"
    timestamps="[[dates]]"
    info="{{_info}}">
  </drops-query-and-timeline>
```

### Dependencies

Dependencies are installed using [Bower](http://bower.io/):

    npm install -g bower
    bower install

### Testing

Tests are run using [web-component-tester](https://github.com/Polymer/web-component-tester):

    npm install -g web-component-tester
    wct

### Demonstration & Documentation

Demonstration and documentation are viewed using [polyserve](https://github.com/PolymerLabs/polyserve):

    npm install -g polyserve
    polyserve

The demo will require a local instance of elasticsearch with the `mockads` index created by running `data/import_test_data.sh`.