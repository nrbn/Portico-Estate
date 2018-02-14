## Portico Estate API Documentation

- [Search](#search)
- [Resource](#resource)


**Search**
----
  Returns json data for search.

* **URL**

  /bookingfrontend/?

* **Method:**

  `GET`
  
*  **URL Params**

   **Required:**
   
    - `menuaction=bookingfrontend.uisearch.query`
    - `searchterm=[string]`
   

* **Data Params**

    - `filter_search_type=[string]`
    - `filter_part_of_town=[integer]`
    - `filter_top_level=[integer]`
    - `phpgw_return_as=[string]`


* **Success Response:**

  * **Code:** 200 <br />
    **Content:**
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




**Resource**
----
  Returns json data for resource.

* **URL**

  /bookingfrontend/?

* **Method:**

  `GET`
  
*  **URL Params**

   **Required:**
   
    - `menuaction=bookingfrontend.uiresource.index_json`
    
   
* **Data Params**

    - `filter_building_id=[integer]`
    - `phpgw_return_as=[string]`


* **Success Response:**

  * **Code:** 200 <br />
    **Content:**
```
 {
  "total_records": 1,
  "start": 0,
  "sort": null,
  "dir": "asc",
  "results": [
    {
      "id": 37,
      "active": 1,
      "sort": 0,
      "name": "Grus (40 x 80)",
      "type": "Lokale",
      "description": "<ul>\r\n<li>7er-bane<\/li><li>Lys er p\u00e5 mandag-fredag 16.00 - 22.15<\/li><\/ul>",
      "activity_id": 2,
      "organizations_ids": "",
      "json_representation": null,
      "building_id": 27,
      "activity_name": "Idrett",
      "buildings": [
        27
      ],
      "link": "\/PorticoEstate\/bookingfrontend\/?menuaction=bookingfrontend.uiresource.show&amp;id=37&amp;domain=default&amp;bookingfrontendsession=v8rkaqgnopln438m5lm0dvqhj7&amp;click_history=fbb79046d66bd4bd29a9f9d39ae32662",
      "building_street": "Madlasandnes",
      "building_city": "4045",
      "building_district": "Madla",
      "building_name": "Hafrsfjord skole fotballbane (Idrett)",
      "full_name": "Hafrsfjord skole fotballbane (Idrett) \/ Grus (40 x 80)"
    }
  ]
}
```
