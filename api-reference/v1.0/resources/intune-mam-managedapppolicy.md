---
title: managedAppPolicy リソースの種類
description: ManagedAppPolicy リソースは、プラットフォーム特有のポリシーの基本型を表します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5766e3a467a157bac0d876fd0178dc3ba1cb94e2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888082"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="61420-103">managedAppPolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="61420-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="61420-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="61420-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="61420-105">ManagedAppPolicy リソースは、プラットフォーム特有のポリシーの基本型を表します。</span><span class="sxs-lookup"><span data-stu-id="61420-105">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>
## <a name="methods"></a><span data-ttu-id="61420-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="61420-106">Methods</span></span>
|<span data-ttu-id="61420-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="61420-107">Method</span></span>|<span data-ttu-id="61420-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="61420-108">Return Type</span></span>|<span data-ttu-id="61420-109">説明</span><span class="sxs-lookup"><span data-stu-id="61420-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="61420-110">List managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="61420-110">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="61420-111">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="61420-111">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="61420-112">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="61420-112">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="61420-113">Get managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="61420-113">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="61420-114">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="61420-114">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="61420-115">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="61420-115">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="61420-116">targetApps アクション</span><span class="sxs-lookup"><span data-stu-id="61420-116">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="61420-117">なし</span><span class="sxs-lookup"><span data-stu-id="61420-117">None</span></span>|<span data-ttu-id="61420-118">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="61420-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="61420-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="61420-119">Properties</span></span>
|<span data-ttu-id="61420-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="61420-120">Property</span></span>|<span data-ttu-id="61420-121">種類</span><span class="sxs-lookup"><span data-stu-id="61420-121">Type</span></span>|<span data-ttu-id="61420-122">説明</span><span class="sxs-lookup"><span data-stu-id="61420-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61420-123">displayName</span><span class="sxs-lookup"><span data-stu-id="61420-123">displayName</span></span>|<span data-ttu-id="61420-124">String</span><span class="sxs-lookup"><span data-stu-id="61420-124">String</span></span>|<span data-ttu-id="61420-125">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="61420-125">Policy display name.</span></span>|
|<span data-ttu-id="61420-126">説明</span><span class="sxs-lookup"><span data-stu-id="61420-126">description</span></span>|<span data-ttu-id="61420-127">String</span><span class="sxs-lookup"><span data-stu-id="61420-127">String</span></span>|<span data-ttu-id="61420-128">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="61420-128">The policy's description.</span></span>|
|<span data-ttu-id="61420-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="61420-129">createdDateTime</span></span>|<span data-ttu-id="61420-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61420-130">DateTimeOffset</span></span>|<span data-ttu-id="61420-131">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="61420-131">The date and time the policy was created.</span></span>|
|<span data-ttu-id="61420-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="61420-132">lastModifiedDateTime</span></span>|<span data-ttu-id="61420-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61420-133">DateTimeOffset</span></span>|<span data-ttu-id="61420-134">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="61420-134">Last time the policy was modified.</span></span>|
|<span data-ttu-id="61420-135">id</span><span class="sxs-lookup"><span data-stu-id="61420-135">id</span></span>|<span data-ttu-id="61420-136">String</span><span class="sxs-lookup"><span data-stu-id="61420-136">String</span></span>|<span data-ttu-id="61420-137">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="61420-137">Key of the entity.</span></span>|
|<span data-ttu-id="61420-138">version</span><span class="sxs-lookup"><span data-stu-id="61420-138">version</span></span>|<span data-ttu-id="61420-139">String</span><span class="sxs-lookup"><span data-stu-id="61420-139">String</span></span>|<span data-ttu-id="61420-140">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="61420-140">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="61420-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="61420-141">Relationships</span></span>
<span data-ttu-id="61420-142">なし</span><span class="sxs-lookup"><span data-stu-id="61420-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="61420-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="61420-143">JSON Representation</span></span>
<span data-ttu-id="61420-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="61420-144">Here is a JSON representation of the resource.</span></span>
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



