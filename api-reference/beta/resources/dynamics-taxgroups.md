---
title: taxGroups リソースの種類
description: Dynamics 365 Business Central の税グループオブジェクト。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 378d8c1d773eacb3339eba35d5d60cc7ef5f2400
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006606"
---
# <a name="taxgroups-resource-type"></a><span data-ttu-id="e5173-103">taxGroups リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e5173-103">taxGroups resource type</span></span>
<span data-ttu-id="e5173-104">Dynamics 365 Business Central の taxGroups リソースの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="e5173-104">Represents a taxGroups resource type in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="e5173-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="e5173-105">Methods</span></span>
| <span data-ttu-id="e5173-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="e5173-106">Method</span></span>       | <span data-ttu-id="e5173-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e5173-107">Return Type</span></span>  |<span data-ttu-id="e5173-108">説明</span><span class="sxs-lookup"><span data-stu-id="e5173-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e5173-109">TaxGroups を取得する</span><span class="sxs-lookup"><span data-stu-id="e5173-109">Get taxGroups</span></span>](../api/dynamics-taxgroups-get.md)|<span data-ttu-id="e5173-110">taxGroups</span><span class="sxs-lookup"><span data-stu-id="e5173-110">taxGroups</span></span>|<span data-ttu-id="e5173-111">税グループオブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="e5173-111">Gets a tax group object.</span></span>|
|[<span data-ttu-id="e5173-112">Post taxGroups</span><span class="sxs-lookup"><span data-stu-id="e5173-112">Post taxGroups</span></span>](../api/dynamics-create-taxgroups.md)|<span data-ttu-id="e5173-113">taxGroups</span><span class="sxs-lookup"><span data-stu-id="e5173-113">taxGroups</span></span>|<span data-ttu-id="e5173-114">税グループオブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e5173-114">Creates a tax group object.</span></span>|
|[<span data-ttu-id="e5173-115">Patch taxGroups</span><span class="sxs-lookup"><span data-stu-id="e5173-115">Patch taxGroups</span></span>](../api/dynamics-taxgroups-update.md)|<span data-ttu-id="e5173-116">taxGroups</span><span class="sxs-lookup"><span data-stu-id="e5173-116">taxGroups</span></span>|<span data-ttu-id="e5173-117">税グループオブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="e5173-117">Updates a tax group object.</span></span>|
|[<span data-ttu-id="e5173-118">TaxGroups の削除</span><span class="sxs-lookup"><span data-stu-id="e5173-118">Delete taxGroups</span></span>](../api/dynamics-taxgroups-delete.md)|<span data-ttu-id="e5173-119">none</span><span class="sxs-lookup"><span data-stu-id="e5173-119">none</span></span>|<span data-ttu-id="e5173-120">税グループオブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="e5173-120">Deletes a tax group object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e5173-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e5173-121">Properties</span></span>
| <span data-ttu-id="e5173-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e5173-122">Property</span></span>     | <span data-ttu-id="e5173-123">型</span><span class="sxs-lookup"><span data-stu-id="e5173-123">Type</span></span>   |<span data-ttu-id="e5173-124">説明</span><span class="sxs-lookup"><span data-stu-id="e5173-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5173-125">id</span><span class="sxs-lookup"><span data-stu-id="e5173-125">id</span></span>|<span data-ttu-id="e5173-126">GUID</span><span class="sxs-lookup"><span data-stu-id="e5173-126">GUID</span></span>|<span data-ttu-id="e5173-127">TaxGroup の一意の ID。</span><span class="sxs-lookup"><span data-stu-id="e5173-127">The unique ID of the taxGroup.</span></span> <span data-ttu-id="e5173-128">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e5173-128">Read-Only.</span></span>|
|<span data-ttu-id="e5173-129">code</span><span class="sxs-lookup"><span data-stu-id="e5173-129">code</span></span>|<span data-ttu-id="e5173-130">string</span><span class="sxs-lookup"><span data-stu-id="e5173-130">string</span></span>|<span data-ttu-id="e5173-131">税グループを指定します。</span><span class="sxs-lookup"><span data-stu-id="e5173-131">Specifies the tax group.</span></span>|
|<span data-ttu-id="e5173-132">displayName</span><span class="sxs-lookup"><span data-stu-id="e5173-132">displayName</span></span>|<span data-ttu-id="e5173-133">string</span><span class="sxs-lookup"><span data-stu-id="e5173-133">string</span></span>|<span data-ttu-id="e5173-134">税グループの表示名を指定します。</span><span class="sxs-lookup"><span data-stu-id="e5173-134">Specifies the tax group display name.</span></span>|
|<span data-ttu-id="e5173-135">taxType</span><span class="sxs-lookup"><span data-stu-id="e5173-135">taxType</span></span>|<span data-ttu-id="e5173-136">string</span><span class="sxs-lookup"><span data-stu-id="e5173-136">string</span></span>|<span data-ttu-id="e5173-137">グループの税の種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="e5173-137">Specifies the tax type for the group.</span></span>|
|<span data-ttu-id="e5173-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e5173-138">lastModifiedDateTime</span></span>|<span data-ttu-id="e5173-139">datetime</span><span class="sxs-lookup"><span data-stu-id="e5173-139">datetime</span></span>|<span data-ttu-id="e5173-140">税グループが最後に変更された日付です。</span><span class="sxs-lookup"><span data-stu-id="e5173-140">The last datetime the tax group was modified.</span></span> <span data-ttu-id="e5173-141">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="e5173-141">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="e5173-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e5173-142">Relationships</span></span>
<span data-ttu-id="e5173-143">なし</span><span class="sxs-lookup"><span data-stu-id="e5173-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5173-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e5173-144">JSON representation</span></span>

<span data-ttu-id="e5173-145">TaxGroup の JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e5173-145">Here is a JSON representation of the taxGroup.</span></span>

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "taxType": "string",
  "lastModifiedDateTime": "datetime"
}

```


