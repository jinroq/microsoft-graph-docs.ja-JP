---
title: managedAppOperation リソースの種類
description: アプリ登録に対して適用される操作を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fe7416c5357b83bd9dc7eb82d94aae6a6d740667
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465217"
---
# <a name="managedappoperation-resource-type"></a><span data-ttu-id="7a0b2-103">managedAppOperation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7a0b2-103">managedAppOperation resource type</span></span>

> <span data-ttu-id="7a0b2-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7a0b2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a0b2-105">アプリ登録に対して適用される操作を表します。</span><span class="sxs-lookup"><span data-stu-id="7a0b2-105">Represents an operation applied against an app registration.</span></span>

## <a name="methods"></a><span data-ttu-id="7a0b2-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="7a0b2-106">Methods</span></span>
|<span data-ttu-id="7a0b2-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="7a0b2-107">Method</span></span>|<span data-ttu-id="7a0b2-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7a0b2-108">Return Type</span></span>|<span data-ttu-id="7a0b2-109">説明</span><span class="sxs-lookup"><span data-stu-id="7a0b2-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7a0b2-110">List managedAppOperations</span><span class="sxs-lookup"><span data-stu-id="7a0b2-110">List managedAppOperations</span></span>](../api/intune-mam-managedappoperation-list.md)|<span data-ttu-id="7a0b2-111">[managedAppOperation](../resources/intune-mam-managedappoperation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7a0b2-111">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="7a0b2-112">[managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="7a0b2-112">List properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) objects.</span></span>|
|[<span data-ttu-id="7a0b2-113">Get managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="7a0b2-113">Get managedAppOperation</span></span>](../api/intune-mam-managedappoperation-get.md)|[<span data-ttu-id="7a0b2-114">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="7a0b2-114">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="7a0b2-115">[managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7a0b2-115">Read properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="7a0b2-116">Create managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="7a0b2-116">Create managedAppOperation</span></span>](../api/intune-mam-managedappoperation-create.md)|[<span data-ttu-id="7a0b2-117">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="7a0b2-117">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="7a0b2-118">新しい [managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7a0b2-118">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="7a0b2-119">Delete managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="7a0b2-119">Delete managedAppOperation</span></span>](../api/intune-mam-managedappoperation-delete.md)|<span data-ttu-id="7a0b2-120">なし</span><span class="sxs-lookup"><span data-stu-id="7a0b2-120">None</span></span>|<span data-ttu-id="7a0b2-121">[managedAppOperation](../resources/intune-mam-managedappoperation.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="7a0b2-121">Deletes a [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span></span>|
|[<span data-ttu-id="7a0b2-122">Update managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="7a0b2-122">Update managedAppOperation</span></span>](../api/intune-mam-managedappoperation-update.md)|[<span data-ttu-id="7a0b2-123">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="7a0b2-123">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="7a0b2-124">[managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7a0b2-124">Update the properties of a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7a0b2-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7a0b2-125">Properties</span></span>
|<span data-ttu-id="7a0b2-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7a0b2-126">Property</span></span>|<span data-ttu-id="7a0b2-127">型</span><span class="sxs-lookup"><span data-stu-id="7a0b2-127">Type</span></span>|<span data-ttu-id="7a0b2-128">説明</span><span class="sxs-lookup"><span data-stu-id="7a0b2-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a0b2-129">displayName</span><span class="sxs-lookup"><span data-stu-id="7a0b2-129">displayName</span></span>|<span data-ttu-id="7a0b2-130">String</span><span class="sxs-lookup"><span data-stu-id="7a0b2-130">String</span></span>|<span data-ttu-id="7a0b2-131">操作名。</span><span class="sxs-lookup"><span data-stu-id="7a0b2-131">The operation name.</span></span>|
|<span data-ttu-id="7a0b2-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7a0b2-132">lastModifiedDateTime</span></span>|<span data-ttu-id="7a0b2-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a0b2-133">DateTimeOffset</span></span>|<span data-ttu-id="7a0b2-134">アプリ操作が変更された最終時刻。</span><span class="sxs-lookup"><span data-stu-id="7a0b2-134">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="7a0b2-135">state</span><span class="sxs-lookup"><span data-stu-id="7a0b2-135">state</span></span>|<span data-ttu-id="7a0b2-136">String</span><span class="sxs-lookup"><span data-stu-id="7a0b2-136">String</span></span>|<span data-ttu-id="7a0b2-137">操作の現在の状態。</span><span class="sxs-lookup"><span data-stu-id="7a0b2-137">The current state of the operation</span></span>|
|<span data-ttu-id="7a0b2-138">id</span><span class="sxs-lookup"><span data-stu-id="7a0b2-138">id</span></span>|<span data-ttu-id="7a0b2-139">String</span><span class="sxs-lookup"><span data-stu-id="7a0b2-139">String</span></span>|<span data-ttu-id="7a0b2-140">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7a0b2-140">Key of the entity.</span></span>|
|<span data-ttu-id="7a0b2-141">version</span><span class="sxs-lookup"><span data-stu-id="7a0b2-141">version</span></span>|<span data-ttu-id="7a0b2-142">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="7a0b2-142">String</span></span>|<span data-ttu-id="7a0b2-143">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="7a0b2-143">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a0b2-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7a0b2-144">Relationships</span></span>
<span data-ttu-id="7a0b2-145">なし</span><span class="sxs-lookup"><span data-stu-id="7a0b2-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7a0b2-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7a0b2-146">JSON Representation</span></span>
<span data-ttu-id="7a0b2-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7a0b2-147">Here is a JSON representation of the resource.</span></span>
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



