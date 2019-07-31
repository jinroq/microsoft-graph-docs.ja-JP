---
title: taxAreas リソースの種類
description: 税金エリア
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 09c1c51fed961489d824136f28aaa2f5b3859b44
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972895"
---
# <a name="taxareas-resource-type"></a><span data-ttu-id="70c10-103">taxAreas リソースの種類</span><span class="sxs-lookup"><span data-stu-id="70c10-103">taxAreas resource type</span></span>
<span data-ttu-id="70c10-104">Dynamics 365 Business Central の税エリアリソースの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="70c10-104">Represents a tax area resource type in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="70c10-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="70c10-105">Methods</span></span>
| <span data-ttu-id="70c10-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="70c10-106">Method</span></span>       | <span data-ttu-id="70c10-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="70c10-107">Return Type</span></span>  |<span data-ttu-id="70c10-108">説明</span><span class="sxs-lookup"><span data-stu-id="70c10-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="70c10-109">TaxAreas を取得する</span><span class="sxs-lookup"><span data-stu-id="70c10-109">Get taxAreas</span></span>](../api/dynamics-taxarea-get.md)|<span data-ttu-id="70c10-110">taxAreas</span><span class="sxs-lookup"><span data-stu-id="70c10-110">taxAreas</span></span>|<span data-ttu-id="70c10-111">税エリアオブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="70c10-111">Gets a tax area object.</span></span>|
|[<span data-ttu-id="70c10-112">Post taxAreas</span><span class="sxs-lookup"><span data-stu-id="70c10-112">Post taxAreas</span></span>](../api/dynamics-create-taxarea.md)|<span data-ttu-id="70c10-113">taxAreas</span><span class="sxs-lookup"><span data-stu-id="70c10-113">taxAreas</span></span>|<span data-ttu-id="70c10-114">Tax area オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="70c10-114">Creates a tax area object.</span></span>|
|[<span data-ttu-id="70c10-115">Patch taxAreas</span><span class="sxs-lookup"><span data-stu-id="70c10-115">Patch taxAreas</span></span>](../api/dynamics-taxarea-update.md)|<span data-ttu-id="70c10-116">taxAreas</span><span class="sxs-lookup"><span data-stu-id="70c10-116">taxAreas</span></span>|<span data-ttu-id="70c10-117">Tax area オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="70c10-117">Updates a tax area object.</span></span>|
|[<span data-ttu-id="70c10-118">TaxAreas の削除</span><span class="sxs-lookup"><span data-stu-id="70c10-118">Delete taxAreas</span></span>](../api/dynamics-taxarea-delete.md)|<span data-ttu-id="70c10-119">none</span><span class="sxs-lookup"><span data-stu-id="70c10-119">none</span></span>|<span data-ttu-id="70c10-120">Tax area オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="70c10-120">Deletes a tax area object.</span></span>|

## <a name="properties"></a><span data-ttu-id="70c10-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="70c10-121">Properties</span></span>
| <span data-ttu-id="70c10-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="70c10-122">Property</span></span>     | <span data-ttu-id="70c10-123">型</span><span class="sxs-lookup"><span data-stu-id="70c10-123">Type</span></span>   |<span data-ttu-id="70c10-124">説明</span><span class="sxs-lookup"><span data-stu-id="70c10-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="70c10-125">id</span><span class="sxs-lookup"><span data-stu-id="70c10-125">id</span></span>|<span data-ttu-id="70c10-126">GUID</span><span class="sxs-lookup"><span data-stu-id="70c10-126">GUID</span></span>|<span data-ttu-id="70c10-127">税エリアの一意の ID です。</span><span class="sxs-lookup"><span data-stu-id="70c10-127">The unique ID of the tax area.</span></span> <span data-ttu-id="70c10-128">編集できません。</span><span class="sxs-lookup"><span data-stu-id="70c10-128">Non-editable.</span></span>|
|<span data-ttu-id="70c10-129">code</span><span class="sxs-lookup"><span data-stu-id="70c10-129">code</span></span>|<span data-ttu-id="70c10-130">文字列、最大サイズ20</span><span class="sxs-lookup"><span data-stu-id="70c10-130">string, maximum size 20</span></span>| <span data-ttu-id="70c10-131">税エリアのコード。</span><span class="sxs-lookup"><span data-stu-id="70c10-131">The code of the tax area.</span></span>|
|<span data-ttu-id="70c10-132">displayName</span><span class="sxs-lookup"><span data-stu-id="70c10-132">displayName</span></span>|<span data-ttu-id="70c10-133">文字列、最大サイズ50</span><span class="sxs-lookup"><span data-stu-id="70c10-133">string, maximum size 50</span></span>| <span data-ttu-id="70c10-134">税エリアの表示名。</span><span class="sxs-lookup"><span data-stu-id="70c10-134">The display name of the tax area.</span></span>|
|<span data-ttu-id="70c10-135">taxType</span><span class="sxs-lookup"><span data-stu-id="70c10-135">taxType</span></span>|<span data-ttu-id="70c10-136">string</span><span class="sxs-lookup"><span data-stu-id="70c10-136">string</span></span>|<span data-ttu-id="70c10-137">税エリアの税タイプ。</span><span class="sxs-lookup"><span data-stu-id="70c10-137">The tax type of the tax area.</span></span>|
|<span data-ttu-id="70c10-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="70c10-138">lastModifiedDateTime</span></span>|<span data-ttu-id="70c10-139">datetime</span><span class="sxs-lookup"><span data-stu-id="70c10-139">datetime</span></span>|<span data-ttu-id="70c10-140">税エリアが変更された最後の datetime。</span><span class="sxs-lookup"><span data-stu-id="70c10-140">The last datetime the tax area was modified.</span></span> <span data-ttu-id="70c10-141">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="70c10-141">Read-Only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="70c10-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="70c10-142">Relationships</span></span>

## <a name="json-representation"></a><span data-ttu-id="70c10-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="70c10-143">JSON representation</span></span>

<span data-ttu-id="70c10-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="70c10-144">Here is a JSON representation of the resource.</span></span>


```json
{
  "id": "GUID",
  "code": "String",
  "displayName": "String",
  "taxType": "String",
  "lastModifiedDateTime": "datetime"
}
```


