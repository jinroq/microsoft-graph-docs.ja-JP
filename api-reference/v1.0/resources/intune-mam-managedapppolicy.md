---
title: managedAppPolicy リソースの種類
description: ManagedAppPolicy リソースは、プラットフォーム特有のポリシーの基本型を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2615d1331c024c1a04bc7db618e36966cc5bcdff
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465343"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="3b639-103">managedAppPolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3b639-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="3b639-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3b639-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b639-105">ManagedAppPolicy リソースは、プラットフォーム特有のポリシーの基本型を表します。</span><span class="sxs-lookup"><span data-stu-id="3b639-105">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="3b639-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="3b639-106">Methods</span></span>
|<span data-ttu-id="3b639-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="3b639-107">Method</span></span>|<span data-ttu-id="3b639-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3b639-108">Return Type</span></span>|<span data-ttu-id="3b639-109">説明</span><span class="sxs-lookup"><span data-stu-id="3b639-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3b639-110">List managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="3b639-110">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="3b639-111">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="3b639-111">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="3b639-112">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="3b639-112">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="3b639-113">Get managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="3b639-113">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="3b639-114">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="3b639-114">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="3b639-115">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="3b639-115">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="3b639-116">targetApps アクション</span><span class="sxs-lookup"><span data-stu-id="3b639-116">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="3b639-117">なし</span><span class="sxs-lookup"><span data-stu-id="3b639-117">None</span></span>|<span data-ttu-id="3b639-118">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="3b639-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="3b639-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3b639-119">Properties</span></span>
|<span data-ttu-id="3b639-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3b639-120">Property</span></span>|<span data-ttu-id="3b639-121">型</span><span class="sxs-lookup"><span data-stu-id="3b639-121">Type</span></span>|<span data-ttu-id="3b639-122">説明</span><span class="sxs-lookup"><span data-stu-id="3b639-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b639-123">displayName</span><span class="sxs-lookup"><span data-stu-id="3b639-123">displayName</span></span>|<span data-ttu-id="3b639-124">String</span><span class="sxs-lookup"><span data-stu-id="3b639-124">String</span></span>|<span data-ttu-id="3b639-125">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="3b639-125">Policy display name.</span></span>|
|<span data-ttu-id="3b639-126">説明</span><span class="sxs-lookup"><span data-stu-id="3b639-126">description</span></span>|<span data-ttu-id="3b639-127">String</span><span class="sxs-lookup"><span data-stu-id="3b639-127">String</span></span>|<span data-ttu-id="3b639-128">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="3b639-128">The policy's description.</span></span>|
|<span data-ttu-id="3b639-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3b639-129">createdDateTime</span></span>|<span data-ttu-id="3b639-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b639-130">DateTimeOffset</span></span>|<span data-ttu-id="3b639-131">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="3b639-131">The date and time the policy was created.</span></span>|
|<span data-ttu-id="3b639-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3b639-132">lastModifiedDateTime</span></span>|<span data-ttu-id="3b639-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b639-133">DateTimeOffset</span></span>|<span data-ttu-id="3b639-134">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="3b639-134">Last time the policy was modified.</span></span>|
|<span data-ttu-id="3b639-135">id</span><span class="sxs-lookup"><span data-stu-id="3b639-135">id</span></span>|<span data-ttu-id="3b639-136">String</span><span class="sxs-lookup"><span data-stu-id="3b639-136">String</span></span>|<span data-ttu-id="3b639-137">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="3b639-137">Key of the entity.</span></span>|
|<span data-ttu-id="3b639-138">version</span><span class="sxs-lookup"><span data-stu-id="3b639-138">version</span></span>|<span data-ttu-id="3b639-139">String</span><span class="sxs-lookup"><span data-stu-id="3b639-139">String</span></span>|<span data-ttu-id="3b639-140">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="3b639-140">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b639-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3b639-141">Relationships</span></span>
<span data-ttu-id="3b639-142">なし</span><span class="sxs-lookup"><span data-stu-id="3b639-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3b639-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3b639-143">JSON Representation</span></span>
<span data-ttu-id="3b639-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3b639-144">Here is a JSON representation of the resource.</span></span>
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



