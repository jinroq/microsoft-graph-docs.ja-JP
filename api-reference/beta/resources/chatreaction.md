---
title: chatMessageReaction リソースの種類
description: 'ChatMessage エンティティへの対応を表します。 '
localization_priority: Normal
ms.openlocfilehash: 5020653ef02c1604aece46f3ff2c7ea1c82a75ec
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810067"
---
# <a name="chatmessagereaction-resource-type"></a><span data-ttu-id="4555b-103">chatMessageReaction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4555b-103">chatMessageReaction resource type</span></span>

<span data-ttu-id="4555b-104">[ChatMessage](chatmessage.md)エンティティへの対応を表します。</span><span class="sxs-lookup"><span data-stu-id="4555b-104">Represents a reaction to a [chatMessage](chatmessage.md) entity.</span></span> 

<span data-ttu-id="4555b-105">エンティティの種類の`chatMessageReaction` [chatMessage](chatmessage.md)エンティティの一部として、[チャネルのメッセージを取得する](../api/channel-get-message.md)API の一部として返されます。</span><span class="sxs-lookup"><span data-stu-id="4555b-105">An entity of type `chatMessageReaction` is returned as part of the [Get channel messages](../api/channel-get-message.md) API, as a part of [chatMessage](chatmessage.md) entity.</span></span>

## <a name="properties"></a><span data-ttu-id="4555b-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4555b-106">Properties</span></span>
| <span data-ttu-id="4555b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4555b-107">Property</span></span>     | <span data-ttu-id="4555b-108">種類</span><span class="sxs-lookup"><span data-stu-id="4555b-108">Type</span></span>   |<span data-ttu-id="4555b-109">説明</span><span class="sxs-lookup"><span data-stu-id="4555b-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4555b-110">reactionType</span><span class="sxs-lookup"><span data-stu-id="4555b-110">reactionType</span></span>|<span data-ttu-id="4555b-111">文字列</span><span class="sxs-lookup"><span data-stu-id="4555b-111">string</span></span>| <span data-ttu-id="4555b-112">反応の型。</span><span class="sxs-lookup"><span data-stu-id="4555b-112">The type of reaction.</span></span> <span data-ttu-id="4555b-113">計画値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="4555b-113">Planned values include:</span></span> <br><ul><li><span data-ttu-id="4555b-114">-のようなメッセージのようなコンテンツは空白でもです。</span><span class="sxs-lookup"><span data-stu-id="4555b-114">Like - Like a message, content is blank in this case.</span></span></li><li><span data-ttu-id="4555b-115">Emoji の Emoji の反力です。</span><span class="sxs-lookup"><span data-stu-id="4555b-115">Emoji - Emoji reaction.</span></span> <span data-ttu-id="4555b-116">コンテンツは、絵文字の unicode 値に設定されています。</span><span class="sxs-lookup"><span data-stu-id="4555b-116">Content is set to unicode value of the emoji.</span></span></li><li><span data-ttu-id="4555b-117">ラベルの内容は、ラベル内の文字列に設定されます。</span><span class="sxs-lookup"><span data-stu-id="4555b-117">Label - Content is set to the string in the label.</span></span></li></ul>|
|<span data-ttu-id="4555b-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4555b-118">createdDateTime</span></span>|<span data-ttu-id="4555b-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4555b-119">dateTimeOffset</span></span>|<span data-ttu-id="4555b-120">ISO 8601 形式のメッセージ ルートの utc 形式のタイムスタンプです。</span><span class="sxs-lookup"><span data-stu-id="4555b-120">UTC timestamp of the root message in ISO-8601 format.</span></span>|
|<span data-ttu-id="4555b-121">user</span><span class="sxs-lookup"><span data-stu-id="4555b-121">user</span></span>|<span data-ttu-id="4555b-122">identitySet</span><span class="sxs-lookup"><span data-stu-id="4555b-122">identitySet</span></span>|<span data-ttu-id="4555b-123">メッセージに反応するユーザーです。</span><span class="sxs-lookup"><span data-stu-id="4555b-123">The user who reacted to the message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4555b-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4555b-124">JSON representation</span></span>

<span data-ttu-id="4555b-125">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4555b-125">The following is a JSON representation of the resource.</span></span>

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
