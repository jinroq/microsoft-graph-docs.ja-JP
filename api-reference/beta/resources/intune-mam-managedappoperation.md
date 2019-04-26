---
title: managedAppOperation リソースの種類
description: アプリ登録に対して適用される操作を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 545cacaa5f5d4c065e681dea1604d0fa89036132
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554108"
---
# <a name="managedappoperation-resource-type"></a><span data-ttu-id="d4b99-103">managedAppOperation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d4b99-103">managedAppOperation resource type</span></span>

> <span data-ttu-id="d4b99-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d4b99-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4b99-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d4b99-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4b99-106">アプリ登録に対して適用される操作を表します。</span><span class="sxs-lookup"><span data-stu-id="d4b99-106">Represents an operation applied against an app registration.</span></span>

## <a name="methods"></a><span data-ttu-id="d4b99-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="d4b99-107">Methods</span></span>
|<span data-ttu-id="d4b99-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="d4b99-108">Method</span></span>|<span data-ttu-id="d4b99-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d4b99-109">Return Type</span></span>|<span data-ttu-id="d4b99-110">説明</span><span class="sxs-lookup"><span data-stu-id="d4b99-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d4b99-111">List managedAppOperations</span><span class="sxs-lookup"><span data-stu-id="d4b99-111">List managedAppOperations</span></span>](../api/intune-mam-managedappoperation-list.md)|<span data-ttu-id="d4b99-112">[managedAppOperation](../resources/intune-mam-managedappoperation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d4b99-112">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="d4b99-113">[managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="d4b99-113">List properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) objects.</span></span>|
|[<span data-ttu-id="d4b99-114">Get managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="d4b99-114">Get managedAppOperation</span></span>](../api/intune-mam-managedappoperation-get.md)|[<span data-ttu-id="d4b99-115">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="d4b99-115">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="d4b99-116">[managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d4b99-116">Read properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="d4b99-117">Create managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="d4b99-117">Create managedAppOperation</span></span>](../api/intune-mam-managedappoperation-create.md)|[<span data-ttu-id="d4b99-118">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="d4b99-118">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="d4b99-119">新しい [managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d4b99-119">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="d4b99-120">Delete managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="d4b99-120">Delete managedAppOperation</span></span>](../api/intune-mam-managedappoperation-delete.md)|<span data-ttu-id="d4b99-121">なし</span><span class="sxs-lookup"><span data-stu-id="d4b99-121">None</span></span>|<span data-ttu-id="d4b99-122">[managedAppOperation](../resources/intune-mam-managedappoperation.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="d4b99-122">Deletes a [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span></span>|
|[<span data-ttu-id="d4b99-123">Update managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="d4b99-123">Update managedAppOperation</span></span>](../api/intune-mam-managedappoperation-update.md)|[<span data-ttu-id="d4b99-124">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="d4b99-124">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="d4b99-125">[managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d4b99-125">Update the properties of a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d4b99-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d4b99-126">Properties</span></span>
|<span data-ttu-id="d4b99-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d4b99-127">Property</span></span>|<span data-ttu-id="d4b99-128">型</span><span class="sxs-lookup"><span data-stu-id="d4b99-128">Type</span></span>|<span data-ttu-id="d4b99-129">説明</span><span class="sxs-lookup"><span data-stu-id="d4b99-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4b99-130">displayName</span><span class="sxs-lookup"><span data-stu-id="d4b99-130">displayName</span></span>|<span data-ttu-id="d4b99-131">String</span><span class="sxs-lookup"><span data-stu-id="d4b99-131">String</span></span>|<span data-ttu-id="d4b99-132">操作名。</span><span class="sxs-lookup"><span data-stu-id="d4b99-132">The operation name.</span></span>|
|<span data-ttu-id="d4b99-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4b99-133">lastModifiedDateTime</span></span>|<span data-ttu-id="d4b99-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4b99-134">DateTimeOffset</span></span>|<span data-ttu-id="d4b99-135">アプリ操作が変更された最終時刻。</span><span class="sxs-lookup"><span data-stu-id="d4b99-135">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="d4b99-136">state</span><span class="sxs-lookup"><span data-stu-id="d4b99-136">state</span></span>|<span data-ttu-id="d4b99-137">String</span><span class="sxs-lookup"><span data-stu-id="d4b99-137">String</span></span>|<span data-ttu-id="d4b99-138">操作の現在の状態。</span><span class="sxs-lookup"><span data-stu-id="d4b99-138">The current state of the operation</span></span>|
|<span data-ttu-id="d4b99-139">id</span><span class="sxs-lookup"><span data-stu-id="d4b99-139">id</span></span>|<span data-ttu-id="d4b99-140">String</span><span class="sxs-lookup"><span data-stu-id="d4b99-140">String</span></span>|<span data-ttu-id="d4b99-141">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d4b99-141">Key of the entity.</span></span>|
|<span data-ttu-id="d4b99-142">version</span><span class="sxs-lookup"><span data-stu-id="d4b99-142">version</span></span>|<span data-ttu-id="d4b99-143">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="d4b99-143">String</span></span>|<span data-ttu-id="d4b99-144">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="d4b99-144">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4b99-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d4b99-145">Relationships</span></span>
<span data-ttu-id="d4b99-146">なし</span><span class="sxs-lookup"><span data-stu-id="d4b99-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4b99-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d4b99-147">JSON Representation</span></span>
<span data-ttu-id="d4b99-148">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d4b99-148">Here is a JSON representation of the resource.</span></span>
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





