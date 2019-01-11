---
title: managedAppPolicy リソースの種類
description: ManagedAppPolicy リソースは、プラットフォーム特有のポリシーの基本型を表します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3cea81d492e708c1d21039c6286fe01e70a590b4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840734"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="791e6-103">managedAppPolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="791e6-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="791e6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="791e6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="791e6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="791e6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="791e6-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="791e6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="791e6-107">ManagedAppPolicy リソースは、プラットフォーム特有のポリシーの基本型を表します。</span><span class="sxs-lookup"><span data-stu-id="791e6-107">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>
## <a name="methods"></a><span data-ttu-id="791e6-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="791e6-108">Methods</span></span>
|<span data-ttu-id="791e6-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="791e6-109">Method</span></span>|<span data-ttu-id="791e6-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="791e6-110">Return Type</span></span>|<span data-ttu-id="791e6-111">説明</span><span class="sxs-lookup"><span data-stu-id="791e6-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="791e6-112">List managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="791e6-112">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="791e6-113">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="791e6-113">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="791e6-114">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="791e6-114">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="791e6-115">Get managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="791e6-115">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="791e6-116">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="791e6-116">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="791e6-117">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="791e6-117">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="791e6-118">targetApps アクション</span><span class="sxs-lookup"><span data-stu-id="791e6-118">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="791e6-119">なし</span><span class="sxs-lookup"><span data-stu-id="791e6-119">None</span></span>|<span data-ttu-id="791e6-120">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="791e6-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="791e6-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="791e6-121">Properties</span></span>
|<span data-ttu-id="791e6-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="791e6-122">Property</span></span>|<span data-ttu-id="791e6-123">種類</span><span class="sxs-lookup"><span data-stu-id="791e6-123">Type</span></span>|<span data-ttu-id="791e6-124">説明</span><span class="sxs-lookup"><span data-stu-id="791e6-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="791e6-125">displayName</span><span class="sxs-lookup"><span data-stu-id="791e6-125">displayName</span></span>|<span data-ttu-id="791e6-126">String</span><span class="sxs-lookup"><span data-stu-id="791e6-126">String</span></span>|<span data-ttu-id="791e6-127">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="791e6-127">Policy display name.</span></span>|
|<span data-ttu-id="791e6-128">説明</span><span class="sxs-lookup"><span data-stu-id="791e6-128">description</span></span>|<span data-ttu-id="791e6-129">String</span><span class="sxs-lookup"><span data-stu-id="791e6-129">String</span></span>|<span data-ttu-id="791e6-130">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="791e6-130">The policy's description.</span></span>|
|<span data-ttu-id="791e6-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="791e6-131">createdDateTime</span></span>|<span data-ttu-id="791e6-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="791e6-132">DateTimeOffset</span></span>|<span data-ttu-id="791e6-133">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="791e6-133">The date and time the policy was created.</span></span>|
|<span data-ttu-id="791e6-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="791e6-134">lastModifiedDateTime</span></span>|<span data-ttu-id="791e6-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="791e6-135">DateTimeOffset</span></span>|<span data-ttu-id="791e6-136">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="791e6-136">Last time the policy was modified.</span></span>|
|<span data-ttu-id="791e6-137">id</span><span class="sxs-lookup"><span data-stu-id="791e6-137">id</span></span>|<span data-ttu-id="791e6-138">String</span><span class="sxs-lookup"><span data-stu-id="791e6-138">String</span></span>|<span data-ttu-id="791e6-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="791e6-139">Key of the entity.</span></span>|
|<span data-ttu-id="791e6-140">version</span><span class="sxs-lookup"><span data-stu-id="791e6-140">version</span></span>|<span data-ttu-id="791e6-141">String</span><span class="sxs-lookup"><span data-stu-id="791e6-141">String</span></span>|<span data-ttu-id="791e6-142">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="791e6-142">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="791e6-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="791e6-143">Relationships</span></span>
<span data-ttu-id="791e6-144">なし</span><span class="sxs-lookup"><span data-stu-id="791e6-144">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="791e6-145">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="791e6-145">JSON Representation</span></span>
<span data-ttu-id="791e6-146">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="791e6-146">Here is a JSON representation of the resource.</span></span>
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





