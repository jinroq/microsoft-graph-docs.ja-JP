---
title: managedMobileApp リソースの種類
description: アプリ展開の識別子。
ms.openlocfilehash: 9bab1e53ff5fdc6065b1031349823e6ae4fee36c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069430"
---
# <a name="managedmobileapp-resource-type"></a><span data-ttu-id="e6c78-103">managedMobileApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e6c78-103">managedMobileApp resource type</span></span>

> <span data-ttu-id="e6c78-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e6c78-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e6c78-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e6c78-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e6c78-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e6c78-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e6c78-107">アプリ展開の識別子。</span><span class="sxs-lookup"><span data-stu-id="e6c78-107">The identifier for the deployment an app.</span></span>
## <a name="methods"></a><span data-ttu-id="e6c78-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="e6c78-108">Methods</span></span>
|<span data-ttu-id="e6c78-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="e6c78-109">Method</span></span>|<span data-ttu-id="e6c78-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e6c78-110">Return Type</span></span>|<span data-ttu-id="e6c78-111">説明</span><span class="sxs-lookup"><span data-stu-id="e6c78-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e6c78-112">List managedMobileApps</span><span class="sxs-lookup"><span data-stu-id="e6c78-112">List managedMobileApps</span></span>](../api/intune-mam-managedmobileapp-list.md)|<span data-ttu-id="e6c78-113">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e6c78-113">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="e6c78-114">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="e6c78-114">List properties and relationships of the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) objects.</span></span>|
|[<span data-ttu-id="e6c78-115">Get managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="e6c78-115">Get managedMobileApp</span></span>](../api/intune-mam-managedmobileapp-get.md)|[<span data-ttu-id="e6c78-116">managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="e6c78-116">managedMobileApp</span></span>](../resources/intune-mam-managedmobileapp.md)|<span data-ttu-id="e6c78-117">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e6c78-117">Read properties and relationships of the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>|
|[<span data-ttu-id="e6c78-118">Create managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="e6c78-118">Create managedMobileApp</span></span>](../api/intune-mam-managedmobileapp-create.md)|[<span data-ttu-id="e6c78-119">managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="e6c78-119">managedMobileApp</span></span>](../resources/intune-mam-managedmobileapp.md)|<span data-ttu-id="e6c78-120">新しい [managedMobileApp](../resources/intune-mam-managedmobileapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e6c78-120">Create a new [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>|
|[<span data-ttu-id="e6c78-121">Delete managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="e6c78-121">Delete managedMobileApp</span></span>](../api/intune-mam-managedmobileapp-delete.md)|<span data-ttu-id="e6c78-122">なし</span><span class="sxs-lookup"><span data-stu-id="e6c78-122">None</span></span>|<span data-ttu-id="e6c78-123">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="e6c78-123">Deletes a [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span></span>|
|[<span data-ttu-id="e6c78-124">Update managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="e6c78-124">Update managedMobileApp</span></span>](../api/intune-mam-managedmobileapp-update.md)|[<span data-ttu-id="e6c78-125">managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="e6c78-125">managedMobileApp</span></span>](../resources/intune-mam-managedmobileapp.md)|<span data-ttu-id="e6c78-126">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e6c78-126">Update the properties of a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e6c78-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e6c78-127">Properties</span></span>
|<span data-ttu-id="e6c78-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e6c78-128">Property</span></span>|<span data-ttu-id="e6c78-129">型</span><span class="sxs-lookup"><span data-stu-id="e6c78-129">Type</span></span>|<span data-ttu-id="e6c78-130">説明</span><span class="sxs-lookup"><span data-stu-id="e6c78-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6c78-131">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="e6c78-131">mobileAppIdentifier</span></span>|[<span data-ttu-id="e6c78-132">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="e6c78-132">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="e6c78-133">対象のオペレーティング システムの種類のアプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="e6c78-133">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="e6c78-134">id</span><span class="sxs-lookup"><span data-stu-id="e6c78-134">id</span></span>|<span data-ttu-id="e6c78-135">String</span><span class="sxs-lookup"><span data-stu-id="e6c78-135">String</span></span>|<span data-ttu-id="e6c78-136">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e6c78-136">Key of the entity.</span></span>|
|<span data-ttu-id="e6c78-137">version</span><span class="sxs-lookup"><span data-stu-id="e6c78-137">version</span></span>|<span data-ttu-id="e6c78-138">String</span><span class="sxs-lookup"><span data-stu-id="e6c78-138">String</span></span>|<span data-ttu-id="e6c78-139">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="e6c78-139">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6c78-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e6c78-140">Relationships</span></span>
<span data-ttu-id="e6c78-141">なし</span><span class="sxs-lookup"><span data-stu-id="e6c78-141">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e6c78-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e6c78-142">JSON Representation</span></span>
<span data-ttu-id="e6c78-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e6c78-143">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedMobileApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "String (identifier)",
  "version": "String"
}
```





