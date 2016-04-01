![swish](https://cloud.githubusercontent.com/assets/3159565/14215385/deb7a68c-f842-11e5-9c9a-1f7102eb4d25.png)
# Swish Python Client Library [![Build Status](https://travis-ci.org/playing-se/swish-python.svg?branch=master)](https://travis-ci.org/playing-se/swish-python)
This client library is designed to support the [Swish API](https://www.getswish.se/content/uploads/2015/06/Guide-Swish-API_160118.pdf). It was originally developed at [Playing](https://playing.se/).

## Installation
Not available yet.

## Quick Start Example

    import swish

    swish_client = swish.SwishClient(
        swish.Environment.Production,
        'YOUR_PAYEE_ALIAS',
        '/path/to/cert.crt'
    )

    swish_client.payment_request(
        amount=123,
        currency='SEK',
        callback_url='https://your-callback.url/here/',
        payment_reference='Optional custom reference',
        message='Quick Start Example'
    )
