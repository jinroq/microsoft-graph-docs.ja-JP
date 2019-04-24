---
title: chatinfo リソースの種類
description: Microsoft Teams のメッセージに関する情報。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3c1414d10a262280bcf0d3a307fc0c71aed2fbde
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461074"
---
# <a name="chatinfo-resource-type"></a><span data-ttu-id="7b5de-103">chatinfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7b5de-103">chatInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b5de-104">Microsoft Teams のメッセージに関する情報。</span><span class="sxs-lookup"><span data-stu-id="7b5de-104">Information about a message in Microsoft Teams.</span></span>

## <a name="properties"></a><span data-ttu-id="7b5de-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7b5de-105">Properties</span></span>

| <span data-ttu-id="7b5de-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7b5de-106">Property</span></span>            | <span data-ttu-id="7b5de-107">型</span><span class="sxs-lookup"><span data-stu-id="7b5de-107">Type</span></span>    | <span data-ttu-id="7b5de-108">説明</span><span class="sxs-lookup"><span data-stu-id="7b5de-108">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="7b5de-109">messageId</span><span class="sxs-lookup"><span data-stu-id="7b5de-109">messageId</span></span>           | <span data-ttu-id="7b5de-110">String</span><span class="sxs-lookup"><span data-stu-id="7b5de-110">String</span></span>  | <span data-ttu-id="7b5de-111">Microsoft Teams チャネル内のメッセージの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="7b5de-111">The unique identifier for a message in a Microsoft Teams channel.</span></span> |
| <span data-ttu-id="7b5de-112">replyChainMessageId</span><span class="sxs-lookup"><span data-stu-id="7b5de-112">replyChainMessageId</span></span> | <span data-ttu-id="7b5de-113">String</span><span class="sxs-lookup"><span data-stu-id="7b5de-113">String</span></span>  | <span data-ttu-id="7b5de-114">返信メッセージの ID。</span><span class="sxs-lookup"><span data-stu-id="7b5de-114">The ID of the reply message.</span></span> |
| <span data-ttu-id="7b5de-115">id</span><span class="sxs-lookup"><span data-stu-id="7b5de-115">threadId</span></span>            | <span data-ttu-id="7b5de-116">String</span><span class="sxs-lookup"><span data-stu-id="7b5de-116">String</span></span>  | <span data-ttu-id="7b5de-117">Microsoft Teams のスレッドの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="7b5de-117">The unique identifier for a thread in Microsoft Teams.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7b5de-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7b5de-118">JSON representation</span></span>

<span data-ttu-id="7b5de-119">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7b5de-119">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/chatInfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
