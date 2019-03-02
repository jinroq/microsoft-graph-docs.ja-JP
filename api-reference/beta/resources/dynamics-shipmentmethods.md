---
title: shipmentMethods リソースの種類
description: Dynamics 365 Business Central の出荷方法。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 2f7ef9611fc85c13ac24c79b292e06a6bdc5d587
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365501"
---
# <a name="shipmentmethods-resource-type"></a><span data-ttu-id="2873d-103">shipmentMethods リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2873d-103">shipmentMethods resource type</span></span>
<span data-ttu-id="2873d-104">UPS、Fedex、DHL など、Dynamics 365 Business Central の出荷方法を表します。</span><span class="sxs-lookup"><span data-stu-id="2873d-104">Represents a method of shipment in Dynamics 365 Business Central, such as UPS, Fedex, and DHL.</span></span>

## <a name="methods"></a><span data-ttu-id="2873d-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="2873d-105">Methods</span></span>

| <span data-ttu-id="2873d-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="2873d-106">Method</span></span>       | <span data-ttu-id="2873d-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2873d-107">Return Type</span></span>  |<span data-ttu-id="2873d-108">説明</span><span class="sxs-lookup"><span data-stu-id="2873d-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2873d-109">shipmentMethods を取得する</span><span class="sxs-lookup"><span data-stu-id="2873d-109">Get shipmentMethods</span></span>](../api/dynamics-shipmentmethods-get.md)|<span data-ttu-id="2873d-110">shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="2873d-110">shipmentMethods</span></span>|<span data-ttu-id="2873d-111">送付方法を取得します。</span><span class="sxs-lookup"><span data-stu-id="2873d-111">Gets a shipment method.</span></span>|
|[<span data-ttu-id="2873d-112">Post shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="2873d-112">Post shipmentMethods</span></span>](../api/dynamics-create-shipmentmethods.md)|<span data-ttu-id="2873d-113">shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="2873d-113">shipmentMethods</span></span>|<span data-ttu-id="2873d-114">送付方法を作成します。</span><span class="sxs-lookup"><span data-stu-id="2873d-114">Creates a shipment method.</span></span>|
|[<span data-ttu-id="2873d-115">Patch shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="2873d-115">Patch shipmentMethods</span></span>](../api/dynamics-shipmentmethods-update.md)|<span data-ttu-id="2873d-116">shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="2873d-116">shipmentMethods</span></span>|<span data-ttu-id="2873d-117">送付方法を更新します。</span><span class="sxs-lookup"><span data-stu-id="2873d-117">Updates a shipment method.</span></span>|
|[<span data-ttu-id="2873d-118">shipmentMethods の削除</span><span class="sxs-lookup"><span data-stu-id="2873d-118">Delete shipmentMethods</span></span>](../api/dynamics-shipmentmethods-delete.md)|<span data-ttu-id="2873d-119">none</span><span class="sxs-lookup"><span data-stu-id="2873d-119">none</span></span>|<span data-ttu-id="2873d-120">送付方法を削除します。</span><span class="sxs-lookup"><span data-stu-id="2873d-120">Deletes a shipment method.</span></span>|

## <a name="properties"></a><span data-ttu-id="2873d-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2873d-121">Properties</span></span>
| <span data-ttu-id="2873d-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2873d-122">Property</span></span>     | <span data-ttu-id="2873d-123">型</span><span class="sxs-lookup"><span data-stu-id="2873d-123">Type</span></span>   |<span data-ttu-id="2873d-124">説明</span><span class="sxs-lookup"><span data-stu-id="2873d-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2873d-125">ID</span><span class="sxs-lookup"><span data-stu-id="2873d-125">id</span></span>|<span data-ttu-id="2873d-126">GUID</span><span class="sxs-lookup"><span data-stu-id="2873d-126">GUID</span></span>|<span data-ttu-id="2873d-127">shipmentMethod の一意の ID。</span><span class="sxs-lookup"><span data-stu-id="2873d-127">The unique ID of the shipmentMethod.</span></span> <span data-ttu-id="2873d-128">編集不可。</span><span class="sxs-lookup"><span data-stu-id="2873d-128">Non-editable.</span></span>|
|<span data-ttu-id="2873d-129">code</span><span class="sxs-lookup"><span data-stu-id="2873d-129">code</span></span>|<span data-ttu-id="2873d-130">文字列</span><span class="sxs-lookup"><span data-stu-id="2873d-130">string</span></span>|<span data-ttu-id="2873d-131">送付方法のコードを指定します。</span><span class="sxs-lookup"><span data-stu-id="2873d-131">Specifies the shipment method code.</span></span>|
|<span data-ttu-id="2873d-132">displayName</span><span class="sxs-lookup"><span data-stu-id="2873d-132">displayName</span></span>|<span data-ttu-id="2873d-133">string</span><span class="sxs-lookup"><span data-stu-id="2873d-133">string</span></span>|<span data-ttu-id="2873d-134">送付方法の表示名を指定します。</span><span class="sxs-lookup"><span data-stu-id="2873d-134">Specifies the shipment method display name.</span></span>|
|<span data-ttu-id="2873d-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2873d-135">lastModifiedDateTime</span></span>|<span data-ttu-id="2873d-136">datetime</span><span class="sxs-lookup"><span data-stu-id="2873d-136">datetime</span></span>|<span data-ttu-id="2873d-137">出荷方法が最後に変更された日付です。</span><span class="sxs-lookup"><span data-stu-id="2873d-137">The last datetime the shipment method was modified.</span></span> <span data-ttu-id="2873d-138">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="2873d-138">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="2873d-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2873d-139">Relationships</span></span>
<span data-ttu-id="2873d-140">なし</span><span class="sxs-lookup"><span data-stu-id="2873d-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2873d-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2873d-141">JSON representation</span></span>

<span data-ttu-id="2873d-142">shipmentMethod の JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2873d-142">Here is a JSON representation of the shipmentMethod.</span></span>

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}

```


