---
description: >-
  The objective of this page, is to guide the user to configure the widget for
  accept payments with StablePay.
---

# Payments

1.Choose Payment to generate your Widget.

![](../.gitbook/assets/image.png)

**Note:** Payments are free fee for your client, if they send you DAI. Any other token wil be converted and generate fee.

2.This is the address of your Ethereum wallet to receive Dai.

![](../.gitbook/assets/image%20%2813%29.png)

If you dont have a wallet, you can start with a MetaMask wallet, is easy and fast. To learn more about it:[https://metamask.io/](https://metamask.io/) 

3.If you want that you payments go to **Compound** activate "Supply to Compound".

![](../.gitbook/assets/image%20%2816%29.png)

To learn more about **Compound**, visit their website: [https://compound.finance/](https://compound.finance/).

4.This is optional. Name of the owner of the Ethreum wallet

![](../.gitbook/assets/image%20%289%29.png)

5.This is Optional. After the payment, the widget is going to redirect to your store, put the direction here.

![](../.gitbook/assets/image%20%281%29.png)

6.The code is going to be generated and you ready to paste it on your page!.

```text
<!DOCTYPE html>
<html>
    <head>
        <!-- Add this <script> to the <head> tag -->
        <script src="https://unpkg.com/@stablepay/widget"></script>
    </head>
    <body>
        <!-- Add this anywhere in your site where you would like to render the Widget -->
        <div id="stablepay-widget"></div>

        <!-- Add this <script> at the end of the <body> tag -->
        <script>
            StablePay.renderWidgetButton(
                {
                    type: 'Payment',
                    source: {
                        name: 'John Doe',
                        address: '0x05b54683C2C02aa690DF8b25B18Cd89C37a44f0C'
                    },
                    amount: {
                        total: INSERT_AMOUNT_VARIABLE_HERE
                    },
                    callbackURL: 'https:/mystore.com',
                    postAction: {
                        action: 'compound'
                    },
                    theme: 'standard',
                },
                'stablepay-widget'
            );
        </script>
    </body>
</html>
```

