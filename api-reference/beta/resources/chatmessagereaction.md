---
title: chatMessageReaction リソースの種類
description: 'ChatMessage エンティティへの反応を表します。 '
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 33fe5a881d05b2ac2bc86e97e11b00c3465a8c09
ms.sourcegitcommit: 624ac42e74533a9bf0d0d22b3b15adbb258fd594
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/05/2019
ms.locfileid: "34709426"
---
# <a name="chatmessagereaction-resource-type"></a><span data-ttu-id="325ea-103">chatMessageReaction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="325ea-103">chatMessageReaction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="325ea-104">[Chatmessage](chatmessage.md)エンティティへの反応を表します。</span><span class="sxs-lookup"><span data-stu-id="325ea-104">Represents a reaction to a [chatMessage](chatmessage.md) entity.</span></span> 

<span data-ttu-id="325ea-105">型`chatMessageReaction`のエンティティは、 [chatmessage](chatmessage.md)エンティティの一部として、 [Get channel message](../api/channel-get-message.md) API の一部として返されます。</span><span class="sxs-lookup"><span data-stu-id="325ea-105">An entity of type `chatMessageReaction` is returned as part of the [Get channel message](../api/channel-get-message.md) API, as a part of the [chatMessage](chatmessage.md) entity.</span></span>

## <a name="properties"></a><span data-ttu-id="325ea-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="325ea-106">Properties</span></span>

| <span data-ttu-id="325ea-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="325ea-107">Property</span></span>     | <span data-ttu-id="325ea-108">型</span><span class="sxs-lookup"><span data-stu-id="325ea-108">Type</span></span>        | <span data-ttu-id="325ea-109">説明</span><span class="sxs-lookup"><span data-stu-id="325ea-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="325ea-110">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="325ea-110">createdDateTime</span></span>|<span data-ttu-id="325ea-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="325ea-111">DateTimeOffset</span></span>|<span data-ttu-id="325ea-p101">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="325ea-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="325ea-114">reactionType</span><span class="sxs-lookup"><span data-stu-id="325ea-114">reactionType</span></span>|<span data-ttu-id="325ea-115">String</span><span class="sxs-lookup"><span data-stu-id="325ea-115">String</span></span>|<span data-ttu-id="325ea-116">計画される値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="325ea-116">Planned values include:</span></span> <br><ul><li><span data-ttu-id="325ea-117">Like-メッセージと同じですが、この場合、コンテンツは空白になります。</span><span class="sxs-lookup"><span data-stu-id="325ea-117">Like - Like a message, content is blank in this case.</span></span></li><li><span data-ttu-id="325ea-118">絵文字と絵文字の反応。</span><span class="sxs-lookup"><span data-stu-id="325ea-118">Emoji - Emoji reaction.</span></span> <span data-ttu-id="325ea-119">コンテンツは絵文字の unicode 値に設定されています。</span><span class="sxs-lookup"><span data-stu-id="325ea-119">Content is set to unicode value of the emoji.</span></span></li><li><span data-ttu-id="325ea-120">Label-コンテンツはラベル内の文字列に設定されます。</span><span class="sxs-lookup"><span data-stu-id="325ea-120">Label - Content is set to the string in the label.</span></span></li></ul>|
|<span data-ttu-id="325ea-121">user</span><span class="sxs-lookup"><span data-stu-id="325ea-121">user</span></span>|[<span data-ttu-id="325ea-122">identitySet</span><span class="sxs-lookup"><span data-stu-id="325ea-122">identitySet</span></span>](identityset.md)|<span data-ttu-id="325ea-123">メッセージに reacted したユーザー。</span><span class="sxs-lookup"><span data-stu-id="325ea-123">The user who reacted to the message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="325ea-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="325ea-124">JSON representation</span></span>

<span data-ttu-id="325ea-125">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="325ea-125">The following is a JSON representation of the resource.</span></span>

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
