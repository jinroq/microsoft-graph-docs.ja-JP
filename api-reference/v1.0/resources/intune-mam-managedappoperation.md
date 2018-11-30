---
title: managedAppOperation リソースの種類
description: アプリ登録に対して適用される操作を表します。
ms.openlocfilehash: 99d75983acda18e11d7abca667679eb66322dcf5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022642"
---
# <a name="managedappoperation-resource-type"></a><span data-ttu-id="14e82-103">managedAppOperation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="14e82-103">managedAppOperation resource type</span></span>

> <span data-ttu-id="14e82-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="14e82-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="14e82-105">アプリ登録に対して適用される操作を表します。</span><span class="sxs-lookup"><span data-stu-id="14e82-105">Represents an operation applied against an app registration.</span></span>
## <a name="methods"></a><span data-ttu-id="14e82-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="14e82-106">Methods</span></span>
|<span data-ttu-id="14e82-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="14e82-107">Method</span></span>|<span data-ttu-id="14e82-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="14e82-108">Return Type</span></span>|<span data-ttu-id="14e82-109">説明</span><span class="sxs-lookup"><span data-stu-id="14e82-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="14e82-110">List managedAppOperations</span><span class="sxs-lookup"><span data-stu-id="14e82-110">List managedAppOperations</span></span>](../api/intune-mam-managedappoperation-list.md)|<span data-ttu-id="14e82-111">[managedAppOperation](../resources/intune-mam-managedappoperation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="14e82-111">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="14e82-112">[managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="14e82-112">List properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) objects.</span></span>|
|[<span data-ttu-id="14e82-113">Get managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="14e82-113">Get managedAppOperation</span></span>](../api/intune-mam-managedappoperation-get.md)|[<span data-ttu-id="14e82-114">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="14e82-114">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="14e82-115">[managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="14e82-115">Read properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="14e82-116">Create managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="14e82-116">Create managedAppOperation</span></span>](../api/intune-mam-managedappoperation-create.md)|[<span data-ttu-id="14e82-117">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="14e82-117">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="14e82-118">新しい [managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="14e82-118">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="14e82-119">Delete managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="14e82-119">Delete managedAppOperation</span></span>](../api/intune-mam-managedappoperation-delete.md)|<span data-ttu-id="14e82-120">なし</span><span class="sxs-lookup"><span data-stu-id="14e82-120">None</span></span>|<span data-ttu-id="14e82-121">[managedAppOperation](../resources/intune-mam-managedappoperation.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="14e82-121">Deletes a [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span></span>|
|[<span data-ttu-id="14e82-122">Update managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="14e82-122">Update managedAppOperation</span></span>](../api/intune-mam-managedappoperation-update.md)|[<span data-ttu-id="14e82-123">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="14e82-123">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="14e82-124">[managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="14e82-124">Update the properties of a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="14e82-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="14e82-125">Properties</span></span>
|<span data-ttu-id="14e82-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="14e82-126">Property</span></span>|<span data-ttu-id="14e82-127">型</span><span class="sxs-lookup"><span data-stu-id="14e82-127">Type</span></span>|<span data-ttu-id="14e82-128">説明</span><span class="sxs-lookup"><span data-stu-id="14e82-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14e82-129">displayName</span><span class="sxs-lookup"><span data-stu-id="14e82-129">displayName</span></span>|<span data-ttu-id="14e82-130">String</span><span class="sxs-lookup"><span data-stu-id="14e82-130">String</span></span>|<span data-ttu-id="14e82-131">操作名。</span><span class="sxs-lookup"><span data-stu-id="14e82-131">The operation name.</span></span>|
|<span data-ttu-id="14e82-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="14e82-132">lastModifiedDateTime</span></span>|<span data-ttu-id="14e82-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14e82-133">DateTimeOffset</span></span>|<span data-ttu-id="14e82-134">アプリ操作が変更された最終時刻。</span><span class="sxs-lookup"><span data-stu-id="14e82-134">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="14e82-135">state</span><span class="sxs-lookup"><span data-stu-id="14e82-135">state</span></span>|<span data-ttu-id="14e82-136">String</span><span class="sxs-lookup"><span data-stu-id="14e82-136">String</span></span>|<span data-ttu-id="14e82-137">操作の現在の状態。</span><span class="sxs-lookup"><span data-stu-id="14e82-137">The current state of the operation</span></span>|
|<span data-ttu-id="14e82-138">id</span><span class="sxs-lookup"><span data-stu-id="14e82-138">id</span></span>|<span data-ttu-id="14e82-139">String</span><span class="sxs-lookup"><span data-stu-id="14e82-139">String</span></span>|<span data-ttu-id="14e82-140">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="14e82-140">Key of the entity.</span></span>|
|<span data-ttu-id="14e82-141">version</span><span class="sxs-lookup"><span data-stu-id="14e82-141">version</span></span>|<span data-ttu-id="14e82-142">String</span><span class="sxs-lookup"><span data-stu-id="14e82-142">String</span></span>|<span data-ttu-id="14e82-143">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="14e82-143">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="14e82-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="14e82-144">Relationships</span></span>
<span data-ttu-id="14e82-145">なし</span><span class="sxs-lookup"><span data-stu-id="14e82-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="14e82-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="14e82-146">JSON Representation</span></span>
<span data-ttu-id="14e82-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="14e82-147">Here is a JSON representation of the resource.</span></span>
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


