---
title: targetedManagedAppConfiguration リソース タイプ
description: カスタム設定のセットをそのまま、ターゲット セキュリティ グループのすべてのユーザーに提供するために使用される構成
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6adafe694a7abb55cd64a5fbfbd64e3c66b7e6e4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149239"
---
# <a name="targetedmanagedappconfiguration-resource-type"></a><span data-ttu-id="7e394-103">targetedManagedAppConfiguration リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="7e394-103">targetedManagedAppConfiguration resource type</span></span>

> <span data-ttu-id="7e394-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e394-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e394-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7e394-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e394-106">カスタム設定のセットをそのまま、ターゲット セキュリティ グループのすべてのユーザーに提供するために使用される構成</span><span class="sxs-lookup"><span data-stu-id="7e394-106">Configuration used to deliver a set of custom settings as-is to all users in the targeted security group</span></span>


<span data-ttu-id="7e394-107">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e394-107">Inherits from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="7e394-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="7e394-108">Methods</span></span>
|<span data-ttu-id="7e394-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="7e394-109">Method</span></span>|<span data-ttu-id="7e394-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7e394-110">Return Type</span></span>|<span data-ttu-id="7e394-111">説明</span><span class="sxs-lookup"><span data-stu-id="7e394-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7e394-112">List targetedManagedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="7e394-112">List targetedManagedAppConfigurations</span></span>](../api/intune-mam-targetedmanagedappconfiguration-list.md)|<span data-ttu-id="7e394-113">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7e394-113">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) collection</span></span>|<span data-ttu-id="7e394-114">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="7e394-114">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="7e394-115">Get targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="7e394-115">Get targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-get.md)|[<span data-ttu-id="7e394-116">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="7e394-116">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="7e394-117">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7e394-117">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="7e394-118">Create targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="7e394-118">Create targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-create.md)|[<span data-ttu-id="7e394-119">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="7e394-119">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="7e394-120">新しい [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7e394-120">Create a new [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="7e394-121">Delete targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="7e394-121">Delete targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-delete.md)|<span data-ttu-id="7e394-122">なし</span><span class="sxs-lookup"><span data-stu-id="7e394-122">None</span></span>|<span data-ttu-id="7e394-123">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="7e394-123">Deletes a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>|
|[<span data-ttu-id="7e394-124">Update targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="7e394-124">Update targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-update.md)|[<span data-ttu-id="7e394-125">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="7e394-125">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="7e394-126">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7e394-126">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="7e394-127">assign action</span><span class="sxs-lookup"><span data-stu-id="7e394-127">assign action</span></span>](../api/intune-mam-targetedmanagedappconfiguration-assign.md)|<span data-ttu-id="7e394-128">なし</span><span class="sxs-lookup"><span data-stu-id="7e394-128">None</span></span>|<span data-ttu-id="7e394-129">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="7e394-129">Not yet documented</span></span>|
|[<span data-ttu-id="7e394-130">targetApps action</span><span class="sxs-lookup"><span data-stu-id="7e394-130">targetApps action</span></span>](../api/intune-mam-targetedmanagedappconfiguration-targetapps.md)|<span data-ttu-id="7e394-131">なし</span><span class="sxs-lookup"><span data-stu-id="7e394-131">None</span></span>|<span data-ttu-id="7e394-132">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="7e394-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="7e394-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7e394-133">Properties</span></span>
|<span data-ttu-id="7e394-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7e394-134">Property</span></span>|<span data-ttu-id="7e394-135">型</span><span class="sxs-lookup"><span data-stu-id="7e394-135">Type</span></span>|<span data-ttu-id="7e394-136">説明</span><span class="sxs-lookup"><span data-stu-id="7e394-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e394-137">displayName</span><span class="sxs-lookup"><span data-stu-id="7e394-137">displayName</span></span>|<span data-ttu-id="7e394-138">String</span><span class="sxs-lookup"><span data-stu-id="7e394-138">String</span></span>|<span data-ttu-id="7e394-139">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="7e394-139">Policy display name.</span></span> <span data-ttu-id="7e394-140">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e394-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7e394-141">説明</span><span class="sxs-lookup"><span data-stu-id="7e394-141">description</span></span>|<span data-ttu-id="7e394-142">String</span><span class="sxs-lookup"><span data-stu-id="7e394-142">String</span></span>|<span data-ttu-id="7e394-143">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="7e394-143">The policy's description.</span></span> <span data-ttu-id="7e394-144">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e394-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7e394-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7e394-145">createdDateTime</span></span>|<span data-ttu-id="7e394-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e394-146">DateTimeOffset</span></span>|<span data-ttu-id="7e394-147">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="7e394-147">The date and time the policy was created.</span></span> <span data-ttu-id="7e394-148">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e394-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7e394-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7e394-149">lastModifiedDateTime</span></span>|<span data-ttu-id="7e394-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e394-150">DateTimeOffset</span></span>|<span data-ttu-id="7e394-151">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="7e394-151">Last time the policy was modified.</span></span> <span data-ttu-id="7e394-152">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e394-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7e394-153">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7e394-153">roleScopeTagIds</span></span>|<span data-ttu-id="7e394-154">String コレクション</span><span class="sxs-lookup"><span data-stu-id="7e394-154">String collection</span></span>|<span data-ttu-id="7e394-155">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="7e394-155">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7e394-156">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e394-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7e394-157">id</span><span class="sxs-lookup"><span data-stu-id="7e394-157">id</span></span>|<span data-ttu-id="7e394-158">文字列</span><span class="sxs-lookup"><span data-stu-id="7e394-158">String</span></span>|<span data-ttu-id="7e394-159">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7e394-159">Key of the entity.</span></span> <span data-ttu-id="7e394-160">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e394-160">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7e394-161">version</span><span class="sxs-lookup"><span data-stu-id="7e394-161">version</span></span>|<span data-ttu-id="7e394-162">String</span><span class="sxs-lookup"><span data-stu-id="7e394-162">String</span></span>|<span data-ttu-id="7e394-163">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="7e394-163">Version of the entity.</span></span> <span data-ttu-id="7e394-164">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e394-164">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7e394-165">customSettings</span><span class="sxs-lookup"><span data-stu-id="7e394-165">customSettings</span></span>|<span data-ttu-id="7e394-166">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7e394-166">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="7e394-167">構成の対象であるユーザーに対して、このサービスで変更せずにアプリに送信される文字列キーと文字列値の一連のペア。[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e394-167">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="7e394-168">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="7e394-168">deployedAppCount</span></span>|<span data-ttu-id="7e394-169">Int32</span><span class="sxs-lookup"><span data-stu-id="7e394-169">Int32</span></span>|<span data-ttu-id="7e394-170">現在のポリシーが配置されたアプリの数。</span><span class="sxs-lookup"><span data-stu-id="7e394-170">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="7e394-171">isAssigned</span><span class="sxs-lookup"><span data-stu-id="7e394-171">isAssigned</span></span>|<span data-ttu-id="7e394-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e394-172">Boolean</span></span>|<span data-ttu-id="7e394-173">包含グループにポリシーを配置するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7e394-173">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e394-174">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7e394-174">Relationships</span></span>
|<span data-ttu-id="7e394-175">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7e394-175">Relationship</span></span>|<span data-ttu-id="7e394-176">型</span><span class="sxs-lookup"><span data-stu-id="7e394-176">Type</span></span>|<span data-ttu-id="7e394-177">説明</span><span class="sxs-lookup"><span data-stu-id="7e394-177">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e394-178">apps</span><span class="sxs-lookup"><span data-stu-id="7e394-178">apps</span></span>|<span data-ttu-id="7e394-179">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7e394-179">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="7e394-180">ポリシーが配置されたアプリのリスト。</span><span class="sxs-lookup"><span data-stu-id="7e394-180">List of apps to which the policy is deployed.</span></span>|
|<span data-ttu-id="7e394-181">deploymentSummary</span><span class="sxs-lookup"><span data-stu-id="7e394-181">deploymentSummary</span></span>|[<span data-ttu-id="7e394-182">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="7e394-182">managedAppPolicyDeploymentSummary</span></span>](../resources/intune-mam-managedapppolicydeploymentsummary.md)|<span data-ttu-id="7e394-183">構成の展開概要のナビゲーション プロパティ。</span><span class="sxs-lookup"><span data-stu-id="7e394-183">Navigation property to deployment summary of the configuration.</span></span>|
|<span data-ttu-id="7e394-184">assignments</span><span class="sxs-lookup"><span data-stu-id="7e394-184">assignments</span></span>|<span data-ttu-id="7e394-185">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7e394-185">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="7e394-186">ポリシーが配置される包含グループと除外グループのリストのナビゲーション プロパティです。</span><span class="sxs-lookup"><span data-stu-id="7e394-186">Navigation property to list of inclusion and exclusion groups to which the policy is deployed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7e394-187">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7e394-187">JSON Representation</span></span>
<span data-ttu-id="7e394-188">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7e394-188">Here is a JSON representation of the resource.</span></span>
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




