---
title: managedAppOperation リソースの種類
description: アプリ登録に対して適用される操作を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fe7416c5357b83bd9dc7eb82d94aae6a6d740667
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253471"
---
# <a name="managedappoperation-resource-type"></a><span data-ttu-id="3a02c-103">managedAppOperation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3a02c-103">managedAppOperation resource type</span></span>

> <span data-ttu-id="3a02c-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3a02c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a02c-105">アプリ登録に対して適用される操作を表します。</span><span class="sxs-lookup"><span data-stu-id="3a02c-105">Represents an operation applied against an app registration.</span></span>

## <a name="methods"></a><span data-ttu-id="3a02c-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="3a02c-106">Methods</span></span>
|<span data-ttu-id="3a02c-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="3a02c-107">Method</span></span>|<span data-ttu-id="3a02c-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3a02c-108">Return Type</span></span>|<span data-ttu-id="3a02c-109">説明</span><span class="sxs-lookup"><span data-stu-id="3a02c-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3a02c-110">List managedAppOperations</span><span class="sxs-lookup"><span data-stu-id="3a02c-110">List managedAppOperations</span></span>](../api/intune-mam-managedappoperation-list.md)|<span data-ttu-id="3a02c-111">[managedAppOperation](../resources/intune-mam-managedappoperation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="3a02c-111">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="3a02c-112">[managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="3a02c-112">List properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) objects.</span></span>|
|[<span data-ttu-id="3a02c-113">Get managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="3a02c-113">Get managedAppOperation</span></span>](../api/intune-mam-managedappoperation-get.md)|[<span data-ttu-id="3a02c-114">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="3a02c-114">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="3a02c-115">[managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="3a02c-115">Read properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="3a02c-116">Create managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="3a02c-116">Create managedAppOperation</span></span>](../api/intune-mam-managedappoperation-create.md)|[<span data-ttu-id="3a02c-117">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="3a02c-117">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="3a02c-118">新しい [managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="3a02c-118">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="3a02c-119">Delete managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="3a02c-119">Delete managedAppOperation</span></span>](../api/intune-mam-managedappoperation-delete.md)|<span data-ttu-id="3a02c-120">なし</span><span class="sxs-lookup"><span data-stu-id="3a02c-120">None</span></span>|<span data-ttu-id="3a02c-121">[managedAppOperation](../resources/intune-mam-managedappoperation.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="3a02c-121">Deletes a [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span></span>|
|[<span data-ttu-id="3a02c-122">Update managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="3a02c-122">Update managedAppOperation</span></span>](../api/intune-mam-managedappoperation-update.md)|[<span data-ttu-id="3a02c-123">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="3a02c-123">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="3a02c-124">[managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3a02c-124">Update the properties of a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3a02c-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3a02c-125">Properties</span></span>
|<span data-ttu-id="3a02c-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3a02c-126">Property</span></span>|<span data-ttu-id="3a02c-127">型</span><span class="sxs-lookup"><span data-stu-id="3a02c-127">Type</span></span>|<span data-ttu-id="3a02c-128">説明</span><span class="sxs-lookup"><span data-stu-id="3a02c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a02c-129">displayName</span><span class="sxs-lookup"><span data-stu-id="3a02c-129">displayName</span></span>|<span data-ttu-id="3a02c-130">String</span><span class="sxs-lookup"><span data-stu-id="3a02c-130">String</span></span>|<span data-ttu-id="3a02c-131">操作名。</span><span class="sxs-lookup"><span data-stu-id="3a02c-131">The operation name.</span></span>|
|<span data-ttu-id="3a02c-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3a02c-132">lastModifiedDateTime</span></span>|<span data-ttu-id="3a02c-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a02c-133">DateTimeOffset</span></span>|<span data-ttu-id="3a02c-134">アプリ操作が変更された最終時刻。</span><span class="sxs-lookup"><span data-stu-id="3a02c-134">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="3a02c-135">state</span><span class="sxs-lookup"><span data-stu-id="3a02c-135">state</span></span>|<span data-ttu-id="3a02c-136">String</span><span class="sxs-lookup"><span data-stu-id="3a02c-136">String</span></span>|<span data-ttu-id="3a02c-137">操作の現在の状態。</span><span class="sxs-lookup"><span data-stu-id="3a02c-137">The current state of the operation</span></span>|
|<span data-ttu-id="3a02c-138">id</span><span class="sxs-lookup"><span data-stu-id="3a02c-138">id</span></span>|<span data-ttu-id="3a02c-139">文字列</span><span class="sxs-lookup"><span data-stu-id="3a02c-139">String</span></span>|<span data-ttu-id="3a02c-140">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="3a02c-140">Key of the entity.</span></span>|
|<span data-ttu-id="3a02c-141">version</span><span class="sxs-lookup"><span data-stu-id="3a02c-141">version</span></span>|<span data-ttu-id="3a02c-142">String</span><span class="sxs-lookup"><span data-stu-id="3a02c-142">String</span></span>|<span data-ttu-id="3a02c-143">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="3a02c-143">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a02c-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3a02c-144">Relationships</span></span>
<span data-ttu-id="3a02c-145">なし</span><span class="sxs-lookup"><span data-stu-id="3a02c-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3a02c-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3a02c-146">JSON Representation</span></span>
<span data-ttu-id="3a02c-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3a02c-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppOperation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "state": "String",
  "id": "String (identifier)",
  "version": "String"
}
```



