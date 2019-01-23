---
title: targetedManagedAppConfiguration リソース タイプ
description: カスタム設定のセットをそのまま、ターゲット セキュリティ グループのすべてのユーザーに提供するために使用される構成
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 41a8ad1e246b977a853ec9ae16b8485894862b0e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420928"
---
# <a name="targetedmanagedappconfiguration-resource-type"></a><span data-ttu-id="35373-103">targetedManagedAppConfiguration リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="35373-103">targetedManagedAppConfiguration resource type</span></span>

> <span data-ttu-id="35373-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="35373-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="35373-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="35373-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="35373-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="35373-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35373-107">カスタム設定のセットをそのまま、ターゲット セキュリティ グループのすべてのユーザーに提供するために使用される構成</span><span class="sxs-lookup"><span data-stu-id="35373-107">Configuration used to deliver a set of custom settings as-is to all users in the targeted security group</span></span>


<span data-ttu-id="35373-108">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="35373-108">Inherits from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="35373-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="35373-109">Methods</span></span>
|<span data-ttu-id="35373-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="35373-110">Method</span></span>|<span data-ttu-id="35373-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="35373-111">Return Type</span></span>|<span data-ttu-id="35373-112">説明</span><span class="sxs-lookup"><span data-stu-id="35373-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="35373-113">List targetedManagedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="35373-113">List targetedManagedAppConfigurations</span></span>](../api/intune-mam-targetedmanagedappconfiguration-list.md)|<span data-ttu-id="35373-114">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="35373-114">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) collection</span></span>|<span data-ttu-id="35373-115">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="35373-115">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="35373-116">Get targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="35373-116">Get targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-get.md)|[<span data-ttu-id="35373-117">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="35373-117">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="35373-118">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="35373-118">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="35373-119">Create targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="35373-119">Create targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-create.md)|[<span data-ttu-id="35373-120">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="35373-120">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="35373-121">新しい [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="35373-121">Create a new [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="35373-122">Delete targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="35373-122">Delete targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-delete.md)|<span data-ttu-id="35373-123">なし</span><span class="sxs-lookup"><span data-stu-id="35373-123">None</span></span>|<span data-ttu-id="35373-124">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="35373-124">Deletes a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>|
|[<span data-ttu-id="35373-125">Update targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="35373-125">Update targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-update.md)|[<span data-ttu-id="35373-126">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="35373-126">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="35373-127">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="35373-127">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="35373-128">assign action</span><span class="sxs-lookup"><span data-stu-id="35373-128">assign action</span></span>](../api/intune-mam-targetedmanagedappconfiguration-assign.md)|<span data-ttu-id="35373-129">なし</span><span class="sxs-lookup"><span data-stu-id="35373-129">None</span></span>|<span data-ttu-id="35373-130">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="35373-130">Not yet documented</span></span>|
|[<span data-ttu-id="35373-131">targetApps action</span><span class="sxs-lookup"><span data-stu-id="35373-131">targetApps action</span></span>](../api/intune-mam-targetedmanagedappconfiguration-targetapps.md)|<span data-ttu-id="35373-132">なし</span><span class="sxs-lookup"><span data-stu-id="35373-132">None</span></span>|<span data-ttu-id="35373-133">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="35373-133">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="35373-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35373-134">Properties</span></span>
|<span data-ttu-id="35373-135">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35373-135">Property</span></span>|<span data-ttu-id="35373-136">型</span><span class="sxs-lookup"><span data-stu-id="35373-136">Type</span></span>|<span data-ttu-id="35373-137">説明</span><span class="sxs-lookup"><span data-stu-id="35373-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35373-138">displayName</span><span class="sxs-lookup"><span data-stu-id="35373-138">displayName</span></span>|<span data-ttu-id="35373-139">String</span><span class="sxs-lookup"><span data-stu-id="35373-139">String</span></span>|<span data-ttu-id="35373-140">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="35373-140">Policy display name.</span></span> <span data-ttu-id="35373-141">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="35373-141">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="35373-142">説明</span><span class="sxs-lookup"><span data-stu-id="35373-142">description</span></span>|<span data-ttu-id="35373-143">String</span><span class="sxs-lookup"><span data-stu-id="35373-143">String</span></span>|<span data-ttu-id="35373-144">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="35373-144">The policy's description.</span></span> <span data-ttu-id="35373-145">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="35373-145">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="35373-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="35373-146">createdDateTime</span></span>|<span data-ttu-id="35373-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35373-147">DateTimeOffset</span></span>|<span data-ttu-id="35373-148">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="35373-148">The date and time the policy was created.</span></span> <span data-ttu-id="35373-149">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="35373-149">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="35373-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="35373-150">lastModifiedDateTime</span></span>|<span data-ttu-id="35373-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35373-151">DateTimeOffset</span></span>|<span data-ttu-id="35373-152">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="35373-152">Last time the policy was modified.</span></span> <span data-ttu-id="35373-153">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="35373-153">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="35373-154">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="35373-154">roleScopeTagIds</span></span>|<span data-ttu-id="35373-155">String コレクション</span><span class="sxs-lookup"><span data-stu-id="35373-155">String collection</span></span>|<span data-ttu-id="35373-156">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="35373-156">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="35373-157">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="35373-157">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="35373-158">id</span><span class="sxs-lookup"><span data-stu-id="35373-158">id</span></span>|<span data-ttu-id="35373-159">String</span><span class="sxs-lookup"><span data-stu-id="35373-159">String</span></span>|<span data-ttu-id="35373-160">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="35373-160">Key of the entity.</span></span> <span data-ttu-id="35373-161">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="35373-161">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="35373-162">version</span><span class="sxs-lookup"><span data-stu-id="35373-162">version</span></span>|<span data-ttu-id="35373-163">String</span><span class="sxs-lookup"><span data-stu-id="35373-163">String</span></span>|<span data-ttu-id="35373-164">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="35373-164">Version of the entity.</span></span> <span data-ttu-id="35373-165">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="35373-165">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="35373-166">customSettings</span><span class="sxs-lookup"><span data-stu-id="35373-166">customSettings</span></span>|<span data-ttu-id="35373-167">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="35373-167">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="35373-168">構成の対象であるユーザーに対して、このサービスで変更せずにアプリに送信される文字列キーと文字列値の一連のペア。[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="35373-168">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="35373-169">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="35373-169">deployedAppCount</span></span>|<span data-ttu-id="35373-170">Int32</span><span class="sxs-lookup"><span data-stu-id="35373-170">Int32</span></span>|<span data-ttu-id="35373-171">現在のポリシーが配置されたアプリの数。</span><span class="sxs-lookup"><span data-stu-id="35373-171">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="35373-172">isAssigned</span><span class="sxs-lookup"><span data-stu-id="35373-172">isAssigned</span></span>|<span data-ttu-id="35373-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="35373-173">Boolean</span></span>|<span data-ttu-id="35373-174">包含グループにポリシーを配置するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="35373-174">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35373-175">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="35373-175">Relationships</span></span>
|<span data-ttu-id="35373-176">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="35373-176">Relationship</span></span>|<span data-ttu-id="35373-177">型</span><span class="sxs-lookup"><span data-stu-id="35373-177">Type</span></span>|<span data-ttu-id="35373-178">説明</span><span class="sxs-lookup"><span data-stu-id="35373-178">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35373-179">apps</span><span class="sxs-lookup"><span data-stu-id="35373-179">apps</span></span>|<span data-ttu-id="35373-180">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="35373-180">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="35373-181">ポリシーが配置されたアプリのリスト。</span><span class="sxs-lookup"><span data-stu-id="35373-181">List of apps to which the policy is deployed.</span></span>|
|<span data-ttu-id="35373-182">deploymentSummary</span><span class="sxs-lookup"><span data-stu-id="35373-182">deploymentSummary</span></span>|[<span data-ttu-id="35373-183">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="35373-183">managedAppPolicyDeploymentSummary</span></span>](../resources/intune-mam-managedapppolicydeploymentsummary.md)|<span data-ttu-id="35373-184">構成の展開概要のナビゲーション プロパティ。</span><span class="sxs-lookup"><span data-stu-id="35373-184">Navigation property to deployment summary of the configuration.</span></span>|
|<span data-ttu-id="35373-185">assignments</span><span class="sxs-lookup"><span data-stu-id="35373-185">assignments</span></span>|<span data-ttu-id="35373-186">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="35373-186">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="35373-187">ポリシーが配置される包含グループと除外グループのリストのナビゲーション プロパティです。</span><span class="sxs-lookup"><span data-stu-id="35373-187">Navigation property to list of inclusion and exclusion groups to which the policy is deployed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="35373-188">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="35373-188">JSON Representation</span></span>
<span data-ttu-id="35373-189">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="35373-189">Here is a JSON representation of the resource.</span></span>
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
  "roleScopeTagIds": [
    "String"
  ],
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




