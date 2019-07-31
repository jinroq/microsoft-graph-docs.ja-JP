---
title: chatMessageReaction リソースの種類
description: 'ChatMessage エンティティへの反応を表します。 '
localization_priority: Normal
doc_type: resourcePageType
author: RamjotSingh
ms.prod: microsoft-teams
ms.openlocfilehash: e1193e65697187f705f2758c2c195e5519326dc0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973990"
---
# <a name="chatmessagereaction-resource-type"></a><span data-ttu-id="b547d-103">chatMessageReaction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b547d-103">chatMessageReaction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b547d-104">[Chatmessage](chatmessage.md)エンティティへの反応を表します。</span><span class="sxs-lookup"><span data-stu-id="b547d-104">Represents a reaction to a [chatMessage](chatmessage.md) entity.</span></span> 

<span data-ttu-id="b547d-105">型`chatMessageReaction`のエンティティは、 [chatmessage](chatmessage.md)エンティティの一部として、 [Get channel message](../api/channel-get-message.md) API の一部として返されます。</span><span class="sxs-lookup"><span data-stu-id="b547d-105">An entity of type `chatMessageReaction` is returned as part of the [Get channel message](../api/channel-get-message.md) API, as a part of the [chatMessage](chatmessage.md) entity.</span></span>

## <a name="properties"></a><span data-ttu-id="b547d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b547d-106">Properties</span></span>

| <span data-ttu-id="b547d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b547d-107">Property</span></span>     | <span data-ttu-id="b547d-108">型</span><span class="sxs-lookup"><span data-stu-id="b547d-108">Type</span></span>        | <span data-ttu-id="b547d-109">説明</span><span class="sxs-lookup"><span data-stu-id="b547d-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b547d-110">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b547d-110">createdDateTime</span></span>|<span data-ttu-id="b547d-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b547d-111">DateTimeOffset</span></span>|<span data-ttu-id="b547d-p101">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b547d-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b547d-114">reactionType</span><span class="sxs-lookup"><span data-stu-id="b547d-114">reactionType</span></span>|<span data-ttu-id="b547d-115">String</span><span class="sxs-lookup"><span data-stu-id="b547d-115">String</span></span>|<span data-ttu-id="b547d-116">サポートされ`like`て`angry`いる`sad`値`laugh`は`heart`、 `surprised`、、、、です。</span><span class="sxs-lookup"><span data-stu-id="b547d-116">Supported values are `like`, `angry`, `sad`, `laugh`, `heart`, `surprised`.</span></span> |
|<span data-ttu-id="b547d-117">user</span><span class="sxs-lookup"><span data-stu-id="b547d-117">user</span></span>|[<span data-ttu-id="b547d-118">identitySet</span><span class="sxs-lookup"><span data-stu-id="b547d-118">identitySet</span></span>](identityset.md)|<span data-ttu-id="b547d-119">メッセージに reacted したユーザー。</span><span class="sxs-lookup"><span data-stu-id="b547d-119">The user who reacted to the message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b547d-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b547d-120">JSON representation</span></span>

<span data-ttu-id="b547d-121">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b547d-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatMessageReaction",
  "baseType": null
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "reactionType": "String",
  "user": {"@odata.type": "microsoft.graph.identitySet"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chatMessageReaction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
