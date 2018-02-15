## Portico Estate API Documentation

- [Search](#search)
- [Building](#building)
- [Building users](#building-users)
- [Building documents](#building-document)
- [Building document download](#building-document-download)
- [Building images](#building-images)
- [Resource](#resource)
- [Resource images](#resource-images)
- [Resource images(2)](#resource-images-2)
- [Resource schedule](#resource-schedule)
- [Organization](#organization)
- [Organization delegate](#organization-delegate)
- [Building & construction used by a organization](#building-&-construction-used-by-a-organization)
- [Organization documents](#organization-documents)

**Search**
---- 
  Search for facilities or resources. Returns json data.

* **URL**

  /bookingfrontend/?

* **Method:**

  `GET`
  
*  **URL Params**

   **Required:**
   
    - `menuaction=bookingfrontend.uisearch.query`
    - `searchterm=[string]`
    
   **Optional:**
   
    - `filter_search_type=[string]`         (filter by building or resource)
    - `filter_part_of_town=[integer]`       (filter by town id)
    - `filter_top_level=[integer]`          (filter by categories/department. eg. sports(2) or school(97))
    - `phpgw_return_as=[string]`            (return value type eg. json or stripped_html)


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
        "link": "\/PorticoEstate\/bookingfrontend\/?menuaction=bookingfrontend.uibuilding.show&amp;id=18&amp;",
        "img_container": "building-18",
        "img_url": "\/PorticoEstate\/bookingfrontend\/?menuaction=bookingfrontend.uidocument_building.index_images&amp;filter_owner_id=18&amp;phpgw_return_as=json&amp;results=1&amp;"
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





**Building**
----
  Returns json data of all buildings.

* **URL**

  /bookingfrontend/?

* **Method:**

  `GET`
  
*  **URL Params**

   **Required:**
   
    - `menuaction=bookingfrontend.uibuilding.index`
    
   **Optional:**
   
    - `phpgw_return_as=[string]`


* **Response:**
```
 {
  "start": 0,
  "sort": null,
  "dir": "asc",
  "recordsTotal": 84,
  "recordsFiltered": 84,
  "data": [
    {
      "id": 7,
      "name": "Tastahallen",
      "homepage": "www.stavanger.kommune.no",
      "calendar_text": "",
      "description": "",
      "phone": "51507270",
      "email": "tastahallen@stavanger.kommune.no",
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
      "location_code": "5071",
      "activity_id": 2,
      "part_of_town_id": "7",
      "street": "Fredtunveien 10",
      "zip_code": "4026",
      "district": "Tasta",
      "city": "Stavanger",
      "active": 1,
      "activity_name": "Idrett",
      "link": "\/PorticoEstate\/bookingfrontend\/?menuaction=bookingfrontend.uibuilding.show&amp;id=7&amp;"
    },
    {
      "id": 33,
      "name": "Jarlebanen",
      "homepage": "",
      "calendar_text": "",
      "description": "Jarlebanen best\u00e5r av en fotballbane og Jarl FKs 2 garderober og klubbhus.",
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
      "location_code": "5017",
      "activity_id": 2,
      "part_of_town_id": "2",
      "street": "Jarlebanen",
      "zip_code": "4016",
      "district": "Hillev\u00e5g",
      "city": "Stavanger",
      "active": 1,
      "activity_name": "Idrett",
      "link": "\/PorticoEstate\/bookingfrontend\/?menuaction=bookingfrontend.uibuilding.show&amp;id=33&amp;"
    }
  ]
}
```



**Building users**
----
  Returns json data for users of building.

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
        "link": "\/PorticoEstate\/bookingfrontend\/?menuaction=bookingfrontend.uiorganization.show&amp;id=183&amp;domain=default&amp;"
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
        "link": "\/PorticoEstate\/bookingfrontend\/?menuaction=bookingfrontend.uiorganization.show&amp;id=178&amp;domain=default&amp;"
      }
    ],
    "actions": null
  }
}

```




**Building documents**
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
      "link": "\/PorticoEstate\/bookingfrontend\/?menuaction=bookingfrontend.uidocument_building.download&amp;id=361&amp;filter_owner_id=27&amp;"
    },
    {
      "id": 360,
      "name": "Reglement for bruk av kommunale idrettsanlegg.pdf",
      "owner_id": 27,
      "category": "Reglement",
      "description": "Reglement for bruk av kommunale idrettsanlegg",
      "owner_name": "Hafrsfjord skole fotballbane",
      "is_image": false,
      "link": "\/PorticoEstate\/bookingfrontend\/?menuaction=bookingfrontend.uidocument_building.download&amp;id=360&amp;filter_owner_id=27&amp;"
    }
  ]
}
```


**Building document download**
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






**Building images**
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
        "src": "\/PorticoEstate\/bookingfrontend\/?menuaction=bookingfrontend.uidocument_building.download&amp;id=41&amp;filter_owner_id=27&amp;"
      },
      {
        "id": 95,
        "name": "oversikt hafrs 2013.jpg",
        "owner_id": 27,
        "category": "picture",
        "description": "Oversikt over Hafrsfjord skole grusbane",
        "owner_name": "Hafrsfjord skole fotballbane",
        "is_image": true,
        "src": "\/PorticoEstate\/bookingfrontend\/?menuaction=bookingfrontend.uidocument_building.download&amp;id=95&amp;filter_owner_id=27"
      }
    ],
    "actions": null
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
      "link": "\/PorticoEstate\/bookingfrontend\/?menuaction=bookingfrontend.uiresource.show&amp;id=37&amp;",
      "building_street": "Madlasandnes",
      "building_city": "4045",
      "building_district": "Madla",
      "building_name": "Hafrsfjord skole fotballbane (Idrett)",
      "full_name": "Hafrsfjord skole fotballbane (Idrett) \/ Grus (40 x 80)"
    }
  ]
}
```




**Resource images**
----
  Returns json data for resource images.

* **URL**

  /bookingfrontend/?

* **Method:**

  `GET`
  
*  **URL Params**

   **Required:**
   
    - `menuaction=bookingfrontend.uidocument_resource.index`
    
   
   **Optional:**
   
    - `filter_owner_id=[integer]`
    - `no_images=[integer]`
    - `sort=[string]`
    - `phpgw_return_as=[string]`


* **Response:**
```
 {
  "start": 0,
  "sort": "name",
  "dir": "asc",
  "recordsTotal": 1,
  "recordsFiltered": 1,
  "data": [
    {
      "id": 164,
      "name": "Hall A.jpeg",
      "owner_id": 89,
      "category": "Bilde",
      "description": "Hall A",
      "owner_name": "Hall A",
      "is_image": true,
      "link": "\/PorticoEstate\/bookingfrontend\/?menuaction=bookingfrontend.uidocument_resource.download&amp;id=164&amp;filter_owner_id=89&amp;"
    }
  ]
}
```





**Resource images 2**
----
  Returns json data for resource images.

* **URL**

  /bookingfrontend/?

* **Method:**

  `GET`
  
*  **URL Params**

   **Required:**
   
    - `menuaction=bookingfrontend.uidocument_resource.index_images`
    
   
   **Optional:**
   
    - `filter_owner_id=[integer]`
    - `sort=[string]`
    - `phpgw_return_as=[string]`


* **Response:**
```
{
  "ResultSet": {
    "totalResultsAvailable": 1,
    "totalRecords": 1,
    "recordsReturned": 1,
    "pageSize": 10,
    "startIndex": null,
    "sortKey": null,
    "sortDir": null,
    "Result": [
      {
        "id": 164,
        "name": "Hall A.jpeg",
        "owner_id": 89,
        "category": "picture",
        "description": "Hall A",
        "owner_name": "Hall A",
        "is_image": true,
        "src": "\/PorticoEstate\/bookingfrontend\/?menuaction=bookingfrontend.uidocument_resource.download&amp;id=164&amp;filter_owner_id=89&amp;"
      }
    ],
    "actions": null
  }
}
```






**Resource schedule**
----
  Returns json data for resource schedule.

* **URL**

  /bookingfrontend/?

* **Method:**

  `POST`
  
*  **URL Params**

   **Required:**
   
    - `menuaction=bookingfrontend.uiresource.schedule`
    - `id=[integer]`
   
   **Optional:**
   
    - `date=[date]`
    - `phpgw_return_as=[string]`


* **Response:**
```
{
  "ResultSet": {
    "totalResultsAvailable": 6,
    "Result": [
      {
        "time": "00:00-08:30",
        "_from": "00:00",
        "_to": "08:30",
        "link": "\/PorticoEstate\/bookingfrontend\/?menuaction=bookingfrontend.uibooking.show&amp;"
      },
      {
        "resource": "Hall A",
        "resource_id": 89,
        "time": "08:30-09:25",
        "_from": "08:30",
        "_to": "09:25",
        "Wed": {
          "id": 266481,
          "id_string": "266481",
          "active": 1,
          "application_id": null,
          "organization_id": 178,
          "building_name": "Hundv\u00e5ghallen",
          "season_id": 396,
          "from_": "08:30",
          "to_": "09:25",
          "cost": 0,
          "completed": 1,
          "organization_name": "Renhold",
          "organization_shortname": "Renhold",
          "building_id": "4",
          "season_name": "Inne 2017\/2018 dag",
          "resources": [
            89
          ],
          "costs": "",
          "name": "Renhold",
          "shortname": "Renhold",
          "type": "allocation",
          "date": "2018-02-14",
          "wday": "Wed",
          "info_url": "\/PorticoEstate\/bookingfrontend\/?menuaction=bookingfrontend.uiallocation.info&amp;id=266481&amp;"
        },
        "Thu": {
          "id": 266487,
          "id_string": "266487",
          "active": 1,
          "application_id": null,
          "organization_id": 184,
          "building_name": "Hundv\u00e5ghallen",
          "season_id": 396,
          "from_": "08:30",
          "to_": "09:25",
          "cost": 0,
          "completed": 1,
          "organization_name": "Hundv\u00e5g skole",
          "organization_shortname": "Hundv\u00e5g",
          "building_id": "4",
          "season_name": "Inne 2017\/2018 dag",
          "resources": [
            89
          ],
          "costs": "",
          "name": "Hundv\u00e5g skole",
          "shortname": "Hundv\u00e5g",
          "type": "allocation",
          "date": "2018-02-15",
          "wday": "Thu",
          "info_url": "\/PorticoEstate\/bookingfrontend\/?menuaction=bookingfrontend.uiallocation.info&amp;id=266487&amp;"
        },
        "Mon": {
          "id": 266473,
          "id_string": "266473",
          "active": 1,
          "application_id": null,
          "organization_id": 178,
          "building_name": "Hundv\u00e5ghallen",
          "season_id": 396,
          "from_": "13:10",
          "to_": "16:00",
          "cost": 0,
          "completed": 1,
          "organization_name": "Renhold",
          "organization_shortname": "Renhold",
          "building_id": "4",
          "season_name": "Inne 2017\/2018 dag",
          "resources": [
            89
          ],
          "costs": "",
          "name": "Renhold",
          "shortname": "Renhold",
          "type": "allocation",
          "date": "2018-02-12",
          "wday": "Mon",
          "info_url": "\/PorticoEstate\/bookingfrontend\/?menuaction=bookingfrontend.uiallocation.info&amp;id=266473&amp;"
        },
        "link": "\/PorticoEstate\/bookingfrontend\/?menuaction=bookingfrontend.uibooking.show&amp;"
      },
      {
        "time": "16:00-00:00",
        "_from": "16:00",
        "_to": "00:00",
        "link": "\/PorticoEstate\/bookingfrontend\/?menuaction=bookingfrontend.uibooking.show&amp;"
      }
    ]
  }
}
```



**Organization**
----
  Returns json data for organization.

* **URL**

  /bookingfrontend/?

* **Method:**

  `GET`
  
*  **URL Params**

   **Required:**
   
    - `menuaction=bookingfrontend.uigroup.index`
    
   **Optional:**
   
    - `sort=[string]`
    - `filter_organization_id[integer]`
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
      "id": 154,
      "active": 1,
      "show_in_portal": 0,
      "organization_id": 128,
      "shortname": "SBS-BREDDE",
      "description": "",
      "name": "Bredde",
      "activity_id": 49,
      "activity_name": "Bueskyting",
      "organization_name": "Stavanger bueskyttere",
      "contacts": [
        {
          "name": "Helge salomonsen",
          "email": "Helge.salomonsen@lyse.net",
          "phone": "93420066"
        },
        {
          "name": "Ole-Kristian olufsen",
          "email": "Okolufsen@gmail.com",
          "phone": "92802745"
        }
      ],
      "link": "\/PorticoEstate\/bookingfrontend\/?menuaction=bookingfrontend.uigroup.show&amp;id=154&amp",
      "primary_contact_name": "Helge salomonsen",
      "primary_contact_phone": "93420066",
      "primary_contact_email": "Helge.salomonsen@lyse.net",
      "secondary_contact_name": "Ole-Kristian olufsen",
      "secondary_contact_phone": "92802745",
      "secondary_contact_email": "Okolufsen@gmail.com"
    },
    {
      "id": 153,
      "active": 1,
      "show_in_portal": 0,
      "organization_id": 128,
      "shortname": "SBS-SATS",
      "description": "",
      "name": "Satsningsgruppe",
      "activity_id": 49,
      "activity_name": "Bueskyting",
      "organization_name": "Stavanger bueskyttere",
      "contacts": [
        {
          "name": "Ole-Kristian olufsen",
          "email": "Okolufsen@gmail.com",
          "phone": "92802745"
        },
        {
          "name": "Ken Henry Tesaker",
          "email": "Kenht@broadpark.no",
          "phone": "90239221"
        }
      ],
      "link": "\/PorticoEstate\/bookingfrontend\/?menuaction=bookingfrontend.uigroup.show&amp;id=153&amp",
      "primary_contact_name": "Ole-Kristian olufsen",
      "primary_contact_phone": "92802745",
      "primary_contact_email": "Okolufsen@gmail.com",
      "secondary_contact_name": "Ken Henry Tesaker",
      "secondary_contact_phone": "90239221",
      "secondary_contact_email": "Kenht@broadpark.no"
    }
  ]
}
```










**Organization delegate**
----
  Returns json data for delegate.

* **URL**

  /bookingfrontend/?

* **Method:**

  `GET`
  
*  **URL Params**

   **Required:**
   
    - `menuaction=bookingfrontend.uidelegate.index`
    
   **Optional:**
   
    - `sort=[string]`
    - `filter_organization_id[integer]`
    - `filter_active[integer]`
    - `phpgw_return_as=[string]`


* **Response:**

```


```


**Building & construction used by a organization**
----
  Returns json data for building and construction used by a organization.

* **URL**

  /bookingfrontend/?

* **Method:**

  `GET`
  
*  **URL Params**

   **Required:**
   
    - `menuaction=bookingfrontend.uibuilding.find_buildings_used_by`
    
   **Optional:**
   
    - `sort=[string]`
    - `organization_id=[integer]`
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
        "id": 4,
        "name": "Hundv\u00e5ghallen",
        "homepage": "www.stavanger.kommune.no",
        "calendar_text": "",
        "description": "Hundv\u00e5ghallen<strong> <\/strong>finner du p\u00e5 Hundv\u00e5g.<br>Hallen inneholder to flerbrukshaller, styrkerom, m\u00f8terom og kafeteria.<br>Hall A er bygget i 1988, mens hall B ble bygget i 2008.<br><br><span VarCleaned=\"text-decoration: underline;\"><strong>\u00c5pningstider:<br><\/strong><\/span>Mandag-Fredag kl. 08.00-22.00<br>L\u00f8rdag kl. 10.00-17.00<br>S\u00f8ndag kl. 11.00-18.00",
        "phone": "51856150",
        "email": "hundvaghallen@stavanger.kommune.no",
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
        "location_code": "5040",
        "activity_id": 2,
        "part_of_town_id": "4",
        "street": "Austb\u00f8svingene 54",
        "zip_code": "4086",
        "district": "Hundv\u00e5g",
        "city": "Hundv\u00e5g",
        "active": 1,
        "activity_name": "Idrett",
        "link": "\/PorticoEstate\/bookingfrontend\/?menuaction=bookingfrontend.uibuilding.show&amp;id=4"
      },
      {
        "id": 85,
        "name": "Hundv\u00e5g sv\u00f8mmehall",
        "homepage": "",
        "calendar_text": "",
        "description": "",
        "phone": "51507610",
        "email": "hundvag.svommehall.51507610@stavanger.kommune.no",
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
        "location_code": "5044",
        "activity_id": null,
        "part_of_town_id": "4",
        "street": "Austb\u00f8geilen 35",
        "zip_code": "4085",
        "district": "Hundv\u00e5g",
        "city": "Hundv\u00e5g",
        "active": 1,
        "activity_name": "",
        "link": "\/PorticoEstate\/bookingfrontend\/?menuaction=bookingfrontend.uibuilding.show&amp;id=85&amp;"
      }
    ],
    "actions": null
  }
}

```





**Organization documents**
----
  Returns json data for organizations documents.

* **URL**

  /bookingfrontend/?

* **Method:**

  `GET`
  
*  **URL Params**

   **Required:**
   
    - `menuaction=bookingfrontend.uidocument_organization.index`
    
   **Optional:**
   
    - `sort=[string]`
    - `filter_owner_id=[integer]`
    - `no_images[integer]`
    - `phpgw_return_as=[string]`


* **Response:**

```


```

