---
title: taxAreas リソースの種類
description: 税金エリア
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: aeda0ca136c178355a8a8f9589eb7410399ef62a
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365452"
---
# <a name="taxareas-resource-type"></a><span data-ttu-id="bfc18-103">taxAreas リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bfc18-103">taxAreas resource type</span></span>
<span data-ttu-id="bfc18-104">Dynamics 365 Business Central の税エリアリソースの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="bfc18-104">Represents a tax area resource type in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="bfc18-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="bfc18-105">Methods</span></span>
| <span data-ttu-id="bfc18-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="bfc18-106">Method</span></span>       | <span data-ttu-id="bfc18-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bfc18-107">Return Type</span></span>  |<span data-ttu-id="bfc18-108">説明</span><span class="sxs-lookup"><span data-stu-id="bfc18-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bfc18-109">taxAreas を取得する</span><span class="sxs-lookup"><span data-stu-id="bfc18-109">Get taxAreas</span></span>](../api/dynamics-taxarea-get.md)|<span data-ttu-id="bfc18-110">taxAreas</span><span class="sxs-lookup"><span data-stu-id="bfc18-110">taxAreas</span></span>|<span data-ttu-id="bfc18-111">税エリアオブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="bfc18-111">Gets a tax area object.</span></span>|
|[<span data-ttu-id="bfc18-112">Post taxAreas</span><span class="sxs-lookup"><span data-stu-id="bfc18-112">Post taxAreas</span></span>](../api/dynamics-create-taxarea.md)|<span data-ttu-id="bfc18-113">taxAreas</span><span class="sxs-lookup"><span data-stu-id="bfc18-113">taxAreas</span></span>|<span data-ttu-id="bfc18-114">tax area オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="bfc18-114">Creates a tax area object.</span></span>|
|[<span data-ttu-id="bfc18-115">Patch taxAreas</span><span class="sxs-lookup"><span data-stu-id="bfc18-115">Patch taxAreas</span></span>](../api/dynamics-taxarea-update.md)|<span data-ttu-id="bfc18-116">taxAreas</span><span class="sxs-lookup"><span data-stu-id="bfc18-116">taxAreas</span></span>|<span data-ttu-id="bfc18-117">tax area オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="bfc18-117">Updates a tax area object.</span></span>|
|[<span data-ttu-id="bfc18-118">taxAreas の削除</span><span class="sxs-lookup"><span data-stu-id="bfc18-118">Delete taxAreas</span></span>](../api/dynamics-taxarea-delete.md)|<span data-ttu-id="bfc18-119">none</span><span class="sxs-lookup"><span data-stu-id="bfc18-119">none</span></span>|<span data-ttu-id="bfc18-120">tax area オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="bfc18-120">Deletes a tax area object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bfc18-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bfc18-121">Properties</span></span>
| <span data-ttu-id="bfc18-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bfc18-122">Property</span></span>     | <span data-ttu-id="bfc18-123">型</span><span class="sxs-lookup"><span data-stu-id="bfc18-123">Type</span></span>   |<span data-ttu-id="bfc18-124">説明</span><span class="sxs-lookup"><span data-stu-id="bfc18-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bfc18-125">ID</span><span class="sxs-lookup"><span data-stu-id="bfc18-125">id</span></span>|<span data-ttu-id="bfc18-126">GUID</span><span class="sxs-lookup"><span data-stu-id="bfc18-126">GUID</span></span>|<span data-ttu-id="bfc18-127">税エリアの一意の ID です。</span><span class="sxs-lookup"><span data-stu-id="bfc18-127">The unique ID of the tax area.</span></span> <span data-ttu-id="bfc18-128">編集不可。</span><span class="sxs-lookup"><span data-stu-id="bfc18-128">Non-editable.</span></span>|
|<span data-ttu-id="bfc18-129">code</span><span class="sxs-lookup"><span data-stu-id="bfc18-129">code</span></span>|<span data-ttu-id="bfc18-130">文字列、最大サイズ20</span><span class="sxs-lookup"><span data-stu-id="bfc18-130">string, maximum size 20</span></span>| <span data-ttu-id="bfc18-131">税エリアのコード。</span><span class="sxs-lookup"><span data-stu-id="bfc18-131">The code of the tax area.</span></span>|
|<span data-ttu-id="bfc18-132">displayName</span><span class="sxs-lookup"><span data-stu-id="bfc18-132">displayName</span></span>|<span data-ttu-id="bfc18-133">文字列、最大サイズ50</span><span class="sxs-lookup"><span data-stu-id="bfc18-133">string, maximum size 50</span></span>| <span data-ttu-id="bfc18-134">税エリアの表示名。</span><span class="sxs-lookup"><span data-stu-id="bfc18-134">The display name of the tax area.</span></span>|
|<span data-ttu-id="bfc18-135">taxType</span><span class="sxs-lookup"><span data-stu-id="bfc18-135">taxType</span></span>|<span data-ttu-id="bfc18-136">string</span><span class="sxs-lookup"><span data-stu-id="bfc18-136">string</span></span>|<span data-ttu-id="bfc18-137">税エリアの税タイプ。</span><span class="sxs-lookup"><span data-stu-id="bfc18-137">The tax type of the tax area.</span></span>|
|<span data-ttu-id="bfc18-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bfc18-138">lastModifiedDateTime</span></span>|<span data-ttu-id="bfc18-139">datetime</span><span class="sxs-lookup"><span data-stu-id="bfc18-139">datetime</span></span>|<span data-ttu-id="bfc18-140">税エリアが変更された最後の datetime。</span><span class="sxs-lookup"><span data-stu-id="bfc18-140">The last datetime the tax area was modified.</span></span> <span data-ttu-id="bfc18-141">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="bfc18-141">Read-Only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bfc18-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bfc18-142">Relationships</span></span>

## <a name="json-representation"></a><span data-ttu-id="bfc18-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bfc18-143">JSON representation</span></span>

<span data-ttu-id="bfc18-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bfc18-144">Here is a JSON representation of the resource.</span></span>


```json
{
  "id": "GUID",
  "code": "String",
  "displayName": "String",
  "taxType": "String",
  "lastModifiedDateTime": "datetime"
}
```


