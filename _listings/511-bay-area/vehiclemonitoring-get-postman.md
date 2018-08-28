{
  "info": {
    "name": "Bay Area 511 Transit API San Francisco 511 Vehicle Monitoring API",
    "_postman_id": "6c35eed2-560e-48d8-9ecc-a1fed571e706",
    "description": "San francisco 511 vehicle monitoring api.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "511",
      "item": [
        {
          "id": "6a6e0b73-4197-4e30-af8f-d3af65f5ab15",
          "name": "LinesGet",
          "request": {
            "url": "http://api.511.org/transit/lines?api_key=%7B%7D&operator_id=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "San francisco 511 transit lines api."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8bc00484-8bb3-4cc7-b0ff-a5ed8703136e"
            }
          ]
        },
        {
          "id": "caa516da-e45d-4887-a25b-8cbe131e07ee",
          "name": "PatternsGet",
          "request": {
            "url": "http://api.511.org/transit/patterns?api_key=%7B%7D&operator_id=%7B%7D&pattern_id=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "San francisco 511 transit transit patterns api."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9e130fc6-3d34-4f7c-8a50-3f394981e6c8"
            }
          ]
        },
        {
          "id": "36883c1d-c3ba-41d9-9a83-249df61ea559",
          "name": "StopsGet",
          "request": {
            "url": "http://api.511.org/transit/stops?api_key=%7B%7D&operator_id=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "San francisco 511 transit stops api."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "12408730-a6f9-4158-9ab6-fc4f1ec84065"
            }
          ]
        },
        {
          "id": "960ee650-a10c-4d4d-9c14-c6d6968e60ed",
          "name": "StopMonitoringGet",
          "request": {
            "url": "http://api.511.org/transit/StopMonitoring?agency=%7B%7D&api_key=%7B%7D&stopCode=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "San francisco 511 transit stop monitoring api."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "44de1eeb-2a40-4c6a-8501-cde4aca7ac36"
            }
          ]
        },
        {
          "id": "08a69dfa-09cd-411c-b63b-2eac703cc544",
          "name": "StoptimetableGet",
          "request": {
            "url": "http://api.511.org/transit/stoptimetable?api_key=%7B%7D&MonitoringRef=%7B%7D&OperatorRef=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "San francisco 511 transit stop timetable api."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7ceb6005-90d2-4d25-9962-afcb22419669"
            }
          ]
        },
        {
          "id": "ee268e12-085e-4df7-8be0-d56d272f13b7",
          "name": "GeneralAnnouncementsGet",
          "request": {
            "url": "http://api.511.org/transit/GeneralAnnouncements?api_key=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "San francisco 511 general announcements api."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "89a7611b-60c0-48fb-9f98-696421625da6"
            }
          ]
        },
        {
          "id": "1bf6f92e-723c-4896-8d57-7f86bc8764c4",
          "name": "StopPlacesGet",
          "request": {
            "url": "http://api.511.org/transit/stopPlaces?api_key=%7B%7D&operator_id=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "San francisco 511 transit stop places api."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c602200c-a476-40e0-93c9-393e81c30dae"
            }
          ]
        },
        {
          "id": "49e625a4-a24d-4791-b77d-f17e090d78d0",
          "name": "VehicleMonitoringGet",
          "request": {
            "url": "http://api.511.org/transit/VehicleMonitoring?agency=%7B%7D&api_key=%7B%7D&stopCode=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "San francisco 511 vehicle monitoring api."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "31828ac2-a187-48c5-8e43-c777cb52c4f9"
            }
          ]
        }
      ]
    }
  ]
}