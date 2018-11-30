---
title: managedAppOperation リソースの種類
description: アプリ登録に対して適用される操作を表します。
ms.openlocfilehash: 267adafc5a74ad447dfb3468cf9238e1c4642e5f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066549"
---
# <a name="managedappoperation-resource-type"></a><span data-ttu-id="4b5e8-103">managedAppOperation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4b5e8-103">managedAppOperation resource type</span></span>

> <span data-ttu-id="4b5e8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4b5e8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4b5e8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4b5e8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4b5e8-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4b5e8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4b5e8-107">アプリ登録に対して適用される操作を表します。</span><span class="sxs-lookup"><span data-stu-id="4b5e8-107">Represents an operation applied against an app registration.</span></span>
## <a name="methods"></a><span data-ttu-id="4b5e8-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="4b5e8-108">Methods</span></span>
|<span data-ttu-id="4b5e8-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="4b5e8-109">Method</span></span>|<span data-ttu-id="4b5e8-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4b5e8-110">Return Type</span></span>|<span data-ttu-id="4b5e8-111">説明</span><span class="sxs-lookup"><span data-stu-id="4b5e8-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4b5e8-112">List managedAppOperations</span><span class="sxs-lookup"><span data-stu-id="4b5e8-112">List managedAppOperations</span></span>](../api/intune-mam-managedappoperation-list.md)|<span data-ttu-id="4b5e8-113">[managedAppOperation](../resources/intune-mam-managedappoperation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4b5e8-113">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="4b5e8-114">[managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="4b5e8-114">List properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) objects.</span></span>|
|[<span data-ttu-id="4b5e8-115">Get managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="4b5e8-115">Get managedAppOperation</span></span>](../api/intune-mam-managedappoperation-get.md)|[<span data-ttu-id="4b5e8-116">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="4b5e8-116">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="4b5e8-117">[managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="4b5e8-117">Read properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="4b5e8-118">Create managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="4b5e8-118">Create managedAppOperation</span></span>](../api/intune-mam-managedappoperation-create.md)|[<span data-ttu-id="4b5e8-119">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="4b5e8-119">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="4b5e8-120">新しい [managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="4b5e8-120">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="4b5e8-121">Delete managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="4b5e8-121">Delete managedAppOperation</span></span>](../api/intune-mam-managedappoperation-delete.md)|<span data-ttu-id="4b5e8-122">なし</span><span class="sxs-lookup"><span data-stu-id="4b5e8-122">None</span></span>|<span data-ttu-id="4b5e8-123">[managedAppOperation](../resources/intune-mam-managedappoperation.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="4b5e8-123">Deletes a [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span></span>|
|[<span data-ttu-id="4b5e8-124">Update managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="4b5e8-124">Update managedAppOperation</span></span>](../api/intune-mam-managedappoperation-update.md)|[<span data-ttu-id="4b5e8-125">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="4b5e8-125">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="4b5e8-126">[managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4b5e8-126">Update the properties of a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4b5e8-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4b5e8-127">Properties</span></span>
|<span data-ttu-id="4b5e8-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4b5e8-128">Property</span></span>|<span data-ttu-id="4b5e8-129">型</span><span class="sxs-lookup"><span data-stu-id="4b5e8-129">Type</span></span>|<span data-ttu-id="4b5e8-130">説明</span><span class="sxs-lookup"><span data-stu-id="4b5e8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b5e8-131">displayName</span><span class="sxs-lookup"><span data-stu-id="4b5e8-131">displayName</span></span>|<span data-ttu-id="4b5e8-132">String</span><span class="sxs-lookup"><span data-stu-id="4b5e8-132">String</span></span>|<span data-ttu-id="4b5e8-133">操作名。</span><span class="sxs-lookup"><span data-stu-id="4b5e8-133">The operation name.</span></span>|
|<span data-ttu-id="4b5e8-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4b5e8-134">lastModifiedDateTime</span></span>|<span data-ttu-id="4b5e8-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b5e8-135">DateTimeOffset</span></span>|<span data-ttu-id="4b5e8-136">アプリ操作が変更された最終時刻。</span><span class="sxs-lookup"><span data-stu-id="4b5e8-136">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="4b5e8-137">state</span><span class="sxs-lookup"><span data-stu-id="4b5e8-137">state</span></span>|<span data-ttu-id="4b5e8-138">String</span><span class="sxs-lookup"><span data-stu-id="4b5e8-138">String</span></span>|<span data-ttu-id="4b5e8-139">操作の現在の状態。</span><span class="sxs-lookup"><span data-stu-id="4b5e8-139">The current state of the operation</span></span>|
|<span data-ttu-id="4b5e8-140">id</span><span class="sxs-lookup"><span data-stu-id="4b5e8-140">id</span></span>|<span data-ttu-id="4b5e8-141">String</span><span class="sxs-lookup"><span data-stu-id="4b5e8-141">String</span></span>|<span data-ttu-id="4b5e8-142">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="4b5e8-142">Key of the entity.</span></span>|
|<span data-ttu-id="4b5e8-143">version</span><span class="sxs-lookup"><span data-stu-id="4b5e8-143">version</span></span>|<span data-ttu-id="4b5e8-144">String</span><span class="sxs-lookup"><span data-stu-id="4b5e8-144">String</span></span>|<span data-ttu-id="4b5e8-145">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="4b5e8-145">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b5e8-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4b5e8-146">Relationships</span></span>
<span data-ttu-id="4b5e8-147">なし</span><span class="sxs-lookup"><span data-stu-id="4b5e8-147">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4b5e8-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4b5e8-148">JSON Representation</span></span>
<span data-ttu-id="4b5e8-149">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4b5e8-149">Here is a JSON representation of the resource.</span></span>
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





