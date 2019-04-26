---
title: chatinfo リソースの種類
description: Microsoft Teams のメッセージに関する情報。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 552844795d3ba7e8ad4c8a3c3a6dff3c18990bc2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339696"
---
# <a name="chatinfo-resource-type"></a><span data-ttu-id="6af1d-103">chatinfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6af1d-103">chatInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6af1d-104">Microsoft Teams のメッセージに関する情報。</span><span class="sxs-lookup"><span data-stu-id="6af1d-104">Information about a message in Microsoft Teams.</span></span>

## <a name="properties"></a><span data-ttu-id="6af1d-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6af1d-105">Properties</span></span>

| <span data-ttu-id="6af1d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6af1d-106">Property</span></span>            | <span data-ttu-id="6af1d-107">型</span><span class="sxs-lookup"><span data-stu-id="6af1d-107">Type</span></span>    | <span data-ttu-id="6af1d-108">説明</span><span class="sxs-lookup"><span data-stu-id="6af1d-108">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="6af1d-109">messageId</span><span class="sxs-lookup"><span data-stu-id="6af1d-109">messageId</span></span>           | <span data-ttu-id="6af1d-110">String</span><span class="sxs-lookup"><span data-stu-id="6af1d-110">String</span></span>  | <span data-ttu-id="6af1d-111">Microsoft Teams チャネル内のメッセージの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="6af1d-111">The unique identifier for a message in a Microsoft Teams channel.</span></span> |
| <span data-ttu-id="6af1d-112">replyChainMessageId</span><span class="sxs-lookup"><span data-stu-id="6af1d-112">replyChainMessageId</span></span> | <span data-ttu-id="6af1d-113">String</span><span class="sxs-lookup"><span data-stu-id="6af1d-113">String</span></span>  | <span data-ttu-id="6af1d-114">返信メッセージの ID。</span><span class="sxs-lookup"><span data-stu-id="6af1d-114">The ID of the reply message.</span></span> |
| <span data-ttu-id="6af1d-115">id</span><span class="sxs-lookup"><span data-stu-id="6af1d-115">threadId</span></span>            | <span data-ttu-id="6af1d-116">String</span><span class="sxs-lookup"><span data-stu-id="6af1d-116">String</span></span>  | <span data-ttu-id="6af1d-117">Microsoft Teams のスレッドの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="6af1d-117">The unique identifier for a thread in Microsoft Teams.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6af1d-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6af1d-118">JSON representation</span></span>

<span data-ttu-id="6af1d-119">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6af1d-119">The following is a JSON representation of the resource.</span></span>

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
