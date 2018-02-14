## Portico Estate API Documentation

- [Search](#search)
- [Resource](#resource)
- [Document](#document)
- [Document download](#document-download)
- [Images](#images)
- [Organization users](#organization-users)


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
    
   **Optional:**
   
    - `filter_search_type=[string]`
    - `filter_part_of_town=[integer]`
    - `filter_top_level=[integer]`
    - `phpgw_return_as=[string]`


* **Response:**
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
    
   
   **Optional:**
   
    - `filter_building_id=[integer]`
    - `phpgw_return_as=[string]`


* **Response:**
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





**Organization users**
----
  Returns json data for users of organization.

* **URL**

  /bookingfrontend/?

* **Method:**

  `GET`
  
*  **URL Params**

   **Required:**
   
    - `menuaction=bookingfrontend.uiorganization.building_users`
    - `building_id=[integer]`
    
   **Optional:**
   
    - `sort=[string]`
    - `results[integer]`
    - `startIndex[integer]`
    - `phpgw_return_as=[string]`


* **Response:**
```
{
  "ResultSet": {
    "totalResultsAvailable": 2,
    "totalRecords": 2,
    "recordsReturned": 2,
    "pageSize": 10,
    "startIndex": 0,
    "sortKey": "name",
    "sortDir": "asc",
    "Result": [
      {
        "id": 183,
        "organization_number": "",
        "name": "Austb\u00f8 Skole",
        "shortname": "Austb\u00f8",
        "homepage": "",
        "phone": "51856332",
        "email": "aasmund.glende.jakobsen@stavanger.kommune.no",
        "description": "<br>Austb\u00f8 Skole",
        "street": "Austb\u00f8svingene 50",
        "zip_code": "4085",
        "district": "Hundv\u00e5g",
        "city": "Hundv\u00e5g",
        "active": 1,
        "show_in_portal": 0,
        "activity_id": 97,
        "customer_identifier_type": "",
        "customer_number": "",
        "customer_ssn": "",
        "customer_organization_number": "",
        "customer_internal": 1,
        "activity_name": "Skole",
        "contacts": [
          {
            "name": "\u00c5smund Glende Jakobsen",
            "ssn": "",
            "email": "aasmund.glende.jakobsen@stavanger.kommune.no",
            "phone": "51856332"
          },
          {
            "name": "Eva Walde Lund",
            "ssn": "",
            "email": "eva.walde.lund@stavanger.kommune.no",
            "phone": "51856335"
          }
        ],
        "link": "\/PorticoEstate\/bookingfrontend\/?menuaction=bookingfrontend.uiorganization.show&amp;id=183&amp;domain=default&amp;bookingfrontendsession=bjd2fum5r5j9i781714tr0bkk1&amp;click_history=14ac1c864b54d432b959c182a28ebd13"
      },
      {
        "id": 178,
        "organization_number": "",
        "name": "Renhold",
        "shortname": "Renhold",
        "homepage": "",
        "phone": "",
        "email": "",
        "description": "",
        "street": "",
        "zip_code": "",
        "district": "",
        "city": "",
        "active": 1,
        "show_in_portal": 0,
        "activity_id": 57,
        "customer_identifier_type": "",
        "customer_number": "",
        "customer_ssn": "",
        "customer_organization_number": "",
        "customer_internal": 1,
        "activity_name": "x Annet",
        "contacts": [
          {
            "name": "",
            "ssn": "",
            "email": "",
            "phone": ""
          },
          {
            "name": "",
            "ssn": "",
            "email": "",
            "phone": ""
          }
        ],
        "link": "\/PorticoEstate\/bookingfrontend\/?menuaction=bookingfrontend.uiorganization.show&amp;id=178&amp;domain=default&amp;bookingfrontendsession=bjd2fum5r5j9i781714tr0bkk1&amp;click_history=14ac1c864b54d432b959c182a28ebd13"
      }
    ],
    "actions": null
  }
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
    
   **Optional:**
   
    - `sort=[string]`
    - `no_images[integer]`
    - `filter_owner_id[integer]`
    - `phpgw_return_as=[string]`


* **Response:**
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


**Document download**
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
    
    
    **Optional:**

    - `filter_owner_id[integer]`
    - `phpgw_return_as=[string]`


* **Response:**

```
{
 
}
```




**Images**
----
  Returns json data for a building images.

* **URL**

  /bookingfrontend/?

* **Method:**

  `GET`
  
*  **URL Params**

   **Required:**
   
    - `menuaction=bookingfrontend.uidocument_building.index_images`
    
   **Optional:**
   
    - `sort[string]`
    - `filter_owner_id[integer]`  
    - `phpgw_return_as=[string]`


* **Response:**
```
{
  "ResultSet": {
    "totalResultsAvailable": 2,
    "totalRecords": 2,
    "recordsReturned": 2,
    "pageSize": 10,
    "startIndex": null,
    "sortKey": null,
    "sortDir": null,
    "Result": [
      {
        "id": 41,
        "name": "Fotballbaner 191.JPG",
        "owner_id": 27,
        "category": "picture",
        "description": "Hafrsfjord skole grusbane",
        "owner_name": "Hafrsfjord skole fotballbane",
        "is_image": true,
        "src": "\/PorticoEstate\/bookingfrontend\/?menuaction=bookingfrontend.uidocument_building.download&amp;id=41&amp;filter_owner_id=27&amp;domain=default&amp;bookingfrontendsession=ksmbnfpqpfpfji794uun4cd994&amp;click_history=ade6d4550f0ca66c486404d0d6d1068e"
      },
      {
        "id": 95,
        "name": "oversikt hafrs 2013.jpg",
        "owner_id": 27,
        "category": "picture",
        "description": "Oversikt over Hafrsfjord skole grusbane",
        "owner_name": "Hafrsfjord skole fotballbane",
        "is_image": true,
        "src": "\/PorticoEstate\/bookingfrontend\/?menuaction=bookingfrontend.uidocument_building.download&amp;id=95&amp;filter_owner_id=27&amp;domain=default&amp;bookingfrontendsession=ksmbnfpqpfpfji794uun4cd994&amp;click_history=ade6d4550f0ca66c486404d0d6d1068e"
      }
    ],
    "actions": null
  }
}
```
