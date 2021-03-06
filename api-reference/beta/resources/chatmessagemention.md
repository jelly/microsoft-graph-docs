---
title: "chatMessageMention resource type"
description: "Represents a mention in a chatMessage entity. The mention can be to a user, team, bot or channel. "
localization_priority: Normal
author: nkramer
---

# chatMessageMention resource type

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represents a mention in a [chatMessage](chatmessage.md) entity. The mention can be to a user, team, bot, or channel. 

## Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|id|int|Index of the entity being mentioned. Matches with the <at id="index"> tag of the message body.|
|mentionText|string|String used to represent the mention. For example, User display name, Team name.|
|mentioned|[identitySet](identityset.md)|The entity (user, application, team, or channel) that was mentioned.|

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageMention"
}-->

```json
{
  "id": "number",
  "mentionText": "string",
  "mentioned": "microsoft.graph.identitySet"
 }

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chatmessagemention.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
