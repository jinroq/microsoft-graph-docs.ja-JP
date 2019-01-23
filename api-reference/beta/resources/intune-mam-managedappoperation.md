---
title: managedAppOperation リソースの種類
description: アプリ登録に対して適用される操作を表します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cb72c4bf8cf7f2a4a55790087c3d46746c46a84a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424659"
---
# <a name="managedappoperation-resource-type"></a><span data-ttu-id="e0093-103">managedAppOperation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e0093-103">managedAppOperation resource type</span></span>

> <span data-ttu-id="e0093-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e0093-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e0093-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e0093-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e0093-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e0093-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0093-107">アプリ登録に対して適用される操作を表します。</span><span class="sxs-lookup"><span data-stu-id="e0093-107">Represents an operation applied against an app registration.</span></span>

## <a name="methods"></a><span data-ttu-id="e0093-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="e0093-108">Methods</span></span>
|<span data-ttu-id="e0093-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="e0093-109">Method</span></span>|<span data-ttu-id="e0093-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e0093-110">Return Type</span></span>|<span data-ttu-id="e0093-111">説明</span><span class="sxs-lookup"><span data-stu-id="e0093-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e0093-112">List managedAppOperations</span><span class="sxs-lookup"><span data-stu-id="e0093-112">List managedAppOperations</span></span>](../api/intune-mam-managedappoperation-list.md)|<span data-ttu-id="e0093-113">[managedAppOperation](../resources/intune-mam-managedappoperation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e0093-113">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="e0093-114">[managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="e0093-114">List properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) objects.</span></span>|
|[<span data-ttu-id="e0093-115">Get managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="e0093-115">Get managedAppOperation</span></span>](../api/intune-mam-managedappoperation-get.md)|[<span data-ttu-id="e0093-116">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="e0093-116">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="e0093-117">[managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e0093-117">Read properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="e0093-118">Create managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="e0093-118">Create managedAppOperation</span></span>](../api/intune-mam-managedappoperation-create.md)|[<span data-ttu-id="e0093-119">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="e0093-119">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="e0093-120">新しい [managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e0093-120">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="e0093-121">Delete managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="e0093-121">Delete managedAppOperation</span></span>](../api/intune-mam-managedappoperation-delete.md)|<span data-ttu-id="e0093-122">なし</span><span class="sxs-lookup"><span data-stu-id="e0093-122">None</span></span>|<span data-ttu-id="e0093-123">[managedAppOperation](../resources/intune-mam-managedappoperation.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="e0093-123">Deletes a [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span></span>|
|[<span data-ttu-id="e0093-124">Update managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="e0093-124">Update managedAppOperation</span></span>](../api/intune-mam-managedappoperation-update.md)|[<span data-ttu-id="e0093-125">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="e0093-125">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="e0093-126">[managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e0093-126">Update the properties of a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e0093-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e0093-127">Properties</span></span>
|<span data-ttu-id="e0093-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e0093-128">Property</span></span>|<span data-ttu-id="e0093-129">型</span><span class="sxs-lookup"><span data-stu-id="e0093-129">Type</span></span>|<span data-ttu-id="e0093-130">説明</span><span class="sxs-lookup"><span data-stu-id="e0093-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0093-131">displayName</span><span class="sxs-lookup"><span data-stu-id="e0093-131">displayName</span></span>|<span data-ttu-id="e0093-132">String</span><span class="sxs-lookup"><span data-stu-id="e0093-132">String</span></span>|<span data-ttu-id="e0093-133">操作名。</span><span class="sxs-lookup"><span data-stu-id="e0093-133">The operation name.</span></span>|
|<span data-ttu-id="e0093-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e0093-134">lastModifiedDateTime</span></span>|<span data-ttu-id="e0093-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0093-135">DateTimeOffset</span></span>|<span data-ttu-id="e0093-136">アプリ操作が変更された最終時刻。</span><span class="sxs-lookup"><span data-stu-id="e0093-136">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="e0093-137">state</span><span class="sxs-lookup"><span data-stu-id="e0093-137">state</span></span>|<span data-ttu-id="e0093-138">String</span><span class="sxs-lookup"><span data-stu-id="e0093-138">String</span></span>|<span data-ttu-id="e0093-139">操作の現在の状態。</span><span class="sxs-lookup"><span data-stu-id="e0093-139">The current state of the operation</span></span>|
|<span data-ttu-id="e0093-140">id</span><span class="sxs-lookup"><span data-stu-id="e0093-140">id</span></span>|<span data-ttu-id="e0093-141">String</span><span class="sxs-lookup"><span data-stu-id="e0093-141">String</span></span>|<span data-ttu-id="e0093-142">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e0093-142">Key of the entity.</span></span>|
|<span data-ttu-id="e0093-143">version</span><span class="sxs-lookup"><span data-stu-id="e0093-143">version</span></span>|<span data-ttu-id="e0093-144">String</span><span class="sxs-lookup"><span data-stu-id="e0093-144">String</span></span>|<span data-ttu-id="e0093-145">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="e0093-145">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0093-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e0093-146">Relationships</span></span>
<span data-ttu-id="e0093-147">なし</span><span class="sxs-lookup"><span data-stu-id="e0093-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e0093-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e0093-148">JSON Representation</span></span>
<span data-ttu-id="e0093-149">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e0093-149">Here is a JSON representation of the resource.</span></span>
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




