---
title: chatmessagereaction リソースの種類
description: 'chatmessage エンティティへの反応を表します。 '
localization_priority: Normal
ms.openlocfilehash: 5020653ef02c1604aece46f3ff2c7ea1c82a75ec
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460640"
---
# <a name="chatmessagereaction-resource-type"></a><span data-ttu-id="15cb3-103">chatmessagereaction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="15cb3-103">chatMessageReaction resource type</span></span>

<span data-ttu-id="15cb3-104">[chatmessage](chatmessage.md)エンティティへの反応を表します。</span><span class="sxs-lookup"><span data-stu-id="15cb3-104">Represents a reaction to a [chatMessage](chatmessage.md) entity.</span></span> 

<span data-ttu-id="15cb3-105">型`chatMessageReaction`のエンティティは、 [chatmessage](chatmessage.md)エンティティの一部として、 [Get channel messages](../api/channel-get-message.md) API の一部として返されます。</span><span class="sxs-lookup"><span data-stu-id="15cb3-105">An entity of type `chatMessageReaction` is returned as part of the [Get channel messages](../api/channel-get-message.md) API, as a part of [chatMessage](chatmessage.md) entity.</span></span>

## <a name="properties"></a><span data-ttu-id="15cb3-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="15cb3-106">Properties</span></span>
| <span data-ttu-id="15cb3-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="15cb3-107">Property</span></span>     | <span data-ttu-id="15cb3-108">型</span><span class="sxs-lookup"><span data-stu-id="15cb3-108">Type</span></span>   |<span data-ttu-id="15cb3-109">説明</span><span class="sxs-lookup"><span data-stu-id="15cb3-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="15cb3-110">reactiontype</span><span class="sxs-lookup"><span data-stu-id="15cb3-110">reactionType</span></span>|<span data-ttu-id="15cb3-111">string</span><span class="sxs-lookup"><span data-stu-id="15cb3-111">string</span></span>| <span data-ttu-id="15cb3-112">反応の種類。</span><span class="sxs-lookup"><span data-stu-id="15cb3-112">The type of reaction.</span></span> <span data-ttu-id="15cb3-113">計画される値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="15cb3-113">Planned values include:</span></span> <br><ul><li><span data-ttu-id="15cb3-114">like-メッセージと同じですが、この場合、コンテンツは空白になります。</span><span class="sxs-lookup"><span data-stu-id="15cb3-114">Like - Like a message, content is blank in this case.</span></span></li><li><span data-ttu-id="15cb3-115">絵文字と絵文字の反応。</span><span class="sxs-lookup"><span data-stu-id="15cb3-115">Emoji - Emoji reaction.</span></span> <span data-ttu-id="15cb3-116">コンテンツは絵文字の unicode 値に設定されています。</span><span class="sxs-lookup"><span data-stu-id="15cb3-116">Content is set to unicode value of the emoji.</span></span></li><li><span data-ttu-id="15cb3-117">label-コンテンツはラベル内の文字列に設定されます。</span><span class="sxs-lookup"><span data-stu-id="15cb3-117">Label - Content is set to the string in the label.</span></span></li></ul>|
|<span data-ttu-id="15cb3-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="15cb3-118">createdDateTime</span></span>|<span data-ttu-id="15cb3-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15cb3-119">dateTimeOffset</span></span>|<span data-ttu-id="15cb3-120">ISO-8601 形式のルートメッセージの UTC タイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="15cb3-120">UTC timestamp of the root message in ISO-8601 format.</span></span>|
|<span data-ttu-id="15cb3-121">user</span><span class="sxs-lookup"><span data-stu-id="15cb3-121">user</span></span>|<span data-ttu-id="15cb3-122">identitySet</span><span class="sxs-lookup"><span data-stu-id="15cb3-122">identitySet</span></span>|<span data-ttu-id="15cb3-123">メッセージに reacted したユーザー。</span><span class="sxs-lookup"><span data-stu-id="15cb3-123">The user who reacted to the message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="15cb3-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="15cb3-124">JSON representation</span></span>

<span data-ttu-id="15cb3-125">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="15cb3-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "content"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageReaction"
}-->

```json
{
  "reactionType": "string ",
  "createdDateTime": "string (timestamp)",
  "user": {"@odata.type": "microsoft.graph.identitySet"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chat message reaction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
