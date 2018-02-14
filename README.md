## Portico Estate API Documentation

- [Search](#search)
- [Resource](#resource)
- [Document](#document)
- [Document download](#document-download)
- [Images](#images)


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
        "link": "\/PorticoEstate\/bookingfrontend\/?menuaction=bookingfrontend.uibuilding.show&amp;id=18&amp;domain=default&amp;bookingfrontendsession=&amp;click_history=",
        "img_container": "building-18",
        "img_url": "\/PorticoEstate\/bookingfrontend\/?menuaction=bookingfrontend.uidocument_building.index_images&amp;filter_owner_id=18&amp;phpgw_return_as=json&amp;results=1&amp;domain=default&amp;bookingfrontendsession=&amp;click_history="
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
      "link": "\/PorticoEstate\/bookingfrontend\/?menuaction=bookingfrontend.uiresource.show&amp;id=37&amp;domain=default&amp;bookingfrontendsession=&amp;click_history=",
      "building_street": "Madlasandnes",
      "building_city": "4045",
      "building_district": "Madla",
      "building_name": "Hafrsfjord skole fotballbane (Idrett)",
      "full_name": "Hafrsfjord skole fotballbane (Idrett) \/ Grus (40 x 80)"
    }
  ]
}
```



**Document**
----
  Returns json data for documents.

* **URL**

  /bookingfrontend/?

* **Method:**

  `GET`
  
*  **URL Params**

   **Required:**
   
    - `menuaction=bookingfrontend.uidocument_building.index`
    
   
* **Data Params**

    - `sort=[string]`
    - `no_images[integer]`
    - `filter_owner_id[integer]`
    - `phpgw_return_as=[string]`


* **Success Response:**

  * **Code:** 200 <br />
    **Content:**
```
 {
  "start": 0,
  "sort": "name",
  "dir": "asc",
  "recordsTotal": 2,
  "recordsFiltered": 2,
  "data": [
    {
      "id": 361,
      "name": "Prisliste for kommunale idrettsanlegg.pdf",
      "owner_id": 27,
      "category": "Prisliste",
      "description": "Prisliste for kommunale idrettsanlegg",
      "owner_name": "Hafrsfjord skole fotballbane",
      "is_image": false,
      "link": "\/PorticoEstate\/bookingfrontend\/?menuaction=bookingfrontend.uidocument_building.download&amp;id=361&amp;filter_owner_id=27&amp;domain=default&amp;bookingfrontendsession=&amp;click_history="
    },
    {
      "id": 360,
      "name": "Reglement for bruk av kommunale idrettsanlegg.pdf",
      "owner_id": 27,
      "category": "Reglement",
      "description": "Reglement for bruk av kommunale idrettsanlegg",
      "owner_name": "Hafrsfjord skole fotballbane",
      "is_image": false,
      "link": "\/PorticoEstate\/bookingfrontend\/?menuaction=bookingfrontend.uidocument_building.download&amp;id=360&amp;filter_owner_id=27&amp;domain=default&amp;bookingfrontendsession=&amp;click_history="
    }
  ]
}
```


**Document download** ERROR
----
  Returns json data for documents download.

* **URL**

  /bookingfrontend/?

* **Method:**

  `GET`
  
*  **URL Params**

   **Required:**
   
    - `menuaction=bookingfrontend.uidocument_building.download`
    - `id=[integer]`
    
   
* **Data Params**

    - `filter_owner_id[integer]`
    - `phpgw_return_as=[string]`


* **Success Response:**

  * **Code:** 200 <br />
    **Content:**
```
{
 
}
```




**Images**
----
  Returns json data for building images.

* **URL**

  /bookingfrontend/?

* **Method:**

  `GET`
  
*  **URL Params**

   **Required:**
   
    - `menuaction=bookingfrontend.uidocument_building.download`
    - `id=[integer]`
    
   
* **Data Params**

    - `filter_owner_id[integer]`
    - `phpgw_return_as=[string]`


* **Success Response:**

  * **Code:** 200 <br />
    **Content:**
```
{
 
}
```
