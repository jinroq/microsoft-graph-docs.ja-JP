---
title: resourceReference リソースの種類
description: Insights のプロパティを含む複合型。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 4fa4563904472fad9fc28fa4acb10b77887b5872
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549707"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="3d890-103">resourceReference リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3d890-103">resourceReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d890-104">[Insights](insights.md)のプロパティを含む複合型。</span><span class="sxs-lookup"><span data-stu-id="3d890-104">Complex type containing properties of [Insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d890-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3d890-105">JSON representation</span></span>

<span data-ttu-id="3d890-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="3d890-106">Here is a JSON representation of the resource</span></span>

```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a><span data-ttu-id="3d890-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3d890-107">Properties</span></span>

| <span data-ttu-id="3d890-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3d890-108">Property</span></span>      | <span data-ttu-id="3d890-109">型</span><span class="sxs-lookup"><span data-stu-id="3d890-109">Type</span></span>      | <span data-ttu-id="3d890-110">説明</span><span class="sxs-lookup"><span data-stu-id="3d890-110">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="3d890-111">webUrl</span><span class="sxs-lookup"><span data-stu-id="3d890-111">webUrl</span></span>        | <span data-ttu-id="3d890-112">String</span><span class="sxs-lookup"><span data-stu-id="3d890-112">String</span></span>    | <span data-ttu-id="3d890-113">参照されるアイテムにつながる URL。</span><span class="sxs-lookup"><span data-stu-id="3d890-113">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="3d890-114">id</span><span class="sxs-lookup"><span data-stu-id="3d890-114">id</span></span>            | <span data-ttu-id="3d890-115">String</span><span class="sxs-lookup"><span data-stu-id="3d890-115">String</span></span>    | <span data-ttu-id="3d890-116">アイテムの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="3d890-116">The item's unique identifier.</span></span>           |
| <span data-ttu-id="3d890-117">type</span><span class="sxs-lookup"><span data-stu-id="3d890-117">type</span></span>          | <span data-ttu-id="3d890-118">String</span><span class="sxs-lookup"><span data-stu-id="3d890-118">String</span></span>    | <span data-ttu-id="3d890-119">アイテムの分類に使用できる文字列値 ("microsoft....." など)</span><span class="sxs-lookup"><span data-stu-id="3d890-119">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-resourcereference.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
