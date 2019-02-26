---
title: targetedManagedAppConfiguration リソース タイプ
description: カスタム設定のセットをそのまま、ターゲット セキュリティ グループのすべてのユーザーに提供するために使用される構成
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cdc5edf73d0d07cb4da6244e90b3d68b54c24812
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261573"
---
# <a name="targetedmanagedappconfiguration-resource-type"></a><span data-ttu-id="c3018-103">targetedManagedAppConfiguration リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="c3018-103">targetedManagedAppConfiguration resource type</span></span>

> <span data-ttu-id="c3018-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c3018-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3018-105">カスタム設定のセットをそのまま、ターゲット セキュリティ グループのすべてのユーザーに提供するために使用される構成</span><span class="sxs-lookup"><span data-stu-id="c3018-105">Configuration used to deliver a set of custom settings as-is to all users in the targeted security group</span></span>


<span data-ttu-id="c3018-106">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c3018-106">Inherits from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="c3018-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="c3018-107">Methods</span></span>
|<span data-ttu-id="c3018-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="c3018-108">Method</span></span>|<span data-ttu-id="c3018-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c3018-109">Return Type</span></span>|<span data-ttu-id="c3018-110">説明</span><span class="sxs-lookup"><span data-stu-id="c3018-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c3018-111">List targetedManagedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="c3018-111">List targetedManagedAppConfigurations</span></span>](../api/intune-mam-targetedmanagedappconfiguration-list.md)|<span data-ttu-id="c3018-112">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c3018-112">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) collection</span></span>|<span data-ttu-id="c3018-113">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="c3018-113">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="c3018-114">Get targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="c3018-114">Get targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-get.md)|[<span data-ttu-id="c3018-115">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="c3018-115">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="c3018-116">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c3018-116">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="c3018-117">Create targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="c3018-117">Create targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-create.md)|[<span data-ttu-id="c3018-118">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="c3018-118">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="c3018-119">新しい [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c3018-119">Create a new [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="c3018-120">Delete targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="c3018-120">Delete targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-delete.md)|<span data-ttu-id="c3018-121">なし</span><span class="sxs-lookup"><span data-stu-id="c3018-121">None</span></span>|<span data-ttu-id="c3018-122">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="c3018-122">Deletes a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>|
|[<span data-ttu-id="c3018-123">Update targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="c3018-123">Update targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-update.md)|[<span data-ttu-id="c3018-124">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="c3018-124">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="c3018-125">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c3018-125">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="c3018-126">assign action</span><span class="sxs-lookup"><span data-stu-id="c3018-126">assign action</span></span>](../api/intune-mam-targetedmanagedappconfiguration-assign.md)|<span data-ttu-id="c3018-127">なし</span><span class="sxs-lookup"><span data-stu-id="c3018-127">None</span></span>|<span data-ttu-id="c3018-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="c3018-128">Not yet documented</span></span>|
|[<span data-ttu-id="c3018-129">targetApps action</span><span class="sxs-lookup"><span data-stu-id="c3018-129">targetApps action</span></span>](../api/intune-mam-targetedmanagedappconfiguration-targetapps.md)|<span data-ttu-id="c3018-130">なし</span><span class="sxs-lookup"><span data-stu-id="c3018-130">None</span></span>|<span data-ttu-id="c3018-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="c3018-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="c3018-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c3018-132">Properties</span></span>
|<span data-ttu-id="c3018-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c3018-133">Property</span></span>|<span data-ttu-id="c3018-134">型</span><span class="sxs-lookup"><span data-stu-id="c3018-134">Type</span></span>|<span data-ttu-id="c3018-135">説明</span><span class="sxs-lookup"><span data-stu-id="c3018-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3018-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c3018-136">displayName</span></span>|<span data-ttu-id="c3018-137">String</span><span class="sxs-lookup"><span data-stu-id="c3018-137">String</span></span>|<span data-ttu-id="c3018-138">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="c3018-138">Policy display name.</span></span> <span data-ttu-id="c3018-139">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c3018-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c3018-140">説明</span><span class="sxs-lookup"><span data-stu-id="c3018-140">description</span></span>|<span data-ttu-id="c3018-141">String</span><span class="sxs-lookup"><span data-stu-id="c3018-141">String</span></span>|<span data-ttu-id="c3018-142">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="c3018-142">The policy's description.</span></span> <span data-ttu-id="c3018-143">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c3018-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c3018-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c3018-144">createdDateTime</span></span>|<span data-ttu-id="c3018-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3018-145">DateTimeOffset</span></span>|<span data-ttu-id="c3018-146">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="c3018-146">The date and time the policy was created.</span></span> <span data-ttu-id="c3018-147">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c3018-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c3018-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c3018-148">lastModifiedDateTime</span></span>|<span data-ttu-id="c3018-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3018-149">DateTimeOffset</span></span>|<span data-ttu-id="c3018-150">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="c3018-150">Last time the policy was modified.</span></span> <span data-ttu-id="c3018-151">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c3018-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c3018-152">id</span><span class="sxs-lookup"><span data-stu-id="c3018-152">id</span></span>|<span data-ttu-id="c3018-153">文字列</span><span class="sxs-lookup"><span data-stu-id="c3018-153">String</span></span>|<span data-ttu-id="c3018-154">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c3018-154">Key of the entity.</span></span> <span data-ttu-id="c3018-155">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c3018-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c3018-156">version</span><span class="sxs-lookup"><span data-stu-id="c3018-156">version</span></span>|<span data-ttu-id="c3018-157">String</span><span class="sxs-lookup"><span data-stu-id="c3018-157">String</span></span>|<span data-ttu-id="c3018-158">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="c3018-158">Version of the entity.</span></span> <span data-ttu-id="c3018-159">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c3018-159">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c3018-160">customSettings</span><span class="sxs-lookup"><span data-stu-id="c3018-160">customSettings</span></span>|<span data-ttu-id="c3018-161">[keyValuePair](../resources/intune-mam-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c3018-161">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="c3018-162">構成の対象であるユーザーに対して、このサービスで変更せずにアプリに送信される文字列キーと文字列値の一連のペア。[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c3018-162">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="c3018-163">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="c3018-163">deployedAppCount</span></span>|<span data-ttu-id="c3018-164">Int32</span><span class="sxs-lookup"><span data-stu-id="c3018-164">Int32</span></span>|<span data-ttu-id="c3018-165">現在のポリシーが配置されたアプリの数。</span><span class="sxs-lookup"><span data-stu-id="c3018-165">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="c3018-166">isAssigned</span><span class="sxs-lookup"><span data-stu-id="c3018-166">isAssigned</span></span>|<span data-ttu-id="c3018-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3018-167">Boolean</span></span>|<span data-ttu-id="c3018-168">包含グループにポリシーを配置するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c3018-168">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3018-169">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c3018-169">Relationships</span></span>
|<span data-ttu-id="c3018-170">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c3018-170">Relationship</span></span>|<span data-ttu-id="c3018-171">型</span><span class="sxs-lookup"><span data-stu-id="c3018-171">Type</span></span>|<span data-ttu-id="c3018-172">説明</span><span class="sxs-lookup"><span data-stu-id="c3018-172">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3018-173">apps</span><span class="sxs-lookup"><span data-stu-id="c3018-173">apps</span></span>|<span data-ttu-id="c3018-174">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c3018-174">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="c3018-175">ポリシーが配置されたアプリのリスト。</span><span class="sxs-lookup"><span data-stu-id="c3018-175">List of apps to which the policy is deployed.</span></span>|
|<span data-ttu-id="c3018-176">deploymentSummary</span><span class="sxs-lookup"><span data-stu-id="c3018-176">deploymentSummary</span></span>|[<span data-ttu-id="c3018-177">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="c3018-177">managedAppPolicyDeploymentSummary</span></span>](../resources/intune-mam-managedapppolicydeploymentsummary.md)|<span data-ttu-id="c3018-178">構成の展開概要のナビゲーション プロパティ。</span><span class="sxs-lookup"><span data-stu-id="c3018-178">Navigation property to deployment summary of the configuration.</span></span>|
|<span data-ttu-id="c3018-179">assignments</span><span class="sxs-lookup"><span data-stu-id="c3018-179">assignments</span></span>|<span data-ttu-id="c3018-180">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c3018-180">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="c3018-181">ポリシーが配置される包含グループと除外グループのリストのナビゲーション プロパティです。</span><span class="sxs-lookup"><span data-stu-id="c3018-181">Navigation property to list of inclusion and exclusion groups to which the policy is deployed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c3018-182">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c3018-182">JSON Representation</span></span>
<span data-ttu-id="c3018-183">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c3018-183">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.targetedManagedAppConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "deployedAppCount": 1024,
  "isAssigned": true
}
```



