---
title: resourceReference リソースの種類
description: 複合型のプロパティ情報にはが含まれています。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 4fa4563904472fad9fc28fa4acb10b77887b5872
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520005"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="28f5d-103">resourceReference リソースの種類</span><span class="sxs-lookup"><span data-stu-id="28f5d-103">resourceReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28f5d-104">複合型のプロパティ[情報](insights.md)にはが含まれています。</span><span class="sxs-lookup"><span data-stu-id="28f5d-104">Complex type containing properties of [Insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="28f5d-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="28f5d-105">JSON representation</span></span>

<span data-ttu-id="28f5d-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="28f5d-106">Here is a JSON representation of the resource</span></span>

```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a><span data-ttu-id="28f5d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="28f5d-107">Properties</span></span>

| <span data-ttu-id="28f5d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="28f5d-108">Property</span></span>      | <span data-ttu-id="28f5d-109">型</span><span class="sxs-lookup"><span data-stu-id="28f5d-109">Type</span></span>      | <span data-ttu-id="28f5d-110">説明</span><span class="sxs-lookup"><span data-stu-id="28f5d-110">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="28f5d-111">webUrl</span><span class="sxs-lookup"><span data-stu-id="28f5d-111">webUrl</span></span>        | <span data-ttu-id="28f5d-112">String</span><span class="sxs-lookup"><span data-stu-id="28f5d-112">String</span></span>    | <span data-ttu-id="28f5d-113">参照先の項目に先行する URL です。</span><span class="sxs-lookup"><span data-stu-id="28f5d-113">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="28f5d-114">id</span><span class="sxs-lookup"><span data-stu-id="28f5d-114">id</span></span>            | <span data-ttu-id="28f5d-115">String</span><span class="sxs-lookup"><span data-stu-id="28f5d-115">String</span></span>    | <span data-ttu-id="28f5d-116">アイテムの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="28f5d-116">The item's unique identifier.</span></span>           |
| <span data-ttu-id="28f5d-117">type</span><span class="sxs-lookup"><span data-stu-id="28f5d-117">type</span></span>          | <span data-ttu-id="28f5d-118">String</span><span class="sxs-lookup"><span data-stu-id="28f5d-118">String</span></span>    | <span data-ttu-id="28f5d-119">文字列値"microsoft.graph.driveItem"など、アイテムの分類に使用できます。</span><span class="sxs-lookup"><span data-stu-id="28f5d-119">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-resourcereference.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
