---
title: taxGroups リソースの種類
description: Dynamics 365 Business Central の税グループオブジェクト。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: bdfbec8f5373637924262388dab0e9c74c363af9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543127"
---
# <a name="taxgroups-resource-type"></a><span data-ttu-id="f2609-103">taxGroups リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f2609-103">taxGroups resource type</span></span>
<span data-ttu-id="f2609-104">Dynamics 365 Business Central の taxGroups リソースの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="f2609-104">Represents a taxGroups resource type in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="f2609-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="f2609-105">Methods</span></span>
| <span data-ttu-id="f2609-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="f2609-106">Method</span></span>       | <span data-ttu-id="f2609-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f2609-107">Return Type</span></span>  |<span data-ttu-id="f2609-108">説明</span><span class="sxs-lookup"><span data-stu-id="f2609-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f2609-109">taxGroups を取得する</span><span class="sxs-lookup"><span data-stu-id="f2609-109">Get taxGroups</span></span>](../api/dynamics-taxgroups-get.md)|<span data-ttu-id="f2609-110">taxGroups</span><span class="sxs-lookup"><span data-stu-id="f2609-110">taxGroups</span></span>|<span data-ttu-id="f2609-111">税グループオブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="f2609-111">Gets a tax group object.</span></span>|
|[<span data-ttu-id="f2609-112">Post taxGroups</span><span class="sxs-lookup"><span data-stu-id="f2609-112">Post taxGroups</span></span>](../api/dynamics-create-taxgroups.md)|<span data-ttu-id="f2609-113">taxGroups</span><span class="sxs-lookup"><span data-stu-id="f2609-113">taxGroups</span></span>|<span data-ttu-id="f2609-114">税グループオブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f2609-114">Creates a tax group object.</span></span>|
|[<span data-ttu-id="f2609-115">Patch taxGroups</span><span class="sxs-lookup"><span data-stu-id="f2609-115">Patch taxGroups</span></span>](../api/dynamics-taxgroups-update.md)|<span data-ttu-id="f2609-116">taxGroups</span><span class="sxs-lookup"><span data-stu-id="f2609-116">taxGroups</span></span>|<span data-ttu-id="f2609-117">税グループオブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="f2609-117">Updates a tax group object.</span></span>|
|[<span data-ttu-id="f2609-118">taxGroups の削除</span><span class="sxs-lookup"><span data-stu-id="f2609-118">Delete taxGroups</span></span>](../api/dynamics-taxgroups-delete.md)|<span data-ttu-id="f2609-119">なし</span><span class="sxs-lookup"><span data-stu-id="f2609-119">none</span></span>|<span data-ttu-id="f2609-120">税グループオブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="f2609-120">Deletes a tax group object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f2609-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f2609-121">Properties</span></span>
| <span data-ttu-id="f2609-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f2609-122">Property</span></span>     | <span data-ttu-id="f2609-123">型</span><span class="sxs-lookup"><span data-stu-id="f2609-123">Type</span></span>   |<span data-ttu-id="f2609-124">説明</span><span class="sxs-lookup"><span data-stu-id="f2609-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2609-125">id</span><span class="sxs-lookup"><span data-stu-id="f2609-125">id</span></span>|<span data-ttu-id="f2609-126">GUID</span><span class="sxs-lookup"><span data-stu-id="f2609-126">GUID</span></span>|<span data-ttu-id="f2609-127">taxGroup の一意の ID。</span><span class="sxs-lookup"><span data-stu-id="f2609-127">The unique ID of the taxGroup.</span></span> <span data-ttu-id="f2609-128">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f2609-128">Read-Only.</span></span>|
|<span data-ttu-id="f2609-129">code</span><span class="sxs-lookup"><span data-stu-id="f2609-129">code</span></span>|<span data-ttu-id="f2609-130">string</span><span class="sxs-lookup"><span data-stu-id="f2609-130">string</span></span>|<span data-ttu-id="f2609-131">税グループを指定します。</span><span class="sxs-lookup"><span data-stu-id="f2609-131">Specifies the tax group.</span></span>|
|<span data-ttu-id="f2609-132">displayName</span><span class="sxs-lookup"><span data-stu-id="f2609-132">displayName</span></span>|<span data-ttu-id="f2609-133">string</span><span class="sxs-lookup"><span data-stu-id="f2609-133">string</span></span>|<span data-ttu-id="f2609-134">税グループの表示名を指定します。</span><span class="sxs-lookup"><span data-stu-id="f2609-134">Specifies the tax group display name.</span></span>|
|<span data-ttu-id="f2609-135">taxType</span><span class="sxs-lookup"><span data-stu-id="f2609-135">taxType</span></span>|<span data-ttu-id="f2609-136">string</span><span class="sxs-lookup"><span data-stu-id="f2609-136">string</span></span>|<span data-ttu-id="f2609-137">グループの税の種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="f2609-137">Specifies the tax type for the group.</span></span>|
|<span data-ttu-id="f2609-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f2609-138">lastModifiedDateTime</span></span>|<span data-ttu-id="f2609-139">datetime</span><span class="sxs-lookup"><span data-stu-id="f2609-139">datetime</span></span>|<span data-ttu-id="f2609-140">税グループが最後に変更された日付です。</span><span class="sxs-lookup"><span data-stu-id="f2609-140">The last datetime the tax group was modified.</span></span> <span data-ttu-id="f2609-141">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="f2609-141">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="f2609-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f2609-142">Relationships</span></span>
<span data-ttu-id="f2609-143">なし</span><span class="sxs-lookup"><span data-stu-id="f2609-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f2609-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f2609-144">JSON representation</span></span>

<span data-ttu-id="f2609-145">taxGroup の JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f2609-145">Here is a JSON representation of the taxGroup.</span></span>

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "taxType": "string",
  "lastModifiedDateTime": "datetime"
}

```


