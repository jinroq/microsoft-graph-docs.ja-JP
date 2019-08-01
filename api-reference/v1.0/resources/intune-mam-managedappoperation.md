---
title: managedAppOperation リソースの種類
description: アプリ登録に対して適用される操作を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6653836cf21f4552e64bc433934a10b717be3708
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36038025"
---
# <a name="managedappoperation-resource-type"></a><span data-ttu-id="d1e02-103">managedAppOperation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d1e02-103">managedAppOperation resource type</span></span>

> <span data-ttu-id="d1e02-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d1e02-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1e02-105">アプリ登録に対して適用される操作を表します。</span><span class="sxs-lookup"><span data-stu-id="d1e02-105">Represents an operation applied against an app registration.</span></span>

## <a name="methods"></a><span data-ttu-id="d1e02-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="d1e02-106">Methods</span></span>
|<span data-ttu-id="d1e02-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="d1e02-107">Method</span></span>|<span data-ttu-id="d1e02-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d1e02-108">Return Type</span></span>|<span data-ttu-id="d1e02-109">説明</span><span class="sxs-lookup"><span data-stu-id="d1e02-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d1e02-110">List managedAppOperations</span><span class="sxs-lookup"><span data-stu-id="d1e02-110">List managedAppOperations</span></span>](../api/intune-mam-managedappoperation-list.md)|<span data-ttu-id="d1e02-111">[managedAppOperation](../resources/intune-mam-managedappoperation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d1e02-111">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="d1e02-112">[managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="d1e02-112">List properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) objects.</span></span>|
|[<span data-ttu-id="d1e02-113">Get managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="d1e02-113">Get managedAppOperation</span></span>](../api/intune-mam-managedappoperation-get.md)|[<span data-ttu-id="d1e02-114">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="d1e02-114">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="d1e02-115">[managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d1e02-115">Read properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="d1e02-116">Create managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="d1e02-116">Create managedAppOperation</span></span>](../api/intune-mam-managedappoperation-create.md)|[<span data-ttu-id="d1e02-117">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="d1e02-117">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="d1e02-118">新しい [managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d1e02-118">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="d1e02-119">Delete managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="d1e02-119">Delete managedAppOperation</span></span>](../api/intune-mam-managedappoperation-delete.md)|<span data-ttu-id="d1e02-120">なし</span><span class="sxs-lookup"><span data-stu-id="d1e02-120">None</span></span>|<span data-ttu-id="d1e02-121">[managedAppOperation](../resources/intune-mam-managedappoperation.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="d1e02-121">Deletes a [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span></span>|
|[<span data-ttu-id="d1e02-122">Update managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="d1e02-122">Update managedAppOperation</span></span>](../api/intune-mam-managedappoperation-update.md)|[<span data-ttu-id="d1e02-123">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="d1e02-123">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="d1e02-124">[managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d1e02-124">Update the properties of a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d1e02-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d1e02-125">Properties</span></span>
|<span data-ttu-id="d1e02-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d1e02-126">Property</span></span>|<span data-ttu-id="d1e02-127">型</span><span class="sxs-lookup"><span data-stu-id="d1e02-127">Type</span></span>|<span data-ttu-id="d1e02-128">説明</span><span class="sxs-lookup"><span data-stu-id="d1e02-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1e02-129">displayName</span><span class="sxs-lookup"><span data-stu-id="d1e02-129">displayName</span></span>|<span data-ttu-id="d1e02-130">String</span><span class="sxs-lookup"><span data-stu-id="d1e02-130">String</span></span>|<span data-ttu-id="d1e02-131">操作名。</span><span class="sxs-lookup"><span data-stu-id="d1e02-131">The operation name.</span></span>|
|<span data-ttu-id="d1e02-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d1e02-132">lastModifiedDateTime</span></span>|<span data-ttu-id="d1e02-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1e02-133">DateTimeOffset</span></span>|<span data-ttu-id="d1e02-134">アプリ操作が変更された最終時刻。</span><span class="sxs-lookup"><span data-stu-id="d1e02-134">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="d1e02-135">state</span><span class="sxs-lookup"><span data-stu-id="d1e02-135">state</span></span>|<span data-ttu-id="d1e02-136">String</span><span class="sxs-lookup"><span data-stu-id="d1e02-136">String</span></span>|<span data-ttu-id="d1e02-137">操作の現在の状態。</span><span class="sxs-lookup"><span data-stu-id="d1e02-137">The current state of the operation</span></span>|
|<span data-ttu-id="d1e02-138">id</span><span class="sxs-lookup"><span data-stu-id="d1e02-138">id</span></span>|<span data-ttu-id="d1e02-139">文字列</span><span class="sxs-lookup"><span data-stu-id="d1e02-139">String</span></span>|<span data-ttu-id="d1e02-140">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d1e02-140">Key of the entity.</span></span>|
|<span data-ttu-id="d1e02-141">version</span><span class="sxs-lookup"><span data-stu-id="d1e02-141">version</span></span>|<span data-ttu-id="d1e02-142">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="d1e02-142">String</span></span>|<span data-ttu-id="d1e02-143">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="d1e02-143">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1e02-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d1e02-144">Relationships</span></span>
<span data-ttu-id="d1e02-145">なし</span><span class="sxs-lookup"><span data-stu-id="d1e02-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1e02-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d1e02-146">JSON Representation</span></span>
<span data-ttu-id="d1e02-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d1e02-147">Here is a JSON representation of the resource.</span></span>
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



