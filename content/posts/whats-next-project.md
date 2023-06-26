---
title: "Whats the Next Project"
date: 2023-06-26T21:53:38+09:00
draft: false
---


Since I stopped working on MEV recently, I was thinking about what I should do next. 
Honestly, I have no idea LOL. I'm browsing the internet and trying out some new things, but nothing interests me so far.
Something special about MEV is that you have no customers and don't need any permission.
Sounds a little bit like a scam, but it is what it is. 
Now, I'm looking for something other than MEV. I need a customer and good product.

<!--more-->

## Is it too much hype for GPT?
It's wild to see so many GPT related repos on GitHub get so many stars way faster than legendary opensource projects.

One ML developer I know on the internet told me this:
> GPT is cool, but there isn't much opportunity for individual and small startups. They all will be bottlenecked by the same set of AI models.
If they want to train models, it becomes a capital intensive game. But if they don't train, basically it is too easy to be replaced.

This is shocking to me because I thought GPT would be a great opportunity for everyone.
He also said that only a few startups will survive in the end. What do you guys think?
I have no idea. I'm a ML noob.


## ID Controversy in Japan
Asides from GPT, I was thinking about the controversial ID system in Japan.

### Some background
Japan has a unique ID system called "My Number", or "マイナンバー" in Japanese.
It is a 12-digit number assigned to each resident of Japan, including foreign residents.
It was introduced in 2016 and since then, the government has been pushing the use of My Number in various ways.
Why did the government introduce this system? Well because we have so many issues on the transition to a digital society.
We still rely on paper documents for many things. Inkan(印鑑), a personal seal, is still used for many contracts.
I cannot believe FAX is the de facto standard for sending documents among doctors.
The legacy systems still survive in this country.

### My Number problems
To solve these issues, the government introduced My Number. 
It is optional to create a My Number card, but most people have one already because there was a campaign of getting $200 by creating one.

However, there are many troubles with My Number. You can see many news articles about My Number problems.
e.g. [data leak](https://www.theregister.com/2023/06/22/japan_my_number_security_review/)


### What's in My Number?
I was playing around with my own My Number card.

Here is the repo:

repo: https://github.com/yuichiroaoki/myna/tree/main


It can be used in contract and contractless interfaces. You can use a normal card reader for contract interfaces. 
For contractless interfaces, you can use a NFC reader. Modern Android phones have NFC readers, so you can use your phone as a card reader as well.

#### Getting attributes
This is how it works:

1. Insert a My Number card into a card reader
2. Send a command to the card reader
3. Enter 4-digit PIN
4. Get the following attributes
- name
- address
- date of birth
- sex

You get the attributes printed on the card. I haven't tried but you can get the photo data as well. 
After you enter the wrong PIN 3 times, the card is locked and you have to go to the city office to unlock it.
These data are not important, but given that you can login to the government system with this card and PIN and see the more private data like income, tax, etc, people don't want to carry it around.

Anyway, it seems easy to do anything with My Number, but in order to develop some system using My Number, you have to go through a long process of getting approval from the government.
I don't like to get into this kind of trouble, but once you get approval, you might get $14,000 per contract with a local government.

Original (Japanese)
>また、自治体や事業者にとって、マイナンバーカードの活用を始める際の注意点やデメリットとしては、導入・運用にかかるコストの問題が挙げられます。マイナンバーカードの活用には、4桁の暗証番号（PIN）とICチップを読み込むためのカードリーダーの端末が必要となるため、初期費用や運用コストがかかってしまいます。一般的に、小さなプランでも初期費用が200万円程度、運用コストが毎年100万円程度はかかる見通しです。

English (Google Translate)
>In addition, for local governments and business operators, one of the points to note and disadvantages when starting to use the My Number Card is the cost of introduction and operation. The use of My Number cards requires a card reader terminal to read a 4-digit personal identification number (PIN) and an IC chip, which incurs initial costs and operating costs. In general, even for a small plan, the initial cost is expected to be about 2 million yen, and the annual operating cost is expected to be about 1 million yen.

https://www.tis.amano.co.jp/gyomu_kaizen/3371/
