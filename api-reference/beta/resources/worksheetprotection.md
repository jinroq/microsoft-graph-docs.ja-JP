---
title: WorksheetProtection リソースの種類
description: シート オブジェクトの保護を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 7e87edcebae95f32ce0bccaf849a7d21140f4878
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512039"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="58b07-103">WorksheetProtection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="58b07-103">WorksheetProtection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58b07-104">シート オブジェクトの保護を表します。</span><span class="sxs-lookup"><span data-stu-id="58b07-104">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="58b07-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="58b07-105">Methods</span></span>

| <span data-ttu-id="58b07-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="58b07-106">Method</span></span>           | <span data-ttu-id="58b07-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="58b07-107">Return Type</span></span>    |<span data-ttu-id="58b07-108">説明</span><span class="sxs-lookup"><span data-stu-id="58b07-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58b07-109">WorksheetProtection を取得する</span><span class="sxs-lookup"><span data-stu-id="58b07-109">[Get WorksheetProtection](../api/worksheetprotection-get.md)</span></span> | <span data-ttu-id="58b07-110">WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="58b07-110">[WorksheetProtection](worksheetprotection.md)</span></span> |<span data-ttu-id="58b07-111">worksheetProtection オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="58b07-111">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="58b07-112">Protect</span><span class="sxs-lookup"><span data-stu-id="58b07-112">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="58b07-113">なし</span><span class="sxs-lookup"><span data-stu-id="58b07-113">None</span></span>|<span data-ttu-id="58b07-p101">ワークシートを保護します。ワークシートが保護されている場合はスローします。</span><span class="sxs-lookup"><span data-stu-id="58b07-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="58b07-116">Unprotect</span><span class="sxs-lookup"><span data-stu-id="58b07-116">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="58b07-117">なし</span><span class="sxs-lookup"><span data-stu-id="58b07-117">None</span></span>|<span data-ttu-id="58b07-118">ワークシートの保護を解除します。</span><span class="sxs-lookup"><span data-stu-id="58b07-118">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="58b07-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="58b07-119">Properties</span></span>
| <span data-ttu-id="58b07-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="58b07-120">Property</span></span>     | <span data-ttu-id="58b07-121">型</span><span class="sxs-lookup"><span data-stu-id="58b07-121">Type</span></span>   |<span data-ttu-id="58b07-122">説明</span><span class="sxs-lookup"><span data-stu-id="58b07-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58b07-123">protected</span><span class="sxs-lookup"><span data-stu-id="58b07-123">protected</span></span>|<span data-ttu-id="58b07-124">boolean</span><span class="sxs-lookup"><span data-stu-id="58b07-124">boolean</span></span>|<span data-ttu-id="58b07-p102">ワークシートが保護されているかどうかを示します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="58b07-p102">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="58b07-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="58b07-127">Relationships</span></span>
| <span data-ttu-id="58b07-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="58b07-128">Relationship</span></span> | <span data-ttu-id="58b07-129">型</span><span class="sxs-lookup"><span data-stu-id="58b07-129">Type</span></span>   |<span data-ttu-id="58b07-130">説明</span><span class="sxs-lookup"><span data-stu-id="58b07-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58b07-131">options</span><span class="sxs-lookup"><span data-stu-id="58b07-131">options</span></span>|[<span data-ttu-id="58b07-132">WorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="58b07-132">WorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="58b07-p103">シートの保護のオプション。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="58b07-p103">Sheet protection options. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="58b07-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="58b07-135">JSON representation</span></span>

<span data-ttu-id="58b07-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="58b07-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.worksheetProtection"
}-->

```json
{
  "protected": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "WorksheetProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/worksheetprotection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
