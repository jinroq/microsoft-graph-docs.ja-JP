---
title: managedAppPolicy リソースの種類
description: ManagedAppPolicy リソースは、プラットフォーム特有のポリシーの基本型を表します。
author: tfitzmac
ms.openlocfilehash: b1efe085bc2fc43804049ff4b091e10c458b9a98
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310550"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="8308d-103">managedAppPolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8308d-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="8308d-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8308d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8308d-105">ManagedAppPolicy リソースは、プラットフォーム特有のポリシーの基本型を表します。</span><span class="sxs-lookup"><span data-stu-id="8308d-105">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>
## <a name="methods"></a><span data-ttu-id="8308d-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="8308d-106">Methods</span></span>
|<span data-ttu-id="8308d-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="8308d-107">Method</span></span>|<span data-ttu-id="8308d-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8308d-108">Return Type</span></span>|<span data-ttu-id="8308d-109">説明</span><span class="sxs-lookup"><span data-stu-id="8308d-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8308d-110">List managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="8308d-110">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="8308d-111">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8308d-111">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="8308d-112">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="8308d-112">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="8308d-113">Get managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="8308d-113">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="8308d-114">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="8308d-114">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="8308d-115">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="8308d-115">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="8308d-116">targetApps アクション</span><span class="sxs-lookup"><span data-stu-id="8308d-116">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="8308d-117">なし</span><span class="sxs-lookup"><span data-stu-id="8308d-117">None</span></span>|<span data-ttu-id="8308d-118">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="8308d-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="8308d-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8308d-119">Properties</span></span>
|<span data-ttu-id="8308d-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8308d-120">Property</span></span>|<span data-ttu-id="8308d-121">種類</span><span class="sxs-lookup"><span data-stu-id="8308d-121">Type</span></span>|<span data-ttu-id="8308d-122">説明</span><span class="sxs-lookup"><span data-stu-id="8308d-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8308d-123">displayName</span><span class="sxs-lookup"><span data-stu-id="8308d-123">displayName</span></span>|<span data-ttu-id="8308d-124">String</span><span class="sxs-lookup"><span data-stu-id="8308d-124">String</span></span>|<span data-ttu-id="8308d-125">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="8308d-125">Policy display name.</span></span>|
|<span data-ttu-id="8308d-126">説明</span><span class="sxs-lookup"><span data-stu-id="8308d-126">description</span></span>|<span data-ttu-id="8308d-127">String</span><span class="sxs-lookup"><span data-stu-id="8308d-127">String</span></span>|<span data-ttu-id="8308d-128">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="8308d-128">The policy's description.</span></span>|
|<span data-ttu-id="8308d-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8308d-129">createdDateTime</span></span>|<span data-ttu-id="8308d-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8308d-130">DateTimeOffset</span></span>|<span data-ttu-id="8308d-131">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="8308d-131">The date and time the policy was created.</span></span>|
|<span data-ttu-id="8308d-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8308d-132">lastModifiedDateTime</span></span>|<span data-ttu-id="8308d-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8308d-133">DateTimeOffset</span></span>|<span data-ttu-id="8308d-134">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="8308d-134">Last time the policy was modified.</span></span>|
|<span data-ttu-id="8308d-135">id</span><span class="sxs-lookup"><span data-stu-id="8308d-135">id</span></span>|<span data-ttu-id="8308d-136">String</span><span class="sxs-lookup"><span data-stu-id="8308d-136">String</span></span>|<span data-ttu-id="8308d-137">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8308d-137">Key of the entity.</span></span>|
|<span data-ttu-id="8308d-138">version</span><span class="sxs-lookup"><span data-stu-id="8308d-138">version</span></span>|<span data-ttu-id="8308d-139">String</span><span class="sxs-lookup"><span data-stu-id="8308d-139">String</span></span>|<span data-ttu-id="8308d-140">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="8308d-140">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8308d-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8308d-141">Relationships</span></span>
<span data-ttu-id="8308d-142">なし</span><span class="sxs-lookup"><span data-stu-id="8308d-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8308d-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8308d-143">JSON Representation</span></span>
<span data-ttu-id="8308d-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8308d-144">Here is a JSON representation of the resource.</span></span>
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



