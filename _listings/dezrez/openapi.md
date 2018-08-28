swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/role/auction/milestone/{roleId}/{milestoneId}:
    delete:
      summary: Delete a custom auction milestone
      description: Delete a custom auction milestone.
      operationId: AuctionRole_DeleteAuctionMilestoneByroleIdBymilestoneId
      x-api-path-slug: apiroleauctionmilestoneroleidmilestoneid-delete
      parameters:
      - in: path
        name: milestoneId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: roleId
      responses:
        200:
          description: OK
      tags:
      - Custom
      - Auction
      - Milestone
  /api/customfieldgroup/{typeName}:
    get:
      summary: Get a list of custom field groups for a type and optional group name
        specified.
      description: Get a list of custom field groups for a type and optional group
        name specified..
      operationId: CustomFieldGroup_GetBytypeNameBygroupName
      x-api-path-slug: apicustomfieldgrouptypename-get
      parameters:
      - in: query
        name: groupName
        description: An optional parameter to filter by group name
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: typeName
        description: The name of the type to get the custom field groups for
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Custom
      - Field
      - Groupsa
      - Type
      - Optional
      - Group
      - Name
      - Specified
  /api/customtextdescription/distinctcustompropertydescriptions:
    get:
      summary: Returns a list of the distinct defined custom descriptions for a property
      description: Returns a list of the distinct defined custom descriptions for
        a property.
      operationId: CustomTextDescription_DistinctCustomPropertyDescriptions
      x-api-path-slug: apicustomtextdescriptiondistinctcustompropertydescriptions-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Distinct
      - Defined
      - Custom
      - Descriptionsa
      - Property
  /api/locale/{culture}:
    get:
      summary: returns the json file containing localization for the app based on
        a culture string, and any custom values for the agent
      description: Returns the json file containing localization for the app based
        on a culture string, and any custom values for the agent.
      operationId: Locale_GetLocalisationFileByculture
      x-api-path-slug: apilocaleculture-get
      parameters:
      - in: path
        name: culture
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Json
      - File
      - Containing
      - Localizationthe
      - App
      - Based
      - "On"
      - Culture
      - String
      - ""
      - Any
      - Custom
      - Valuesthe
      - Agent
  /api/CustomField:
    put:
      summary: ""
      description: .
      operationId: CustomField_SaveCustomFieldValueBysaveCustomFieldValueCommandSaveDataContract
      x-api-path-slug: apicustomfield-put
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: saveCustomFieldValueCommandSaveDataContract
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - ""