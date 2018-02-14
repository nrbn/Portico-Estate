## Welcome to Portico Estate API Documentation

Portico Estate application is based on phpGroupWare. phpGroupWare (formerly known as webdistro) is a multi-user groupware suite written in PHP. Its provides a Web-based calendar, todo-list, addressbook, email, news headlines, and a file manager. The calendar supports repeating events.

- [Bookingfrontend](#bookingfrontend)
- [Search](#search)


# Bookingfrontend

All front-end content are under the bookingfrontend path and the parameter menuaction will call method for the page user visits.

### Search

Main required paramaters for search is menuaction, and searchterm. Searchterm is the value of search data. So the url will look like this `(searchterm=åmøy%20idrettspark)`:

```

http://.../PorticoEstate/bookingfrontend/?searchterm=åmøy%20idrettspark&menuaction=bookingfrontend.uisearch.query&phpgw_return_as=json

```
And the respons will be:

```
{
  "results": {
    "total_records": [
      1,
      0
    ],
    "results": [
      {
        "id": 18,
        "name": "Austre \u00c5m\u00f8y idrettspark",
        "homepage": "",
        "calendar_text": "",
        "description": "Austre \u00c5m\u00f8y idrettspark best\u00e5r av en fotballbane. Det finnes 2 gardeober i skolen.",
        "phone": "",
        "email": "",
        "tilsyn_name": "",
        "tilsyn_phone": "",
        "tilsyn_email": "",
        "tilsyn_name2": "",
        "tilsyn_phone2": "",
        "tilsyn_email2": "",
        "deactivate_calendar": 0,
        "deactivate_application": 0,
        "deactivate_sendmessage": 1,
        "extra_kalendar": 0,
        "location_code": "5070",
        "activity_id": 2,
        "part_of_town_id": "7",
        "street": "V\u00e5gholmveien",
        "zip_code": "4154",
        "district": "Tasta",
        "city": "Austre \u00c5m\u00f8y",
        "active": 1,
        "activity_name": "Idrett",
        "type": "building",
        "link": "\/PorticoEstate\/bookingfrontend\/?menuaction=bookingfrontend.uibuilding.show&amp;id=18&amp;domain=default&amp;bookingfrontendsession=naoei7vir38k4g39rtsb662q81&amp;click_history=f93f70f6b76473b22343453d2f911119",
        "img_container": "building-18",
        "img_url": "\/PorticoEstate\/bookingfrontend\/?menuaction=bookingfrontend.uidocument_building.index_images&amp;filter_owner_id=18&amp;phpgw_return_as=json&amp;results=1&amp;domain=default&amp;bookingfrontendsession=naoei7vir38k4g39rtsb662q81&amp;click_history=f93f70f6b76473b22343453d2f911119"
      }
    ],
    "start": [
      0,
      0
    ],
    "sort": [
      "name",
      "name"
    ],
    "dir": [
      "asc",
      "asc"
    ],
    "total_records_sum": 1
  }
}
```




**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```


[a relative link](home.md)


Search Request

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/nrbn/Portico-Estate/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
