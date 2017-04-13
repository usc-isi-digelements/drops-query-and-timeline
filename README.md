# drops-query-and-timeline

A Polymer Element that does an elasticsearch query and uses the results to create a timeline display.

Example:
```html
  <drops-query-and-timeline
    client="[[esclient]]"
    index="mockads"
    date-hist-name="dates"
    date-hist-field="date"
    location-agg-name="locations"
    location-agg-field="city"
    index-types='["ad"]'
    filter-list='[]'
    query="[[query]]"
    transform="[[eventDropsTimeline]]">
  </drops-query-and-timeline>
```

### Styling
`<drops-query-and-timeline>` includes the `<drops-timeline>` component, which has support for the following custom properties and mixins for styling:

Custom property        | Description                                                                                          | Default
-----------------------|------------------------------------------------------------------------------------------------------|--------------------------
`--timeline-color-1`   | Color for first row of drops in timeline (there can be up to 16 colors total, depending on the data) | --paper-blue-500
`--timeline-color-2`   | Second color for drops in timeline                                                                   | --paper-orange-500
`--timeline-color-3`   | Third color for drops in timeline                                                                    | --paper-green-500
`--timeline-color-4`   | Fourth color for drops in timeline                                                                   | --paper-red-500
`--timeline-color-5`   | Fifth color for drops in timeline                                                                    | --paper-purple-500
`--timeline-color-6`   | Sixth drop timeline color                                                                            | --paper-yellow-500
`--timeline-color-7`   | Seventh drop timeline color                                                                          | --paper-indigo-500
`--timeline-color-8`   | Eighth drop timeline color                                                                           | --paper-cyan-500
`--timeline-color-9`   | Ninth drop timeline color                                                                            | --paper-deep-orange-500
`--timeline-color-10`  | Tenth drop timeline color                                                                            | --paper-lime-500
`--timeline-color-11`  | Eleventh drop timeline color                                                                         | --paper-pink-500
`--timeline-color-12`  | Twelfth drop timeline color                                                                          | --paper-deep-purple-500
`--timeline-color-13`  | Thirteenth drop timeline color                                                                       | --paper-amber-500
`--timeline-color-14`  | Fourteenth drop timeline color                                                                       | --paper-teal-500
`--timeline-color-15`  | Fifteenth drop timeline color                                                                        | --paper-light-green-500
`--timeline-color-16`  | Sixteenth drop timeline color                                                                        | --paper-light-blue-500

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
