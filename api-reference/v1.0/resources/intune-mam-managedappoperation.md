---
title: managedAppOperation リソースの種類
description: アプリ登録に対して適用される操作を表します。
author: tfitzmac
ms.openlocfilehash: d92c467f1ff5eae403f348deac2cb6c17a3a950d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345410"
---
# <a name="managedappoperation-resource-type"></a><span data-ttu-id="f7993-103">managedAppOperation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f7993-103">managedAppOperation resource type</span></span>

> <span data-ttu-id="f7993-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f7993-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f7993-105">アプリ登録に対して適用される操作を表します。</span><span class="sxs-lookup"><span data-stu-id="f7993-105">Represents an operation applied against an app registration.</span></span>
## <a name="methods"></a><span data-ttu-id="f7993-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="f7993-106">Methods</span></span>
|<span data-ttu-id="f7993-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="f7993-107">Method</span></span>|<span data-ttu-id="f7993-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f7993-108">Return Type</span></span>|<span data-ttu-id="f7993-109">説明</span><span class="sxs-lookup"><span data-stu-id="f7993-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f7993-110">List managedAppOperations</span><span class="sxs-lookup"><span data-stu-id="f7993-110">List managedAppOperations</span></span>](../api/intune-mam-managedappoperation-list.md)|<span data-ttu-id="f7993-111">[managedAppOperation](../resources/intune-mam-managedappoperation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f7993-111">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="f7993-112">[managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="f7993-112">List properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) objects.</span></span>|
|[<span data-ttu-id="f7993-113">Get managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="f7993-113">Get managedAppOperation</span></span>](../api/intune-mam-managedappoperation-get.md)|[<span data-ttu-id="f7993-114">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="f7993-114">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="f7993-115">[managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f7993-115">Read properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="f7993-116">Create managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="f7993-116">Create managedAppOperation</span></span>](../api/intune-mam-managedappoperation-create.md)|[<span data-ttu-id="f7993-117">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="f7993-117">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="f7993-118">新しい [managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f7993-118">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="f7993-119">Delete managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="f7993-119">Delete managedAppOperation</span></span>](../api/intune-mam-managedappoperation-delete.md)|<span data-ttu-id="f7993-120">なし</span><span class="sxs-lookup"><span data-stu-id="f7993-120">None</span></span>|<span data-ttu-id="f7993-121">[managedAppOperation](../resources/intune-mam-managedappoperation.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="f7993-121">Deletes a [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span></span>|
|[<span data-ttu-id="f7993-122">Update managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="f7993-122">Update managedAppOperation</span></span>](../api/intune-mam-managedappoperation-update.md)|[<span data-ttu-id="f7993-123">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="f7993-123">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="f7993-124">[managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f7993-124">Update the properties of a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f7993-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f7993-125">Properties</span></span>
|<span data-ttu-id="f7993-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f7993-126">Property</span></span>|<span data-ttu-id="f7993-127">種類</span><span class="sxs-lookup"><span data-stu-id="f7993-127">Type</span></span>|<span data-ttu-id="f7993-128">説明</span><span class="sxs-lookup"><span data-stu-id="f7993-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7993-129">displayName</span><span class="sxs-lookup"><span data-stu-id="f7993-129">displayName</span></span>|<span data-ttu-id="f7993-130">String</span><span class="sxs-lookup"><span data-stu-id="f7993-130">String</span></span>|<span data-ttu-id="f7993-131">操作名。</span><span class="sxs-lookup"><span data-stu-id="f7993-131">The operation name.</span></span>|
|<span data-ttu-id="f7993-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f7993-132">lastModifiedDateTime</span></span>|<span data-ttu-id="f7993-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7993-133">DateTimeOffset</span></span>|<span data-ttu-id="f7993-134">アプリ操作が変更された最終時刻。</span><span class="sxs-lookup"><span data-stu-id="f7993-134">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="f7993-135">state</span><span class="sxs-lookup"><span data-stu-id="f7993-135">state</span></span>|<span data-ttu-id="f7993-136">String</span><span class="sxs-lookup"><span data-stu-id="f7993-136">String</span></span>|<span data-ttu-id="f7993-137">操作の現在の状態。</span><span class="sxs-lookup"><span data-stu-id="f7993-137">The current state of the operation</span></span>|
|<span data-ttu-id="f7993-138">id</span><span class="sxs-lookup"><span data-stu-id="f7993-138">id</span></span>|<span data-ttu-id="f7993-139">String</span><span class="sxs-lookup"><span data-stu-id="f7993-139">String</span></span>|<span data-ttu-id="f7993-140">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f7993-140">Key of the entity.</span></span>|
|<span data-ttu-id="f7993-141">version</span><span class="sxs-lookup"><span data-stu-id="f7993-141">version</span></span>|<span data-ttu-id="f7993-142">String</span><span class="sxs-lookup"><span data-stu-id="f7993-142">String</span></span>|<span data-ttu-id="f7993-143">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="f7993-143">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7993-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f7993-144">Relationships</span></span>
<span data-ttu-id="f7993-145">なし</span><span class="sxs-lookup"><span data-stu-id="f7993-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f7993-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f7993-146">JSON Representation</span></span>
<span data-ttu-id="f7993-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f7993-147">Here is a JSON representation of the resource.</span></span>
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



