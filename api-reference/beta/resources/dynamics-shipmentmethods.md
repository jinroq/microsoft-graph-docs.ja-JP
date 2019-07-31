---
title: shipmentMethods リソースの種類
description: Dynamics 365 Business Central の出荷方法。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: e8d25294b219815c8aa569c7a8c7fab7ec68830c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006613"
---
# <a name="shipmentmethods-resource-type"></a><span data-ttu-id="f8b82-103">shipmentMethods リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f8b82-103">shipmentMethods resource type</span></span>
<span data-ttu-id="f8b82-104">UPS、Fedex、DHL など、Dynamics 365 Business Central の出荷方法を表します。</span><span class="sxs-lookup"><span data-stu-id="f8b82-104">Represents a method of shipment in Dynamics 365 Business Central, such as UPS, Fedex, and DHL.</span></span>

## <a name="methods"></a><span data-ttu-id="f8b82-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="f8b82-105">Methods</span></span>

| <span data-ttu-id="f8b82-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="f8b82-106">Method</span></span>       | <span data-ttu-id="f8b82-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f8b82-107">Return Type</span></span>  |<span data-ttu-id="f8b82-108">説明</span><span class="sxs-lookup"><span data-stu-id="f8b82-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f8b82-109">ShipmentMethods を取得する</span><span class="sxs-lookup"><span data-stu-id="f8b82-109">Get shipmentMethods</span></span>](../api/dynamics-shipmentmethods-get.md)|<span data-ttu-id="f8b82-110">shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="f8b82-110">shipmentMethods</span></span>|<span data-ttu-id="f8b82-111">送付方法を取得します。</span><span class="sxs-lookup"><span data-stu-id="f8b82-111">Gets a shipment method.</span></span>|
|[<span data-ttu-id="f8b82-112">Post shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="f8b82-112">Post shipmentMethods</span></span>](../api/dynamics-create-shipmentmethods.md)|<span data-ttu-id="f8b82-113">shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="f8b82-113">shipmentMethods</span></span>|<span data-ttu-id="f8b82-114">送付方法を作成します。</span><span class="sxs-lookup"><span data-stu-id="f8b82-114">Creates a shipment method.</span></span>|
|[<span data-ttu-id="f8b82-115">Patch shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="f8b82-115">Patch shipmentMethods</span></span>](../api/dynamics-shipmentmethods-update.md)|<span data-ttu-id="f8b82-116">shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="f8b82-116">shipmentMethods</span></span>|<span data-ttu-id="f8b82-117">送付方法を更新します。</span><span class="sxs-lookup"><span data-stu-id="f8b82-117">Updates a shipment method.</span></span>|
|[<span data-ttu-id="f8b82-118">ShipmentMethods の削除</span><span class="sxs-lookup"><span data-stu-id="f8b82-118">Delete shipmentMethods</span></span>](../api/dynamics-shipmentmethods-delete.md)|<span data-ttu-id="f8b82-119">none</span><span class="sxs-lookup"><span data-stu-id="f8b82-119">none</span></span>|<span data-ttu-id="f8b82-120">送付方法を削除します。</span><span class="sxs-lookup"><span data-stu-id="f8b82-120">Deletes a shipment method.</span></span>|

## <a name="properties"></a><span data-ttu-id="f8b82-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f8b82-121">Properties</span></span>
| <span data-ttu-id="f8b82-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f8b82-122">Property</span></span>     | <span data-ttu-id="f8b82-123">型</span><span class="sxs-lookup"><span data-stu-id="f8b82-123">Type</span></span>   |<span data-ttu-id="f8b82-124">説明</span><span class="sxs-lookup"><span data-stu-id="f8b82-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f8b82-125">id</span><span class="sxs-lookup"><span data-stu-id="f8b82-125">id</span></span>|<span data-ttu-id="f8b82-126">GUID</span><span class="sxs-lookup"><span data-stu-id="f8b82-126">GUID</span></span>|<span data-ttu-id="f8b82-127">ShipmentMethod の一意の ID。</span><span class="sxs-lookup"><span data-stu-id="f8b82-127">The unique ID of the shipmentMethod.</span></span> <span data-ttu-id="f8b82-128">編集できません。</span><span class="sxs-lookup"><span data-stu-id="f8b82-128">Non-editable.</span></span>|
|<span data-ttu-id="f8b82-129">code</span><span class="sxs-lookup"><span data-stu-id="f8b82-129">code</span></span>|<span data-ttu-id="f8b82-130">string</span><span class="sxs-lookup"><span data-stu-id="f8b82-130">string</span></span>|<span data-ttu-id="f8b82-131">送付方法のコードを指定します。</span><span class="sxs-lookup"><span data-stu-id="f8b82-131">Specifies the shipment method code.</span></span>|
|<span data-ttu-id="f8b82-132">displayName</span><span class="sxs-lookup"><span data-stu-id="f8b82-132">displayName</span></span>|<span data-ttu-id="f8b82-133">string</span><span class="sxs-lookup"><span data-stu-id="f8b82-133">string</span></span>|<span data-ttu-id="f8b82-134">送付方法の表示名を指定します。</span><span class="sxs-lookup"><span data-stu-id="f8b82-134">Specifies the shipment method display name.</span></span>|
|<span data-ttu-id="f8b82-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f8b82-135">lastModifiedDateTime</span></span>|<span data-ttu-id="f8b82-136">datetime</span><span class="sxs-lookup"><span data-stu-id="f8b82-136">datetime</span></span>|<span data-ttu-id="f8b82-137">出荷方法が最後に変更された日付です。</span><span class="sxs-lookup"><span data-stu-id="f8b82-137">The last datetime the shipment method was modified.</span></span> <span data-ttu-id="f8b82-138">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="f8b82-138">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="f8b82-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f8b82-139">Relationships</span></span>
<span data-ttu-id="f8b82-140">なし</span><span class="sxs-lookup"><span data-stu-id="f8b82-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f8b82-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f8b82-141">JSON representation</span></span>

<span data-ttu-id="f8b82-142">ShipmentMethod の JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f8b82-142">Here is a JSON representation of the shipmentMethod.</span></span>

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}

```


