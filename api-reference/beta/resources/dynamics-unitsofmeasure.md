---
title: unitsOfMeasure リソースの種類
description: Dynamics 365 Business Central の測定単位オブジェクト。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 870e188939646594b62e6eebf3e234eb0211f140
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543029"
---
# <a name="unitsofmeasure-resource-type"></a><span data-ttu-id="6bc27-103">unitsOfMeasure リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6bc27-103">unitsOfMeasure resource type</span></span>
<span data-ttu-id="6bc27-104">Dynamics 365 Business Central の、数量の標準測定基準である測定単位を表します。</span><span class="sxs-lookup"><span data-stu-id="6bc27-104">Represents a unit of measure, which is a standard of measurement of a quantity, in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="6bc27-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="6bc27-105">Methods</span></span>

| <span data-ttu-id="6bc27-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="6bc27-106">Method</span></span>       | <span data-ttu-id="6bc27-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6bc27-107">Return Type</span></span>  |<span data-ttu-id="6bc27-108">説明</span><span class="sxs-lookup"><span data-stu-id="6bc27-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6bc27-109">unitsOfMeasure を取得する</span><span class="sxs-lookup"><span data-stu-id="6bc27-109">Get unitsOfMeasure</span></span>](../api/dynamics-unitsofmeasure-get.md)|<span data-ttu-id="6bc27-110">unitsOfMeasure</span><span class="sxs-lookup"><span data-stu-id="6bc27-110">unitsOfMeasure</span></span>|<span data-ttu-id="6bc27-111">測定単位オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="6bc27-111">Gets a unit of measure object.</span></span>|
|[<span data-ttu-id="6bc27-112">Post unitsOfMeasure</span><span class="sxs-lookup"><span data-stu-id="6bc27-112">Post unitsOfMeasure</span></span>](../api/dynamics-create-unitsofmeasure.md)|<span data-ttu-id="6bc27-113">unitsOfMeasure</span><span class="sxs-lookup"><span data-stu-id="6bc27-113">unitsOfMeasure</span></span>|<span data-ttu-id="6bc27-114">測定単位オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6bc27-114">Creates a unit of measure object.</span></span>|
|[<span data-ttu-id="6bc27-115">Patch unitsOfMeasure</span><span class="sxs-lookup"><span data-stu-id="6bc27-115">Patch unitsOfMeasure</span></span>](../api/dynamics-unitsofmeasure-update.md)|<span data-ttu-id="6bc27-116">unitsOfMeasure</span><span class="sxs-lookup"><span data-stu-id="6bc27-116">unitsOfMeasure</span></span>|<span data-ttu-id="6bc27-117">測定単位オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="6bc27-117">Updates a unit of measure object.</span></span>|
|[<span data-ttu-id="6bc27-118">unitsOfMeasure の削除</span><span class="sxs-lookup"><span data-stu-id="6bc27-118">Delete unitsOfMeasure</span></span>](../api/dynamics-unitsofmeasure-delete.md)|<span data-ttu-id="6bc27-119">なし</span><span class="sxs-lookup"><span data-stu-id="6bc27-119">none</span></span>|<span data-ttu-id="6bc27-120">測定単位オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="6bc27-120">Deletes a unit of measure object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6bc27-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6bc27-121">Properties</span></span>
| <span data-ttu-id="6bc27-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6bc27-122">Property</span></span>     | <span data-ttu-id="6bc27-123">型</span><span class="sxs-lookup"><span data-stu-id="6bc27-123">Type</span></span>   |<span data-ttu-id="6bc27-124">説明</span><span class="sxs-lookup"><span data-stu-id="6bc27-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6bc27-125">id</span><span class="sxs-lookup"><span data-stu-id="6bc27-125">id</span></span>|<span data-ttu-id="6bc27-126">GUID</span><span class="sxs-lookup"><span data-stu-id="6bc27-126">GUID</span></span>|<span data-ttu-id="6bc27-127">unitsOfMeasure の一意の ID。</span><span class="sxs-lookup"><span data-stu-id="6bc27-127">The unique ID of the unitsOfMeasure.</span></span> <span data-ttu-id="6bc27-128">編集できません。</span><span class="sxs-lookup"><span data-stu-id="6bc27-128">Non-editable.</span></span>|
|<span data-ttu-id="6bc27-129">code</span><span class="sxs-lookup"><span data-stu-id="6bc27-129">code</span></span>|<span data-ttu-id="6bc27-130">string</span><span class="sxs-lookup"><span data-stu-id="6bc27-130">string</span></span>|<span data-ttu-id="6bc27-131">測定単位のコードを指定します。</span><span class="sxs-lookup"><span data-stu-id="6bc27-131">Specifies the code for the unit of measure.</span></span>|
|<span data-ttu-id="6bc27-132">displayName</span><span class="sxs-lookup"><span data-stu-id="6bc27-132">displayName</span></span>|<span data-ttu-id="6bc27-133">string</span><span class="sxs-lookup"><span data-stu-id="6bc27-133">string</span></span>|<span data-ttu-id="6bc27-134">測定単位の表示名を指定します。</span><span class="sxs-lookup"><span data-stu-id="6bc27-134">Specifies the unit of measure's display name.</span></span>|
|<span data-ttu-id="6bc27-135">internationalStandardCode</span><span class="sxs-lookup"><span data-stu-id="6bc27-135">internationalStandardCode</span></span>|<span data-ttu-id="6bc27-136">string</span><span class="sxs-lookup"><span data-stu-id="6bc27-136">string</span></span>|<span data-ttu-id="6bc27-137">営業ドキュメントの電子送信に関連して、UNECE Rec20 standard に従って表される測定単位コードの単位を指定します。</span><span class="sxs-lookup"><span data-stu-id="6bc27-137">Specifies the unit of measure code expressed according to the UNECE Rec20 standard in connection with electronic sending of sales documents.</span></span>|
|<span data-ttu-id="6bc27-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6bc27-138">lastModifiedDateTime</span></span>|<span data-ttu-id="6bc27-139">datetime</span><span class="sxs-lookup"><span data-stu-id="6bc27-139">datetime</span></span>|<span data-ttu-id="6bc27-140">測定単位が変更された最後の datetime。</span><span class="sxs-lookup"><span data-stu-id="6bc27-140">The last datetime the unit of measure was modified.</span></span> <span data-ttu-id="6bc27-141">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="6bc27-141">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="6bc27-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6bc27-142">Relationships</span></span>
<span data-ttu-id="6bc27-143">なし</span><span class="sxs-lookup"><span data-stu-id="6bc27-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6bc27-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6bc27-144">JSON representation</span></span>

<span data-ttu-id="6bc27-145">ここでは、 **unitsOfMeasure**リソースの JSON 表記を示します。</span><span class="sxs-lookup"><span data-stu-id="6bc27-145">Here is a JSON representation of the **unitsOfMeasure** resource.</span></span>

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "internationalStandardCode": "string",
  "lastModifiedDateTime": "datetime"
}

```
