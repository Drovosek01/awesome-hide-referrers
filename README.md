# List of services for hiding referrers

Language: [Русский](README_RU.md) | English

## Content

- [List of services for hiding referrers](#list-of-services-for-hiding-referrers)
  - [Content](#content)
  - [What is this repository](#what-is-this-repository)
  - [What is HTTP Referer](#what-is-http-referer)
  - [FAQ](#faq)
  - [Hiding Referrers vs Shortening Links](#hiding-referrers-vs-shortening-links)
  - [Lists of services and comparison tables](#lists-of-services-and-comparison-tables)
    - [Alternative services](#alternative-services)
  - [Explanation of table headers](#explanation-of-table-headers)
  - [Dead services](#dead-services)

## What is this repository

This repository is a list of services for hiding referrers when switching from one site to another. The services are presented in a comparative table.

You can read more about the concept of "Awesome" lists [here](https://github.com/sindresorhus/awesome/blob/master/awesome.md).

> Unfortunately, I can't always find the time to fill out a comparison table. If you have an opportunity to improve the repository (correct errors in the text or fill in items in the comparison table or something else) - do it and create a Pull Request


## What is HTTP Referer

In short, this is the address of the site from which the transition to the current site was made.

You can read more about HTTP Referer at [MDN](https://developer.mozilla.org/docs/Web/HTTP/Headers/Referer) and [Wikipedia](https://en.wikipedia.org/wiki/HTTP_referer).

## FAQ

Answers to predictable questions.

- Why is the information in the repository only in 2 languages? (English will be later)
  - Because my native language is Russian and it is more convenient for me to formulate thoughts in my native language. After that, I use online translators to translate from Russian to English. If you have the desire and the opportunity - make a full translation into another language and create a Pull Request

- Will there be a translation into other languages?
  - I do not plan to translate into other languages. If someone makes a complete translation of files into another language and creates a Pull-Request, I will add this translation, but I will not be able to support it (add new information if it is not just a jackdaw in the table)

- By what principle do services get into this list/table?
  - It's simple. If the service is designed to store images or you can upload images that are stored for a long time and you can get a direct link to them - we add it to the table with the appropriate category and try to find out about the properties of the service by filling in the items in the comparison table.

## Hiding Referrers vs Shortening Links

Link shortening services also hide the referrer, but still, link shortening services have a different purpose, although they can also be used to hide the referer.

I will try to find time and create a repository with services to shorten links, but in this repository there will only be services that hide the referer and when using such a service, you can see a link to the site to which the transition will be made.

## Lists of services and comparison tables

Below are all the services I know that allow me to generate a link to hide the referrer.

I have tried to reduce the column headers to a minimum so that they do not lose their meaning. For more information about the meaning of the header, about what information is in each column, see the section "Explanation of the headers in the table" below.

Links | Example | No delay | There is SSL
--- | --- | --- | ---
http://hidereferrer.net/ | http://hidereferrer.net/?https://github.com/ | + | -
https://href.li/ | https://href.li/?https://github.com/ | + | +
https://url.rw/ | https://url.rw/?https://github.com/ | + | +
https://noref.io/ | https://noref.io/#https://github.com/ | + | +
https://redirect.me/ | https://redirect.me/?https://github.com/ | + | +
https://privatelink.de/ | https://privatelink.de/?https://github.com/ | 0.2s | +
https://anonymz.com/ | https://www.anonymz.com/?https://github.com/ | 0.5s | +
https://anonym.to/ | https://anonym.to/?https://github.com/ | 1s | +
https://dereferer.link/ | https://dereferer.link/?https://github.com/ | 3s | +
https://anonymiz.com/ | https://anonymiz.com/?https://github.com/ | 6s | +
https://www.lolinez.com/ | https://www.lolinez.com/?https://github.com/ | 20s | +
https://noref.one/ | https://noref.one/?https://github.com/ | 20s | +
https://dereferer.me/ | https://dereferer.me/?https%3A//github.com/ | 5s | +
https://xww.ro/ | https://xww.ro/?https://github.com/ | 2s | +
https://anoni.men/ | https://anoni.men/go/https://github.com/ | 6s | +
https://anonim.xyz/ | https://anonim.xyz/go/https://github.com/ | 6s | +
https://norefs.com/ | https://norefs.com/https://github.com/ |2s | +

### Alternative services

Below is a list of services that do not position themselves as services for hiding referrers, but they can still be used for this. These services do not have a familiar interface in order to insert a link to the source site, click on the button and get the generated link - you will need to manually generate the final link.

Also, these services have several disadvantages - not all of them automatically redirect to the site where you need to hide the referrer, also some of them filter and may not redirect you to sites that they consider malicious, and some of these services are blocked in some countries (for example, VK is blocked in Ukraine).

Links | Example | No confirmation needed | No site filter
--- | --- | --- | ---
https://vk.com/away.php?to= | https://vk.com/away.php?to=https://github.com/ | + | -
https://adguardteam.github.io/AnonymousRedirect/redirect.html?url= | https://adguardteam.github.io/AnonymousRedirect/redirect.html?url=https://github.com/ | - | ?
https://www.youtube.com/redirect?q= | https://www.youtube.com/redirect?q=https://github.com | - | ?
https://steamcommunity.com/linkfilter/?url= | https://steamcommunity.com/linkfilter/?url=https://github.com | - | ?
http://forum.oszone.net/go.php?url= | http://forum.oszone.net/go.php?url=https://github.com/ | + | -
[https://brnm.ru/go?](https://brnm.ru/go?) | https://brnm.ru/go?https://github.com/ | + | ?
https://2baksa.ws/go/go.php?url= | https://2baksa.ws/go/go.php?url=https://github.com/ | +- | ?
https://philka.ru/forum/go/? | https://philka.ru/forum/go/?https://github.com/ | +- | ?

## Explanation of table headers

It is difficult to fit detailed information about what information is displayed in the column into the headers, so detailed information about each header from the comparison table will be in this section.

I tried to formulate the headings so that the answer "yes" in the column meant something positive about the service. Instead of a simple answer `Yes` or `No`, of course it is more convenient and expedient to put `+` or `-`.

1. Links - links to the service. If the resource has several mirror domains, then you need to specify them separated by commas `,`. Links to link shortening services that lead to viewing the image do not need to be specified in this column.
2. Example - an example of a link that is generated by the service. The example may differ from what you get when using the service, for example, some services generate a link from http and when you click on the generated link, you get to a page with https.
3. No delay - there is no delay when clicking on the generated link. Some services are trying to earn money and show ads when clicking on the generated link. Usually there is a timer on the advertising page, after which an automatic transition to the final link will occur. Also, some of these services have only a button on the advertising page for manually switching to the end link, and some have a clickable end link.
4. There is SSL - is it possible to get to the service page via HTTPS.

## Dead services

These are services that have stopped working. Just leave them here for the story.

> The sites of some of these services are still working, but when clicking on the generated links, redirection is not carried out.

- https://hidemyref.org/
- https://nullrefer.com/
- http://refhide.com/
- http://hide-referrer.com/
- http://www.fakeref.com/
- http://clickbakers.com/
- https://linkonym.appspot.com/
- http://safereferer.com/
- https://blankrefer.com/
- https://hidereferrer.com/
- https://nonameno.com/proxy2/
- https://www.web-api.eu/hidereferer
- https://www.anolink.pro/
- https://skiprefer.com/
