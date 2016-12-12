# elastic-create

Element providing a way to create a single elasticsearch document. 

Example:
```html
<elastic-client
    config='{"host": "http://localhost:9200"}'
    client="{{esclient}}"
    cluster-status="{{my-status}}">
</elastic-client>

<elastic-create
    client="[[esclient]]"
    index="mockads"
    elastic-type="ad"
    body='{title: "new title here", "city": "New York City"}'
    results="{{data}}"
    lastError="{{error}}">
</elastic-create>
```

## Dependencies

Element dependencies are managed via [Bower](http://bower.io/). You can
install that via:

    npm install -g bower

Then, go ahead and download the element's dependencies:

    bower install

To run the demo and unit tests, you will need a local elasticsearch instance and the mockads data referenced in the elastic-client-search repo.
