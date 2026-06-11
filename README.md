# Cardsort+

Cardsort+ is a **free and open-source** tool for conducting virtual card sorting. It was built as a way to **quickly conduct card sorting online**, without the need to sign up or subscribe to commercial solutions or self-host an open-source project.

It is most effective when used in conjunction with other tools. For example, you could create a form with instructions, a questionnaire and a link to card sorting. You could also ask the participants to copy the results back into the form.

[![Screenshot showing a card sort already started](./images/sort_s.png)](./images/sort.png)

Card Sort Allows to:

- Quickly create a set of cards to sort from a simple comma separated list of items
- Quickly preset some categories (comma-separated list of categories)  
[![Screenshot showing how to set cards and categories](./images/set_cards_cats_s.png)](./images/set_cards_cats.png)
- Choose if cards are randomized or not
- Choose if users can create new cards or new categories
- Create a link to share card testing with others. e.g.: [Link example](https://bmarne.codeberg.page/cardsortplus/card-sort.html#eJw9kcFOwzAMhl8FlesuXHdBUGAHNq1ikxBCHNzgtdaSOHITpgnx7iTOOlXK_9lyftvpb3PbLD-bhxAsNousQoZjIYlkRj5qdgogMKSp8A8b-OZMj-DzVwDBq2BUsfamwxBQSmTBHHsUOWuQ8MrCxrCljC30PQyo5CNYTqEGAq5nC5VFx2ohWTpYPql7ixbVrR0vti0b9kkrWcpUrYCfe7bJJNfrzSeIpcfzMASbm2Z8oSGfKxBLpgDzdB12JRDwIIniHGR9pRPNuTXiUcWxV40xmVK0JldkA34ob7ZJ0yjMLuPWk9Zu84C6fAcBzqAgk6dQCMGMVaVKOckjXP5XZ1Px6tjhkH3qUh1HiKVbl1w4UmnyBt80jQpTmLfaBfLVfxcFTnN6z65e3yepY7xnX3Fodd4PcM3Xorlvlnd__zI6t8U=)
- Share sorting results as a link to show the results in Card Sort or to export results as a JSON (in the clipboard) e.g. [example of link to share a card table](https://bmarne.codeberg.page/cardsortplus/card-sort.html#eJxFUcFuwjAM_RXUXbnsymWCbnAYiGogTdO0gxtMG5HEkZsMoWn_vtgFpkp5z4n9_Oz-VGuEYzX7rBZMxpCz1bSqoW2hw-prWu0QD_qKEDRO6CcQDpOjozOyPM2HCAxdHuR9ydkmLXAZW2S-FL2FA3O6B-jcpMEYS3WJIJSvkPk3GTiQsBgdKrI1lFT1vxkna3o6qbl9bsfbBaLmPUhQQ0jgKEfUURh8Sw5GzkVPSHb2OkCJ0KE6q_urxZoMhayZxEGAIdz819lk32rlMyTp8dJ10ZWmhS5tV84VsLNGCNFw38KKIeJR93MNCr7as73drRFPCp6CYkrZSNLaeoENhE4WtMlDz0S-0G2wmrstBjvJaSDCBZTwEGwUhmD6EXkEOW1AuC66cVm0GvLYFZ1xqIYSJOnWZB9PVpq8wcEOvZIh3qbaRRtG_V1iON-u9-TH8n3m0cZ70WWPTv1-gJf_9VTNHn__AI5qzhg=).
- Have an overview of the results in a basic but efficient enough visual interface showing them  
![Screenshot showing results in a table with a percentage of each answer for each category](./images/results.png)

Cardsort+ is a (friendly) soft fork of [Card Sort](https://github.com/indigane/cardsort). It was created to [implement some missing features](https://github.com/indigane/cardsort/pull/6). The new features are:

- Allows adding local images with a relative or an absolute file path (Card Sort only allows adding online images with an HTTP path, and embedded images with a data path).
- Enables users to edit card content (then, the old content is shown as struck through).
- Enables users to duplicate the cards (then they can sort the cards into several categories).
- Adds an export button to export refined data provided in the analysis tool to a CSV (copied to the clipboard)
- Adds a share button to generate a shareable URL with the current state of the categories’ refinement (copied to the clipboard). Ex.: [Shared Refinement URL](https://bmarne.codeberg.page/cardsortplus/analysis.html#eJxVkDFuwzAMRa9icNYJutUBOnUI2qBL4YGSflwjsmXQcovC0N0jKnDSQoNI8X3yUxsdWPxCT58bvcg6JA3pCBYydIojp1iC53kOoM7QB3oktgEVO7C13KMALXhSbplZuF8X6rLZ6BV8Vq6V6FwMQyF2Sen1DvhaVa3mCWPDk2_OIf5AtPSnn7nZq4KwwkLkVwcHdpd7ghCaI-YZ6r7lqRx19R0d-8ceesvgYqpdH8MkDe4rXqq502pvry1QuNyp9YQ-yqC7b7ub_dOyoTdMPML_w3K-At4Vc9Y=).
- Early alpha stage: displays an interactive dendrogram, that shows automated clustering of the participants card spread (it can be exported as SVG image)  
![Screenshot showing a dendrogram](./images/dendrogram.svg)

## Demo


[Test me](https://bmarne.codeberg.page/cardsortplus/card-sort.html#eJw9kcFOwzAMhl8FlesuXHdBUGAHNq1ikxBCHNzgtdaSOHITpgnx7iTOOlXK_9lyftvpb3PbLD-bhxAsNousQoZjIYlkRj5qdgogMKSp8A8b-OZMj-DzVwDBq2BUsfamwxBQSmTBHHsUOWuQ8MrCxrCljC30PQyo5CNYTqEGAq5nC5VFx2ohWTpYPql7ixbVrR0vti0b9kkrWcpUrYCfe7bJJNfrzSeIpcfzMASbm2Z8oSGfKxBLpgDzdB12JRDwIIniHGR9pRPNuTXiUcWxV40xmVK0JldkA34ob7ZJ0yjMLuPWk9Zu84C6fAcBzqAgk6dQCMGMVaVKOckjXP5XZ1Px6tjhkH3qUh1HiKVbl1w4UmnyBt80jQpTmLfaBfLVfxcFTnN6z65e3yepY7xnX3Fodd4PcM3Xorlvlnd__zI6t8U=), then paste the *Exported Results* to [the analysis tool](https://bmarne.codeberg.page/cardsortplus/analysis.html) (you can paste more than one result, they are added to the analysis). 

## Install

You can "install" Cardsort+ in 3 different ways.

- **Do nothing**. Just use <https://bmarne.codeberg.page/cardsortplus/>. Your browser will download and run Cardsort+ locally, without sending any data to servers. Cardsort+ is gracefully hosted by Codeberg.org 🙏.
- Alternatively, consider **downloading the ZIP** file from this link: <https://codeberg.org/bmarne/cardsortplus/archive/main.zip>. Then you can open the files with your local browser on any machine. `index.html` creates a card sort URL and `analysis.html` analyses the results.
- Alternatively, **host your own instance** of Cardsort+. Simply transfer the contents of the zip file (<https://codeberg.org/bmarne/cardsortplus/archive/main.zip>) to your personal web server.

## How to use Cardsort+?

3 steps for using Cardsort+

1. **Create a test** by using the index page (i.e. <https://bmarne.codeberg.page/cardsortplus/>) by listing cards, categories, and switching options, and validating. Then copy the generated link ([Link example](https://bmarne.codeberg.page/cardsortplus/card-sort.html#eJw9kcFOwzAMhl8FlesuXHdBUGAHNq1ikxBCHNzgtdaSOHITpgnx7iTOOlXK_9lyftvpb3PbLD-bhxAsNousQoZjIYlkRj5qdgogMKSp8A8b-OZMj-DzVwDBq2BUsfamwxBQSmTBHHsUOWuQ8MrCxrCljC30PQyo5CNYTqEGAq5nC5VFx2ohWTpYPql7ixbVrR0vti0b9kkrWcpUrYCfe7bJJNfrzSeIpcfzMASbm2Z8oSGfKxBLpgDzdB12JRDwIIniHGR9pRPNuTXiUcWxV40xmVK0JldkA34ob7ZJ0yjMLuPWk9Zu84C6fAcBzqAgk6dQCMGMVaVKOckjXP5XZ1Px6tjhkH3qUh1HiKVbl1w4UmnyBt80jQpTmLfaBfLVfxcFTnN6z65e3yepY7xnX3Fodd4PcM3Xorlvlnd__zI6t8U=)) and send it to your testers.
2. Use the generated link to **take the test with multiple participants**. At the end of the sort, click on `Share Results` to generate and automatically copy a link ([Example](https://bmarne.codeberg.page/cardsortplus/card-sort.html#eJxFUcFuwjAM_RXUXbnsymWCbnAYiGogTdO0gxtMG5HEkZsMoWn_vtgFpkp5z4n9_Oz-VGuEYzX7rBZMxpCz1bSqoW2hw-prWu0QD_qKEDRO6CcQDpOjozOyPM2HCAxdHuR9ydkmLXAZW2S-FL2FA3O6B-jcpMEYS3WJIJSvkPk3GTiQsBgdKrI1lFT1vxkna3o6qbl9bsfbBaLmPUhQQ0jgKEfUURh8Sw5GzkVPSHb2OkCJ0KE6q_urxZoMhayZxEGAIdz819lk32rlMyTp8dJ10ZWmhS5tV84VsLNGCNFw38KKIeJR93MNCr7as73drRFPCp6CYkrZSNLaeoENhE4WtMlDz0S-0G2wmrstBjvJaSDCBZTwEGwUhmD6EXkEOW1AuC66cVm0GvLYFZ1xqIYSJOnWZB9PVpq8wcEOvZIh3qbaRRtG_V1iON-u9-TH8n3m0cZ70WWPTv1-gJf_9VTNHn__AI5qzhg=)) into your clipboard. This link will take you to a page displaying all the cards that have been arranged. Save this URL. Then, click on `Export Result` to generate and copy a JSON of the sorted results to the clipboard, which you can then save. Results are more usefull if you take the test with multiple testers.
3. **Analyze results**. Go to the analysis page (<https://bmarne.codeberg.page/cardsortplus/analysis.html>) and paste all the JSON you have collected. In the interface, you can merge similar categories. You can then use the table or its CSV export to better understand how testers are sorting the cards.

-----

Analysis tools are in development. If you’re interested, you can take a look at the [current progress](https://indigane.github.io/cardsort/analysis.html) and discuss [in the issues page](https://github.com/indigane/cardsort/issues/2).



## Create your own


<https://bmarne.codeberg.page/cardsortplus/>


## Read about card sorting

<https://en.wikipedia.org/wiki/Card_sorting>


-----

## Advanced use

### Insert images

Images can be added to the cards by typing `image:` and a link to the image.

```
image:https://domain.tld/image.jpg
```

or

```
image:../myfolder/image.jpg
```

Text can also be included before or after an image.

```
image:https://domain.tld/cat.jpg A photo of a cat
```

### Programmatic use

Query parameters can be passed to the card sorting page instead of going through the creation form.

All parameters are optional.

```url
https://bmarne.codeberg.page/cardsortplus/card-sort.html?cards=a,b,c&categories=1,2,3&allowCategoryEditing=0&isRandomized=1
```
