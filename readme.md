
Welcome to the [Identibyte](https://identibyte.com) blog! Identibyte is an API
for checking if an email address domain is disposable or free.


## Posts

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>

## How Identibyte works

You can get started with a simple `curl` command:

    $ curl -u token: https://identibyte.com/check/user@mvrht.com
    {
      "email": {
        "email": "user@mvrht.com",
        "disposable": true,
        "domain": "mvrht.com",
        "valid": true,
        "free": false
      },
      "domain": {
        "domain": "mvrht.com"
      },
      "createdAt": "2018-10-07T23:16:49.840Z"
    }


You can also integrate Identibyte with Zapier to purge your Mailchimp lists fro
disposable emails.  See our post: **[Remove disposable emails from Mailchimp
with Zapier and
Identibyte](https://identibyte.github.io/examples/zapier/zapier-mailchimp-identibyte.html)**.

Check out our [examples page](https://identibyte.github.io/examples) for more information.

## License

MIT

