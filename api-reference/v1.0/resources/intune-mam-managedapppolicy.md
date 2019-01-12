---
title: managedAppPolicy リソースの種類
description: ManagedAppPolicy リソースは、プラットフォーム特有のポリシーの基本型を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5054566f0ee80940165ba19f8f0da197b5e4f3c0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981106"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="39d3b-103">managedAppPolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="39d3b-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="39d3b-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="39d3b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="39d3b-105">ManagedAppPolicy リソースは、プラットフォーム特有のポリシーの基本型を表します。</span><span class="sxs-lookup"><span data-stu-id="39d3b-105">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>
## <a name="methods"></a><span data-ttu-id="39d3b-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="39d3b-106">Methods</span></span>
|<span data-ttu-id="39d3b-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="39d3b-107">Method</span></span>|<span data-ttu-id="39d3b-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="39d3b-108">Return Type</span></span>|<span data-ttu-id="39d3b-109">説明</span><span class="sxs-lookup"><span data-stu-id="39d3b-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="39d3b-110">List managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="39d3b-110">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="39d3b-111">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="39d3b-111">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="39d3b-112">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="39d3b-112">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="39d3b-113">Get managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="39d3b-113">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="39d3b-114">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="39d3b-114">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="39d3b-115">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="39d3b-115">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="39d3b-116">targetApps アクション</span><span class="sxs-lookup"><span data-stu-id="39d3b-116">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="39d3b-117">なし</span><span class="sxs-lookup"><span data-stu-id="39d3b-117">None</span></span>|<span data-ttu-id="39d3b-118">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="39d3b-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="39d3b-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="39d3b-119">Properties</span></span>
|<span data-ttu-id="39d3b-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="39d3b-120">Property</span></span>|<span data-ttu-id="39d3b-121">型</span><span class="sxs-lookup"><span data-stu-id="39d3b-121">Type</span></span>|<span data-ttu-id="39d3b-122">説明</span><span class="sxs-lookup"><span data-stu-id="39d3b-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39d3b-123">displayName</span><span class="sxs-lookup"><span data-stu-id="39d3b-123">displayName</span></span>|<span data-ttu-id="39d3b-124">String</span><span class="sxs-lookup"><span data-stu-id="39d3b-124">String</span></span>|<span data-ttu-id="39d3b-125">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="39d3b-125">Policy display name.</span></span>|
|<span data-ttu-id="39d3b-126">説明</span><span class="sxs-lookup"><span data-stu-id="39d3b-126">description</span></span>|<span data-ttu-id="39d3b-127">String</span><span class="sxs-lookup"><span data-stu-id="39d3b-127">String</span></span>|<span data-ttu-id="39d3b-128">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="39d3b-128">The policy's description.</span></span>|
|<span data-ttu-id="39d3b-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="39d3b-129">createdDateTime</span></span>|<span data-ttu-id="39d3b-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39d3b-130">DateTimeOffset</span></span>|<span data-ttu-id="39d3b-131">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="39d3b-131">The date and time the policy was created.</span></span>|
|<span data-ttu-id="39d3b-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="39d3b-132">lastModifiedDateTime</span></span>|<span data-ttu-id="39d3b-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39d3b-133">DateTimeOffset</span></span>|<span data-ttu-id="39d3b-134">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="39d3b-134">Last time the policy was modified.</span></span>|
|<span data-ttu-id="39d3b-135">id</span><span class="sxs-lookup"><span data-stu-id="39d3b-135">id</span></span>|<span data-ttu-id="39d3b-136">String</span><span class="sxs-lookup"><span data-stu-id="39d3b-136">String</span></span>|<span data-ttu-id="39d3b-137">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="39d3b-137">Key of the entity.</span></span>|
|<span data-ttu-id="39d3b-138">version</span><span class="sxs-lookup"><span data-stu-id="39d3b-138">version</span></span>|<span data-ttu-id="39d3b-139">String</span><span class="sxs-lookup"><span data-stu-id="39d3b-139">String</span></span>|<span data-ttu-id="39d3b-140">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="39d3b-140">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="39d3b-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="39d3b-141">Relationships</span></span>
<span data-ttu-id="39d3b-142">なし</span><span class="sxs-lookup"><span data-stu-id="39d3b-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="39d3b-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="39d3b-143">JSON Representation</span></span>
<span data-ttu-id="39d3b-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="39d3b-144">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicy",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String"
}
```



