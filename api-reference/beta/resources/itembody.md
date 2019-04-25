---
title: itemBody リソースの種類
description: メッセージ、イベント、またはグループの投稿など、アイテムの本文のプロパティを表します。
localization_priority: Normal
ms.openlocfilehash: 1cf79f78caa7b2772bc44b99c6b9bdc526340a87
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523491"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="ffe43-103">itemBody リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ffe43-103">itemBody resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ffe43-104">メッセージ、イベント、またはグループの投稿など、アイテムの本文のプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="ffe43-104">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="ffe43-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ffe43-105">Properties</span></span>
| <span data-ttu-id="ffe43-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ffe43-106">Property</span></span>     | <span data-ttu-id="ffe43-107">型</span><span class="sxs-lookup"><span data-stu-id="ffe43-107">Type</span></span>   |<span data-ttu-id="ffe43-108">説明</span><span class="sxs-lookup"><span data-stu-id="ffe43-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ffe43-109">content</span><span class="sxs-lookup"><span data-stu-id="ffe43-109">content</span></span>|<span data-ttu-id="ffe43-110">String</span><span class="sxs-lookup"><span data-stu-id="ffe43-110">String</span></span>|<span data-ttu-id="ffe43-111">アイテムのコンテンツ。</span><span class="sxs-lookup"><span data-stu-id="ffe43-111">The content of the item.</span></span>|
|<span data-ttu-id="ffe43-112">contentType</span><span class="sxs-lookup"><span data-stu-id="ffe43-112">contentType</span></span>|<span data-ttu-id="ffe43-113">String</span><span class="sxs-lookup"><span data-stu-id="ffe43-113">String</span></span>|<span data-ttu-id="ffe43-p101">コンテンツの種類。可能な値は、`text` と `HTML` です。</span><span class="sxs-lookup"><span data-stu-id="ffe43-p101">The type of the content. Possible values are `text` and `HTML`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ffe43-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ffe43-116">JSON representation</span></span>

<span data-ttu-id="ffe43-117">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="ffe43-117">Here is a JSON representation of the resource</span></span>

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
