---
title: WorksheetProtection リソースの種類
description: シート オブジェクトの保護を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5b9faed56e545698cb731728b2c95fd31682b252
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916993"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="d621a-103">WorksheetProtection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d621a-103">WorksheetProtection resource type</span></span>

> <span data-ttu-id="d621a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d621a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d621a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d621a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d621a-106">シート オブジェクトの保護を表します。</span><span class="sxs-lookup"><span data-stu-id="d621a-106">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="d621a-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="d621a-107">Methods</span></span>

| <span data-ttu-id="d621a-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="d621a-108">Method</span></span>           | <span data-ttu-id="d621a-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d621a-109">Return Type</span></span>    |<span data-ttu-id="d621a-110">説明</span><span class="sxs-lookup"><span data-stu-id="d621a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d621a-111">WorksheetProtection を取得する</span><span class="sxs-lookup"><span data-stu-id="d621a-111">Get WorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="d621a-112">WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="d621a-112">WorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="d621a-113">worksheetProtection オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d621a-113">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="d621a-114">Protect</span><span class="sxs-lookup"><span data-stu-id="d621a-114">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="d621a-115">なし</span><span class="sxs-lookup"><span data-stu-id="d621a-115">None</span></span>|<span data-ttu-id="d621a-p102">ワークシートを保護します。ワークシートが保護されている場合はスローします。</span><span class="sxs-lookup"><span data-stu-id="d621a-p102">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="d621a-118">Unprotect</span><span class="sxs-lookup"><span data-stu-id="d621a-118">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="d621a-119">なし</span><span class="sxs-lookup"><span data-stu-id="d621a-119">None</span></span>|<span data-ttu-id="d621a-120">ワークシートの保護を解除します。</span><span class="sxs-lookup"><span data-stu-id="d621a-120">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="d621a-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d621a-121">Properties</span></span>
| <span data-ttu-id="d621a-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d621a-122">Property</span></span>     | <span data-ttu-id="d621a-123">種類</span><span class="sxs-lookup"><span data-stu-id="d621a-123">Type</span></span>   |<span data-ttu-id="d621a-124">説明</span><span class="sxs-lookup"><span data-stu-id="d621a-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d621a-125">protected</span><span class="sxs-lookup"><span data-stu-id="d621a-125">protected</span></span>|<span data-ttu-id="d621a-126">ブール値</span><span class="sxs-lookup"><span data-stu-id="d621a-126">boolean</span></span>|<span data-ttu-id="d621a-p103">ワークシートが保護されているかどうかを示します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d621a-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d621a-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d621a-129">Relationships</span></span>
| <span data-ttu-id="d621a-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d621a-130">Relationship</span></span> | <span data-ttu-id="d621a-131">型</span><span class="sxs-lookup"><span data-stu-id="d621a-131">Type</span></span>   |<span data-ttu-id="d621a-132">説明</span><span class="sxs-lookup"><span data-stu-id="d621a-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d621a-133">options</span><span class="sxs-lookup"><span data-stu-id="d621a-133">options</span></span>|[<span data-ttu-id="d621a-134">WorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="d621a-134">WorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="d621a-p104">シートの保護のオプション。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="d621a-p104">Sheet protection options. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d621a-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d621a-137">JSON representation</span></span>

<span data-ttu-id="d621a-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d621a-138">Here is a JSON representation of the resource.</span></span>

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
