# Greed

A [customizable](/config/template_config.toml), [multilanguage](/strings) Telegram shop bot with [Telegram Payments support](https://core.telegram.org/bots/payments)!  

\[ [**Documentation**](https://github.com/Steffo99/greed/wiki) | [Support](https://github.com/Steffo99/greed/issues/new/choose) \]

![](https://i.imgur.com/FdT2tRV.png)

![](https://i.imgur.com/rDYWdUB.png)

![](https://i.imgur.com/9plMzO6.png)



# Installation

before start make sure you installed git, python3 and python3-pip packages

1- clone the repository:
```bash
git clone https://github.com/firildax/BTCPay_Greed
```

2- go to BTCPay_Greed folder and install python required packages from 'requirements.txt':
```bash
cd BTCPay_Greed
python3 -m pip install -r requirements.txt
```
3- create copy from template_config.toml and name it config.toml and configure it:
```bash
cd config
cp template_config.toml config.toml
```
4- open 'config.toml' with your favorite editor and fill these rows depend on your btcpayserver's data and telegram bot token:

    * line 17 : choose your lang (default_language = "en")
    * line 34 : put your bot_token (token = "3345476541:Xcsd3dfgajdluduuuudifdmsYkdnsydfs+dfg")
    * line 74 : to disabling credit cart payment put "" (credit_card_token = "")
    * line 108 : btcpaysever url (url = 'btcpayserver.example.com')
    * line 110 : btcpayserver user token (token = "55323428082308423hhd08s0d8s8s0d8gs0d8gs08df0s8d0sd0602")
        ## needs these two permission on btcpayserver:
            * btcpay.store.canviewinvoices
            * btcpay.store.cancreateinvoice
    * line 112 : btcpayserver storeId (storeId = 'FMXa7ateurSASFAFaoasad90sdgoaugsoagubo1832830808380235')

    and save it.

5- go back to repo's main directory and run 'core.py':
```bash
cd ..
python3 core.py
```

