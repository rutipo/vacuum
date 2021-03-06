# Vacuum

[![Build Status][1]][2]

Vacuum is a Ruby wrapper to the [Amazon Product Advertising API][4].

![vacuum][3]

## Usage

```ruby
req = Vacuum.new

req.configure key:    'foo',
              secret: 'secret',
              tag:    'biz-val'

params = { 'Operation'   => 'ItemSearch',
           'SearchIndex' => 'Books',
           'Keywords'    => 'Architecture' }

req.get query: params # XPath is your friend.
```

[1]: https://secure.travis-ci.org/hakanensari/vacuum.png
[2]: http://travis-ci.org/hakanensari/vacuum
[3]: http://f.cl.ly/items/2k2X0e2u0G3k1c260D2u/vacuum.png
[4]: https://affiliate-program.amazon.com/gp/advertising/api/detail/main.html
