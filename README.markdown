Gumroad
======

Gumroad is a Ruby wrapper for the Gumroad API.

**This gem is a work in progress. Contributions are welcome.**

Authentication
--------
``` ruby
client = Gumroad.new(username, password)
```

Links
--------
``` ruby
links = client.links.all
```

``` ruby
link = client.links.find(id)
```

You now have a Gumroad::Link object. You can call methods such as `link.name` and `link.url`.

It's pretty easy to create a link.

``` ruby
client.links.create(name: 'Github', url: 'http://github.com')
```

Thanks
--------
* GroupMe's [quimby](https://github.com/groupme/quimby) gem. I took their object approach when writing this gem.