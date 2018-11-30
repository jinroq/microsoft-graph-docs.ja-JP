---
title: WorksheetProtection リソースの種類
description: シート オブジェクトの保護を表します。
ms.openlocfilehash: 8886117df669201a0c8a6f9fda1df18bb47cc4a4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073768"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="c4649-103">WorksheetProtection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c4649-103">WorksheetProtection resource type</span></span>

> <span data-ttu-id="c4649-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c4649-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c4649-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c4649-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c4649-106">シート オブジェクトの保護を表します。</span><span class="sxs-lookup"><span data-stu-id="c4649-106">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="c4649-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="c4649-107">Methods</span></span>

| <span data-ttu-id="c4649-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="c4649-108">Method</span></span>           | <span data-ttu-id="c4649-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c4649-109">Return Type</span></span>    |<span data-ttu-id="c4649-110">説明</span><span class="sxs-lookup"><span data-stu-id="c4649-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c4649-111">WorksheetProtection を取得する</span><span class="sxs-lookup"><span data-stu-id="c4649-111">Get WorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="c4649-112">WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="c4649-112">WorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="c4649-113">worksheetProtection オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c4649-113">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="c4649-114">Protect</span><span class="sxs-lookup"><span data-stu-id="c4649-114">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="c4649-115">なし</span><span class="sxs-lookup"><span data-stu-id="c4649-115">None</span></span>|<span data-ttu-id="c4649-p102">ワークシートを保護します。ワークシートが保護されている場合はスローします。</span><span class="sxs-lookup"><span data-stu-id="c4649-p102">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="c4649-118">Unprotect</span><span class="sxs-lookup"><span data-stu-id="c4649-118">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="c4649-119">なし</span><span class="sxs-lookup"><span data-stu-id="c4649-119">None</span></span>|<span data-ttu-id="c4649-120">ワークシートの保護を解除します。</span><span class="sxs-lookup"><span data-stu-id="c4649-120">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="c4649-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c4649-121">Properties</span></span>
| <span data-ttu-id="c4649-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c4649-122">Property</span></span>     | <span data-ttu-id="c4649-123">型</span><span class="sxs-lookup"><span data-stu-id="c4649-123">Type</span></span>   |<span data-ttu-id="c4649-124">説明</span><span class="sxs-lookup"><span data-stu-id="c4649-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c4649-125">protected</span><span class="sxs-lookup"><span data-stu-id="c4649-125">protected</span></span>|<span data-ttu-id="c4649-126">ブール値</span><span class="sxs-lookup"><span data-stu-id="c4649-126">boolean</span></span>|<span data-ttu-id="c4649-p103">ワークシートが保護されているかどうかを示します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c4649-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c4649-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c4649-129">Relationships</span></span>
| <span data-ttu-id="c4649-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c4649-130">Relationship</span></span> | <span data-ttu-id="c4649-131">型</span><span class="sxs-lookup"><span data-stu-id="c4649-131">Type</span></span>   |<span data-ttu-id="c4649-132">説明</span><span class="sxs-lookup"><span data-stu-id="c4649-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c4649-133">options</span><span class="sxs-lookup"><span data-stu-id="c4649-133">options</span></span>|[<span data-ttu-id="c4649-134">WorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="c4649-134">WorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="c4649-p104">シートの保護のオプション。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="c4649-p104">Sheet protection options. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c4649-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c4649-137">JSON representation</span></span>

<span data-ttu-id="c4649-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c4649-138">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->