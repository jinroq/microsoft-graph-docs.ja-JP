---
title: taxGroups リソースの種類
description: Dynamics 365 Business Central の税グループオブジェクト。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: bdfbec8f5373637924262388dab0e9c74c363af9
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366691"
---
# <a name="taxgroups-resource-type"></a><span data-ttu-id="890f3-103">taxGroups リソースの種類</span><span class="sxs-lookup"><span data-stu-id="890f3-103">taxGroups resource type</span></span>
<span data-ttu-id="890f3-104">Dynamics 365 Business Central の taxGroups リソースの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="890f3-104">Represents a taxGroups resource type in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="890f3-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="890f3-105">Methods</span></span>
| <span data-ttu-id="890f3-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="890f3-106">Method</span></span>       | <span data-ttu-id="890f3-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="890f3-107">Return Type</span></span>  |<span data-ttu-id="890f3-108">説明</span><span class="sxs-lookup"><span data-stu-id="890f3-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="890f3-109">taxGroups を取得する</span><span class="sxs-lookup"><span data-stu-id="890f3-109">Get taxGroups</span></span>](../api/dynamics-taxgroups-get.md)|<span data-ttu-id="890f3-110">taxGroups</span><span class="sxs-lookup"><span data-stu-id="890f3-110">taxGroups</span></span>|<span data-ttu-id="890f3-111">税グループオブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="890f3-111">Gets a tax group object.</span></span>|
|[<span data-ttu-id="890f3-112">Post taxGroups</span><span class="sxs-lookup"><span data-stu-id="890f3-112">Post taxGroups</span></span>](../api/dynamics-create-taxgroups.md)|<span data-ttu-id="890f3-113">taxGroups</span><span class="sxs-lookup"><span data-stu-id="890f3-113">taxGroups</span></span>|<span data-ttu-id="890f3-114">税グループオブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="890f3-114">Creates a tax group object.</span></span>|
|[<span data-ttu-id="890f3-115">Patch taxGroups</span><span class="sxs-lookup"><span data-stu-id="890f3-115">Patch taxGroups</span></span>](../api/dynamics-taxgroups-update.md)|<span data-ttu-id="890f3-116">taxGroups</span><span class="sxs-lookup"><span data-stu-id="890f3-116">taxGroups</span></span>|<span data-ttu-id="890f3-117">税グループオブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="890f3-117">Updates a tax group object.</span></span>|
|[<span data-ttu-id="890f3-118">taxGroups の削除</span><span class="sxs-lookup"><span data-stu-id="890f3-118">Delete taxGroups</span></span>](../api/dynamics-taxgroups-delete.md)|<span data-ttu-id="890f3-119">none</span><span class="sxs-lookup"><span data-stu-id="890f3-119">none</span></span>|<span data-ttu-id="890f3-120">税グループオブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="890f3-120">Deletes a tax group object.</span></span>|

## <a name="properties"></a><span data-ttu-id="890f3-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="890f3-121">Properties</span></span>
| <span data-ttu-id="890f3-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="890f3-122">Property</span></span>     | <span data-ttu-id="890f3-123">型</span><span class="sxs-lookup"><span data-stu-id="890f3-123">Type</span></span>   |<span data-ttu-id="890f3-124">説明</span><span class="sxs-lookup"><span data-stu-id="890f3-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="890f3-125">ID</span><span class="sxs-lookup"><span data-stu-id="890f3-125">id</span></span>|<span data-ttu-id="890f3-126">GUID</span><span class="sxs-lookup"><span data-stu-id="890f3-126">GUID</span></span>|<span data-ttu-id="890f3-127">taxGroup の一意の ID。</span><span class="sxs-lookup"><span data-stu-id="890f3-127">The unique ID of the taxGroup.</span></span> <span data-ttu-id="890f3-128">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="890f3-128">Read-Only.</span></span>|
|<span data-ttu-id="890f3-129">code</span><span class="sxs-lookup"><span data-stu-id="890f3-129">code</span></span>|<span data-ttu-id="890f3-130">文字列</span><span class="sxs-lookup"><span data-stu-id="890f3-130">string</span></span>|<span data-ttu-id="890f3-131">税グループを指定します。</span><span class="sxs-lookup"><span data-stu-id="890f3-131">Specifies the tax group.</span></span>|
|<span data-ttu-id="890f3-132">displayName</span><span class="sxs-lookup"><span data-stu-id="890f3-132">displayName</span></span>|<span data-ttu-id="890f3-133">string</span><span class="sxs-lookup"><span data-stu-id="890f3-133">string</span></span>|<span data-ttu-id="890f3-134">税グループの表示名を指定します。</span><span class="sxs-lookup"><span data-stu-id="890f3-134">Specifies the tax group display name.</span></span>|
|<span data-ttu-id="890f3-135">taxType</span><span class="sxs-lookup"><span data-stu-id="890f3-135">taxType</span></span>|<span data-ttu-id="890f3-136">string</span><span class="sxs-lookup"><span data-stu-id="890f3-136">string</span></span>|<span data-ttu-id="890f3-137">グループの税の種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="890f3-137">Specifies the tax type for the group.</span></span>|
|<span data-ttu-id="890f3-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="890f3-138">lastModifiedDateTime</span></span>|<span data-ttu-id="890f3-139">datetime</span><span class="sxs-lookup"><span data-stu-id="890f3-139">datetime</span></span>|<span data-ttu-id="890f3-140">税グループが最後に変更された日付です。</span><span class="sxs-lookup"><span data-stu-id="890f3-140">The last datetime the tax group was modified.</span></span> <span data-ttu-id="890f3-141">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="890f3-141">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="890f3-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="890f3-142">Relationships</span></span>
<span data-ttu-id="890f3-143">なし</span><span class="sxs-lookup"><span data-stu-id="890f3-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="890f3-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="890f3-144">JSON representation</span></span>

<span data-ttu-id="890f3-145">taxGroup の JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="890f3-145">Here is a JSON representation of the taxGroup.</span></span>

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "taxType": "string",
  "lastModifiedDateTime": "datetime"
}

```


