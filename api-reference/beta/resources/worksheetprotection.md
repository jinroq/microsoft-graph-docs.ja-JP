---
title: WorksheetProtection リソースの種類
description: シート オブジェクトの保護を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 7e87edcebae95f32ce0bccaf849a7d21140f4878
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29639945"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="a4473-103">WorksheetProtection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a4473-103">WorksheetProtection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4473-104">シート オブジェクトの保護を表します。</span><span class="sxs-lookup"><span data-stu-id="a4473-104">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="a4473-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="a4473-105">Methods</span></span>

| <span data-ttu-id="a4473-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="a4473-106">Method</span></span>           | <span data-ttu-id="a4473-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a4473-107">Return Type</span></span>    |<span data-ttu-id="a4473-108">説明</span><span class="sxs-lookup"><span data-stu-id="a4473-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a4473-109">WorksheetProtection を取得する</span><span class="sxs-lookup"><span data-stu-id="a4473-109">Get WorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="a4473-110">WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="a4473-110">WorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="a4473-111">worksheetProtection オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a4473-111">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="a4473-112">Protect</span><span class="sxs-lookup"><span data-stu-id="a4473-112">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="a4473-113">なし</span><span class="sxs-lookup"><span data-stu-id="a4473-113">None</span></span>|<span data-ttu-id="a4473-p101">ワークシートを保護します。ワークシートが保護されている場合はスローします。</span><span class="sxs-lookup"><span data-stu-id="a4473-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="a4473-116">Unprotect</span><span class="sxs-lookup"><span data-stu-id="a4473-116">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="a4473-117">なし</span><span class="sxs-lookup"><span data-stu-id="a4473-117">None</span></span>|<span data-ttu-id="a4473-118">ワークシートの保護を解除します。</span><span class="sxs-lookup"><span data-stu-id="a4473-118">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="a4473-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4473-119">Properties</span></span>
| <span data-ttu-id="a4473-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4473-120">Property</span></span>     | <span data-ttu-id="a4473-121">型</span><span class="sxs-lookup"><span data-stu-id="a4473-121">Type</span></span>   |<span data-ttu-id="a4473-122">説明</span><span class="sxs-lookup"><span data-stu-id="a4473-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4473-123">protected</span><span class="sxs-lookup"><span data-stu-id="a4473-123">protected</span></span>|<span data-ttu-id="a4473-124">ブール値</span><span class="sxs-lookup"><span data-stu-id="a4473-124">boolean</span></span>|<span data-ttu-id="a4473-p102">ワークシートが保護されているかどうかを示します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a4473-p102">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4473-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a4473-127">Relationships</span></span>
| <span data-ttu-id="a4473-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a4473-128">Relationship</span></span> | <span data-ttu-id="a4473-129">型</span><span class="sxs-lookup"><span data-stu-id="a4473-129">Type</span></span>   |<span data-ttu-id="a4473-130">説明</span><span class="sxs-lookup"><span data-stu-id="a4473-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4473-131">options</span><span class="sxs-lookup"><span data-stu-id="a4473-131">options</span></span>|[<span data-ttu-id="a4473-132">WorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="a4473-132">WorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="a4473-p103">シートの保護のオプション。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="a4473-p103">Sheet protection options. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a4473-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a4473-135">JSON representation</span></span>

<span data-ttu-id="a4473-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a4473-136">Here is a JSON representation of the resource.</span></span>

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
