---
title: managedAppPolicy リソースの種類
description: ManagedAppPolicy リソースは、プラットフォーム特有のポリシーの基本型を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8e98735a03583fef25fc460c6f989a5a7edf9b44
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144024"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="50258-103">managedAppPolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="50258-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="50258-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="50258-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50258-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="50258-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50258-106">ManagedAppPolicy リソースは、プラットフォーム特有のポリシーの基本型を表します。</span><span class="sxs-lookup"><span data-stu-id="50258-106">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="50258-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="50258-107">Methods</span></span>
|<span data-ttu-id="50258-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="50258-108">Method</span></span>|<span data-ttu-id="50258-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="50258-109">Return Type</span></span>|<span data-ttu-id="50258-110">説明</span><span class="sxs-lookup"><span data-stu-id="50258-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="50258-111">List managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="50258-111">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="50258-112">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="50258-112">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="50258-113">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="50258-113">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="50258-114">Get managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="50258-114">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="50258-115">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="50258-115">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="50258-116">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="50258-116">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="50258-117">targetApps アクション</span><span class="sxs-lookup"><span data-stu-id="50258-117">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="50258-118">なし</span><span class="sxs-lookup"><span data-stu-id="50258-118">None</span></span>|<span data-ttu-id="50258-119">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="50258-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="50258-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="50258-120">Properties</span></span>
|<span data-ttu-id="50258-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="50258-121">Property</span></span>|<span data-ttu-id="50258-122">型</span><span class="sxs-lookup"><span data-stu-id="50258-122">Type</span></span>|<span data-ttu-id="50258-123">説明</span><span class="sxs-lookup"><span data-stu-id="50258-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50258-124">displayName</span><span class="sxs-lookup"><span data-stu-id="50258-124">displayName</span></span>|<span data-ttu-id="50258-125">String</span><span class="sxs-lookup"><span data-stu-id="50258-125">String</span></span>|<span data-ttu-id="50258-126">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="50258-126">Policy display name.</span></span>|
|<span data-ttu-id="50258-127">説明</span><span class="sxs-lookup"><span data-stu-id="50258-127">description</span></span>|<span data-ttu-id="50258-128">String</span><span class="sxs-lookup"><span data-stu-id="50258-128">String</span></span>|<span data-ttu-id="50258-129">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="50258-129">The policy's description.</span></span>|
|<span data-ttu-id="50258-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="50258-130">createdDateTime</span></span>|<span data-ttu-id="50258-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50258-131">DateTimeOffset</span></span>|<span data-ttu-id="50258-132">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="50258-132">The date and time the policy was created.</span></span>|
|<span data-ttu-id="50258-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="50258-133">lastModifiedDateTime</span></span>|<span data-ttu-id="50258-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50258-134">DateTimeOffset</span></span>|<span data-ttu-id="50258-135">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="50258-135">Last time the policy was modified.</span></span>|
|<span data-ttu-id="50258-136">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="50258-136">roleScopeTagIds</span></span>|<span data-ttu-id="50258-137">String collection</span><span class="sxs-lookup"><span data-stu-id="50258-137">String collection</span></span>|<span data-ttu-id="50258-138">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="50258-138">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="50258-139">id</span><span class="sxs-lookup"><span data-stu-id="50258-139">id</span></span>|<span data-ttu-id="50258-140">文字列</span><span class="sxs-lookup"><span data-stu-id="50258-140">String</span></span>|<span data-ttu-id="50258-141">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="50258-141">Key of the entity.</span></span>|
|<span data-ttu-id="50258-142">version</span><span class="sxs-lookup"><span data-stu-id="50258-142">version</span></span>|<span data-ttu-id="50258-143">String</span><span class="sxs-lookup"><span data-stu-id="50258-143">String</span></span>|<span data-ttu-id="50258-144">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="50258-144">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="50258-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="50258-145">Relationships</span></span>
<span data-ttu-id="50258-146">なし</span><span class="sxs-lookup"><span data-stu-id="50258-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="50258-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="50258-147">JSON Representation</span></span>
<span data-ttu-id="50258-148">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="50258-148">Here is a JSON representation of the resource.</span></span>
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
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "version": "String"
}
```




