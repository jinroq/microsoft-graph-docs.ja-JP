---
title: resourceReference リソースの種類
description: 複合型のプロパティ情報にはが含まれています。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 8cc7e686aebd531a25b6c1637fcf99338df09396
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572298"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="650ff-103">resourceReference リソースの種類</span><span class="sxs-lookup"><span data-stu-id="650ff-103">resourceReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="650ff-104">複合型のプロパティ[情報](insights.md)にはが含まれています。</span><span class="sxs-lookup"><span data-stu-id="650ff-104">Complex type containing properties of [insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="650ff-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="650ff-105">JSON representation</span></span>

<span data-ttu-id="650ff-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="650ff-106">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "singleValueLegacyExtendedProperty",
    "multiValueLegacyExtendedProperty"
  ],
  "@odata.type": "microsoft.graph.resourceReference"
}-->
```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a><span data-ttu-id="650ff-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="650ff-107">Properties</span></span>

| <span data-ttu-id="650ff-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="650ff-108">Property</span></span>      | <span data-ttu-id="650ff-109">型</span><span class="sxs-lookup"><span data-stu-id="650ff-109">Type</span></span>      | <span data-ttu-id="650ff-110">説明</span><span class="sxs-lookup"><span data-stu-id="650ff-110">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="650ff-111">webUrl</span><span class="sxs-lookup"><span data-stu-id="650ff-111">webUrl</span></span>        | <span data-ttu-id="650ff-112">String</span><span class="sxs-lookup"><span data-stu-id="650ff-112">String</span></span>    | <span data-ttu-id="650ff-113">参照先の項目に先行する URL です。</span><span class="sxs-lookup"><span data-stu-id="650ff-113">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="650ff-114">id</span><span class="sxs-lookup"><span data-stu-id="650ff-114">id</span></span>            | <span data-ttu-id="650ff-115">String</span><span class="sxs-lookup"><span data-stu-id="650ff-115">String</span></span>    | <span data-ttu-id="650ff-116">アイテムの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="650ff-116">The item's unique identifier.</span></span>           |
| <span data-ttu-id="650ff-117">type</span><span class="sxs-lookup"><span data-stu-id="650ff-117">type</span></span>          | <span data-ttu-id="650ff-118">String</span><span class="sxs-lookup"><span data-stu-id="650ff-118">String</span></span>    | <span data-ttu-id="650ff-119">文字列値"microsoft.graph.driveItem"など、アイテムの分類に使用できます。</span><span class="sxs-lookup"><span data-stu-id="650ff-119">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-resourcereference.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
