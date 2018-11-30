---
title: managedAppPolicy リソースの種類
description: ManagedAppPolicy リソースは、プラットフォーム特有のポリシーの基本型を表します。
ms.openlocfilehash: 0cd886e594e58dec3486af6d447969f1610c84fe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022865"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="cf5e2-103">managedAppPolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cf5e2-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="cf5e2-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cf5e2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cf5e2-105">ManagedAppPolicy リソースは、プラットフォーム特有のポリシーの基本型を表します。</span><span class="sxs-lookup"><span data-stu-id="cf5e2-105">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>
## <a name="methods"></a><span data-ttu-id="cf5e2-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="cf5e2-106">Methods</span></span>
|<span data-ttu-id="cf5e2-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="cf5e2-107">Method</span></span>|<span data-ttu-id="cf5e2-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="cf5e2-108">Return Type</span></span>|<span data-ttu-id="cf5e2-109">説明</span><span class="sxs-lookup"><span data-stu-id="cf5e2-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cf5e2-110">List managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="cf5e2-110">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="cf5e2-111">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cf5e2-111">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="cf5e2-112">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="cf5e2-112">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="cf5e2-113">Get managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="cf5e2-113">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="cf5e2-114">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="cf5e2-114">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="cf5e2-115">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="cf5e2-115">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="cf5e2-116">targetApps アクション</span><span class="sxs-lookup"><span data-stu-id="cf5e2-116">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="cf5e2-117">なし</span><span class="sxs-lookup"><span data-stu-id="cf5e2-117">None</span></span>|<span data-ttu-id="cf5e2-118">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="cf5e2-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="cf5e2-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cf5e2-119">Properties</span></span>
|<span data-ttu-id="cf5e2-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cf5e2-120">Property</span></span>|<span data-ttu-id="cf5e2-121">型</span><span class="sxs-lookup"><span data-stu-id="cf5e2-121">Type</span></span>|<span data-ttu-id="cf5e2-122">説明</span><span class="sxs-lookup"><span data-stu-id="cf5e2-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf5e2-123">displayName</span><span class="sxs-lookup"><span data-stu-id="cf5e2-123">displayName</span></span>|<span data-ttu-id="cf5e2-124">String</span><span class="sxs-lookup"><span data-stu-id="cf5e2-124">String</span></span>|<span data-ttu-id="cf5e2-125">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="cf5e2-125">Policy display name.</span></span>|
|<span data-ttu-id="cf5e2-126">説明</span><span class="sxs-lookup"><span data-stu-id="cf5e2-126">description</span></span>|<span data-ttu-id="cf5e2-127">String</span><span class="sxs-lookup"><span data-stu-id="cf5e2-127">String</span></span>|<span data-ttu-id="cf5e2-128">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="cf5e2-128">The policy's description.</span></span>|
|<span data-ttu-id="cf5e2-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cf5e2-129">createdDateTime</span></span>|<span data-ttu-id="cf5e2-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf5e2-130">DateTimeOffset</span></span>|<span data-ttu-id="cf5e2-131">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="cf5e2-131">The date and time the policy was created.</span></span>|
|<span data-ttu-id="cf5e2-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cf5e2-132">lastModifiedDateTime</span></span>|<span data-ttu-id="cf5e2-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf5e2-133">DateTimeOffset</span></span>|<span data-ttu-id="cf5e2-134">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="cf5e2-134">Last time the policy was modified.</span></span>|
|<span data-ttu-id="cf5e2-135">id</span><span class="sxs-lookup"><span data-stu-id="cf5e2-135">id</span></span>|<span data-ttu-id="cf5e2-136">String</span><span class="sxs-lookup"><span data-stu-id="cf5e2-136">String</span></span>|<span data-ttu-id="cf5e2-137">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="cf5e2-137">Key of the entity.</span></span>|
|<span data-ttu-id="cf5e2-138">version</span><span class="sxs-lookup"><span data-stu-id="cf5e2-138">version</span></span>|<span data-ttu-id="cf5e2-139">String</span><span class="sxs-lookup"><span data-stu-id="cf5e2-139">String</span></span>|<span data-ttu-id="cf5e2-140">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="cf5e2-140">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cf5e2-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cf5e2-141">Relationships</span></span>
<span data-ttu-id="cf5e2-142">なし</span><span class="sxs-lookup"><span data-stu-id="cf5e2-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cf5e2-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cf5e2-143">JSON Representation</span></span>
<span data-ttu-id="cf5e2-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cf5e2-144">Here is a JSON representation of the resource.</span></span>
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



