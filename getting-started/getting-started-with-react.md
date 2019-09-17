---
description: >-
  This page describes how you can install and use the Stable Pay widget on your
  code from a React project.
---

# Using with React

## Usage

Enable cryptocurrency payments and donations in your site by either:

* Using the Widget Component Library by installing our NPM Package in your **React App**. \(Read how to install [Here](https://www.github.com/)\) -- OR --
* Using our Embeddable Widget in your site using **HTML/JavaScript**. \(Read our [Docs](https://github.com/dtutila/stablepay_widget/blob/master) for more information\)

## Installing

Using npm:

```text
  npm install stablepay-widget
```

Using yarn:

```text
   yarn add stablepay-widget
```

## Example

Predefined Widget Button:

```text
import React from 'react';
import { WidgetButton } from 'stablepay-widget';

const Checkout = () => {
    const payload = {
        type: 'Payment',
        source: {
            name: 'Your Store',
            address: '0x0...'
        },
        amount: {
            total: '9.99'
        },
        callbackURL: 'https://yourstore.com/checkout',
        theme: 'standard'
    };

    return <WidgetButton {...payload} />;
};

export default Checkout;
```

Custom Widget Button:

```text
import React from 'react';
import { Widget } from 'stablepay-widget';

const Checkout = () => {
    const payload = {
        type: 'Payment',
        source: {
            name: 'Your Store',
            address: '0x0...'
        },
        amount: {
            total: '9.99'
        },
        callbackURL: 'https://yourstore.com/checkout',
        theme: 'custom'
    };

    return (
        <button onClick={() => Widget.open(payload)}>Pay With StablePay</button>
    );
};

export default Checkout;
```

For more information, you can visit our page:[https://stablepay.io/](https://stablepay.io/)

