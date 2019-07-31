---
title: chatInfo リソースの種類
description: Microsoft Teams のメッセージに関する情報。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5a2c7b705078e49c7e3bd68056b698e05d3f83bb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012976"
---
# <a name="chatinfo-resource-type"></a><span data-ttu-id="e16b5-103">chatInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e16b5-103">chatInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e16b5-104">Microsoft Teams のメッセージに関する情報。</span><span class="sxs-lookup"><span data-stu-id="e16b5-104">Information about a message in Microsoft Teams.</span></span>

## <a name="properties"></a><span data-ttu-id="e16b5-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e16b5-105">Properties</span></span>

| <span data-ttu-id="e16b5-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e16b5-106">Property</span></span>            | <span data-ttu-id="e16b5-107">型</span><span class="sxs-lookup"><span data-stu-id="e16b5-107">Type</span></span>    | <span data-ttu-id="e16b5-108">説明</span><span class="sxs-lookup"><span data-stu-id="e16b5-108">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="e16b5-109">messageId</span><span class="sxs-lookup"><span data-stu-id="e16b5-109">messageId</span></span>           | <span data-ttu-id="e16b5-110">String</span><span class="sxs-lookup"><span data-stu-id="e16b5-110">String</span></span>  | <span data-ttu-id="e16b5-111">Microsoft Teams チャネル内のメッセージの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="e16b5-111">The unique identifier for a message in a Microsoft Teams channel.</span></span> |
| <span data-ttu-id="e16b5-112">replyChainMessageId</span><span class="sxs-lookup"><span data-stu-id="e16b5-112">replyChainMessageId</span></span> | <span data-ttu-id="e16b5-113">String</span><span class="sxs-lookup"><span data-stu-id="e16b5-113">String</span></span>  | <span data-ttu-id="e16b5-114">返信メッセージの ID。</span><span class="sxs-lookup"><span data-stu-id="e16b5-114">The ID of the reply message.</span></span> |
| <span data-ttu-id="e16b5-115">Id</span><span class="sxs-lookup"><span data-stu-id="e16b5-115">threadId</span></span>            | <span data-ttu-id="e16b5-116">String</span><span class="sxs-lookup"><span data-stu-id="e16b5-116">String</span></span>  | <span data-ttu-id="e16b5-117">Microsoft Teams のスレッドの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="e16b5-117">The unique identifier for a thread in Microsoft Teams.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e16b5-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e16b5-118">JSON representation</span></span>

<span data-ttu-id="e16b5-119">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e16b5-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatInfo"
}-->
```json
{
  "messageId": "String",
  "replyChainMessageId": "String",
  "threadId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chatInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
