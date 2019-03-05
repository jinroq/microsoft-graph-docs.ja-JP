---
title: managedAppPolicy リソースの種類
description: ManagedAppPolicy リソースは、プラットフォーム特有のポリシーの基本型を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2615d1331c024c1a04bc7db618e36966cc5bcdff
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251168"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="8299a-103">managedAppPolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8299a-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="8299a-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8299a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8299a-105">ManagedAppPolicy リソースは、プラットフォーム特有のポリシーの基本型を表します。</span><span class="sxs-lookup"><span data-stu-id="8299a-105">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="8299a-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="8299a-106">Methods</span></span>
|<span data-ttu-id="8299a-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="8299a-107">Method</span></span>|<span data-ttu-id="8299a-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8299a-108">Return Type</span></span>|<span data-ttu-id="8299a-109">説明</span><span class="sxs-lookup"><span data-stu-id="8299a-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8299a-110">List managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="8299a-110">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="8299a-111">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8299a-111">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="8299a-112">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="8299a-112">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="8299a-113">Get managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="8299a-113">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="8299a-114">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="8299a-114">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="8299a-115">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="8299a-115">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="8299a-116">targetApps アクション</span><span class="sxs-lookup"><span data-stu-id="8299a-116">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="8299a-117">なし</span><span class="sxs-lookup"><span data-stu-id="8299a-117">None</span></span>|<span data-ttu-id="8299a-118">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="8299a-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="8299a-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8299a-119">Properties</span></span>
|<span data-ttu-id="8299a-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8299a-120">Property</span></span>|<span data-ttu-id="8299a-121">型</span><span class="sxs-lookup"><span data-stu-id="8299a-121">Type</span></span>|<span data-ttu-id="8299a-122">説明</span><span class="sxs-lookup"><span data-stu-id="8299a-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8299a-123">displayName</span><span class="sxs-lookup"><span data-stu-id="8299a-123">displayName</span></span>|<span data-ttu-id="8299a-124">String</span><span class="sxs-lookup"><span data-stu-id="8299a-124">String</span></span>|<span data-ttu-id="8299a-125">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="8299a-125">Policy display name.</span></span>|
|<span data-ttu-id="8299a-126">説明</span><span class="sxs-lookup"><span data-stu-id="8299a-126">description</span></span>|<span data-ttu-id="8299a-127">String</span><span class="sxs-lookup"><span data-stu-id="8299a-127">String</span></span>|<span data-ttu-id="8299a-128">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="8299a-128">The policy's description.</span></span>|
|<span data-ttu-id="8299a-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8299a-129">createdDateTime</span></span>|<span data-ttu-id="8299a-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8299a-130">DateTimeOffset</span></span>|<span data-ttu-id="8299a-131">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="8299a-131">The date and time the policy was created.</span></span>|
|<span data-ttu-id="8299a-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8299a-132">lastModifiedDateTime</span></span>|<span data-ttu-id="8299a-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8299a-133">DateTimeOffset</span></span>|<span data-ttu-id="8299a-134">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="8299a-134">Last time the policy was modified.</span></span>|
|<span data-ttu-id="8299a-135">id</span><span class="sxs-lookup"><span data-stu-id="8299a-135">id</span></span>|<span data-ttu-id="8299a-136">文字列</span><span class="sxs-lookup"><span data-stu-id="8299a-136">String</span></span>|<span data-ttu-id="8299a-137">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8299a-137">Key of the entity.</span></span>|
|<span data-ttu-id="8299a-138">version</span><span class="sxs-lookup"><span data-stu-id="8299a-138">version</span></span>|<span data-ttu-id="8299a-139">String</span><span class="sxs-lookup"><span data-stu-id="8299a-139">String</span></span>|<span data-ttu-id="8299a-140">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="8299a-140">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8299a-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8299a-141">Relationships</span></span>
<span data-ttu-id="8299a-142">なし</span><span class="sxs-lookup"><span data-stu-id="8299a-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8299a-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8299a-143">JSON Representation</span></span>
<span data-ttu-id="8299a-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8299a-144">Here is a JSON representation of the resource.</span></span>
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



