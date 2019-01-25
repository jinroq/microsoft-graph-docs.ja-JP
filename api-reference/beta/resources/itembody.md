---
title: itemBody リソースの種類
description: メッセージ、イベント、またはグループの投稿など、アイテムの本文のプロパティを表します。
localization_priority: Normal
ms.openlocfilehash: f316beda82f292e62d5063f45363e08eeeff7111
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526145"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="48b90-103">itemBody リソースの種類</span><span class="sxs-lookup"><span data-stu-id="48b90-103">itemBody resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48b90-104">メッセージ、イベント、またはグループの投稿など、アイテムの本文のプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="48b90-104">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="48b90-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="48b90-105">Properties</span></span>
| <span data-ttu-id="48b90-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="48b90-106">Property</span></span>     | <span data-ttu-id="48b90-107">型</span><span class="sxs-lookup"><span data-stu-id="48b90-107">Type</span></span>   |<span data-ttu-id="48b90-108">説明</span><span class="sxs-lookup"><span data-stu-id="48b90-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48b90-109">content</span><span class="sxs-lookup"><span data-stu-id="48b90-109">content</span></span>|<span data-ttu-id="48b90-110">String</span><span class="sxs-lookup"><span data-stu-id="48b90-110">String</span></span>|<span data-ttu-id="48b90-111">アイテムのコンテンツ。</span><span class="sxs-lookup"><span data-stu-id="48b90-111">The content of the item.</span></span>|
|<span data-ttu-id="48b90-112">contentType</span><span class="sxs-lookup"><span data-stu-id="48b90-112">contentType</span></span>|<span data-ttu-id="48b90-113">String</span><span class="sxs-lookup"><span data-stu-id="48b90-113">String</span></span>|<span data-ttu-id="48b90-p101">コンテンツの種類。可能な値は、`Text` と `HTML` です。</span><span class="sxs-lookup"><span data-stu-id="48b90-p101">The type of the content. Possible values are `Text` and `HTML`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="48b90-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="48b90-116">JSON representation</span></span>

<span data-ttu-id="48b90-117">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="48b90-117">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.itemBody"
}-->

```json
{
  "content": "string",
  "contentType": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "itemBody resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/itembody.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
