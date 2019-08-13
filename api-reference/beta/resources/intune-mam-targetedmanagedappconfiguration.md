---
title: targetedManagedAppConfiguration リソース タイプ
description: カスタム設定のセットをそのまま、ターゲット セキュリティ グループのすべてのユーザーに提供するために使用される構成
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d7949f1aa4931f9ec08b5bb17a5452ac8e8e383a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373631"
---
# <a name="targetedmanagedappconfiguration-resource-type"></a><span data-ttu-id="ca47e-103">targetedManagedAppConfiguration リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="ca47e-103">targetedManagedAppConfiguration resource type</span></span>

> <span data-ttu-id="ca47e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ca47e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca47e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ca47e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca47e-106">カスタム設定のセットをそのまま、ターゲット セキュリティ グループのすべてのユーザーに提供するために使用される構成</span><span class="sxs-lookup"><span data-stu-id="ca47e-106">Configuration used to deliver a set of custom settings as-is to all users in the targeted security group</span></span>


<span data-ttu-id="ca47e-107">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ca47e-107">Inherits from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="ca47e-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="ca47e-108">Methods</span></span>
|<span data-ttu-id="ca47e-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="ca47e-109">Method</span></span>|<span data-ttu-id="ca47e-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ca47e-110">Return Type</span></span>|<span data-ttu-id="ca47e-111">説明</span><span class="sxs-lookup"><span data-stu-id="ca47e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ca47e-112">List targetedManagedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="ca47e-112">List targetedManagedAppConfigurations</span></span>](../api/intune-mam-targetedmanagedappconfiguration-list.md)|<span data-ttu-id="ca47e-113">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ca47e-113">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) collection</span></span>|<span data-ttu-id="ca47e-114">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="ca47e-114">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="ca47e-115">Get targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="ca47e-115">Get targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-get.md)|[<span data-ttu-id="ca47e-116">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="ca47e-116">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="ca47e-117">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ca47e-117">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="ca47e-118">Create targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="ca47e-118">Create targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-create.md)|[<span data-ttu-id="ca47e-119">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="ca47e-119">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="ca47e-120">新しい [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ca47e-120">Create a new [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="ca47e-121">Delete targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="ca47e-121">Delete targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-delete.md)|<span data-ttu-id="ca47e-122">なし</span><span class="sxs-lookup"><span data-stu-id="ca47e-122">None</span></span>|<span data-ttu-id="ca47e-123">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="ca47e-123">Deletes a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>|
|[<span data-ttu-id="ca47e-124">Update targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="ca47e-124">Update targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-update.md)|[<span data-ttu-id="ca47e-125">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="ca47e-125">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="ca47e-126">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ca47e-126">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="ca47e-127">assign action</span><span class="sxs-lookup"><span data-stu-id="ca47e-127">assign action</span></span>](../api/intune-mam-targetedmanagedappconfiguration-assign.md)|<span data-ttu-id="ca47e-128">None</span><span class="sxs-lookup"><span data-stu-id="ca47e-128">None</span></span>|<span data-ttu-id="ca47e-129">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ca47e-129">Not yet documented</span></span>|
|[<span data-ttu-id="ca47e-130">targetApps action</span><span class="sxs-lookup"><span data-stu-id="ca47e-130">targetApps action</span></span>](../api/intune-mam-targetedmanagedappconfiguration-targetapps.md)|<span data-ttu-id="ca47e-131">None</span><span class="sxs-lookup"><span data-stu-id="ca47e-131">None</span></span>|<span data-ttu-id="ca47e-132">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ca47e-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="ca47e-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ca47e-133">Properties</span></span>
|<span data-ttu-id="ca47e-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ca47e-134">Property</span></span>|<span data-ttu-id="ca47e-135">型</span><span class="sxs-lookup"><span data-stu-id="ca47e-135">Type</span></span>|<span data-ttu-id="ca47e-136">説明</span><span class="sxs-lookup"><span data-stu-id="ca47e-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca47e-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ca47e-137">displayName</span></span>|<span data-ttu-id="ca47e-138">String</span><span class="sxs-lookup"><span data-stu-id="ca47e-138">String</span></span>|<span data-ttu-id="ca47e-139">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="ca47e-139">Policy display name.</span></span> <span data-ttu-id="ca47e-140">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ca47e-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ca47e-141">description</span><span class="sxs-lookup"><span data-stu-id="ca47e-141">description</span></span>|<span data-ttu-id="ca47e-142">String</span><span class="sxs-lookup"><span data-stu-id="ca47e-142">String</span></span>|<span data-ttu-id="ca47e-143">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="ca47e-143">The policy's description.</span></span> <span data-ttu-id="ca47e-144">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ca47e-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ca47e-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ca47e-145">createdDateTime</span></span>|<span data-ttu-id="ca47e-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca47e-146">DateTimeOffset</span></span>|<span data-ttu-id="ca47e-147">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="ca47e-147">The date and time the policy was created.</span></span> <span data-ttu-id="ca47e-148">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ca47e-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ca47e-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ca47e-149">lastModifiedDateTime</span></span>|<span data-ttu-id="ca47e-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca47e-150">DateTimeOffset</span></span>|<span data-ttu-id="ca47e-151">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="ca47e-151">Last time the policy was modified.</span></span> <span data-ttu-id="ca47e-152">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ca47e-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ca47e-153">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ca47e-153">roleScopeTagIds</span></span>|<span data-ttu-id="ca47e-154">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="ca47e-154">String collection</span></span>|<span data-ttu-id="ca47e-155">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="ca47e-155">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ca47e-156">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ca47e-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ca47e-157">id</span><span class="sxs-lookup"><span data-stu-id="ca47e-157">id</span></span>|<span data-ttu-id="ca47e-158">文字列</span><span class="sxs-lookup"><span data-stu-id="ca47e-158">String</span></span>|<span data-ttu-id="ca47e-159">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ca47e-159">Key of the entity.</span></span> <span data-ttu-id="ca47e-160">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ca47e-160">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ca47e-161">version</span><span class="sxs-lookup"><span data-stu-id="ca47e-161">version</span></span>|<span data-ttu-id="ca47e-162">String</span><span class="sxs-lookup"><span data-stu-id="ca47e-162">String</span></span>|<span data-ttu-id="ca47e-163">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="ca47e-163">Version of the entity.</span></span> <span data-ttu-id="ca47e-164">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ca47e-164">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ca47e-165">customSettings</span><span class="sxs-lookup"><span data-stu-id="ca47e-165">customSettings</span></span>|<span data-ttu-id="ca47e-166">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ca47e-166">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="ca47e-167">構成の対象であるユーザーに対して、このサービスで変更せずにアプリに送信される文字列キーと文字列値の一連のペア。[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ca47e-167">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="ca47e-168">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="ca47e-168">deployedAppCount</span></span>|<span data-ttu-id="ca47e-169">Int32</span><span class="sxs-lookup"><span data-stu-id="ca47e-169">Int32</span></span>|<span data-ttu-id="ca47e-170">現在のポリシーが配置されたアプリの数。</span><span class="sxs-lookup"><span data-stu-id="ca47e-170">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="ca47e-171">isAssigned</span><span class="sxs-lookup"><span data-stu-id="ca47e-171">isAssigned</span></span>|<span data-ttu-id="ca47e-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca47e-172">Boolean</span></span>|<span data-ttu-id="ca47e-173">包含グループにポリシーを配置するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ca47e-173">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ca47e-174">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ca47e-174">Relationships</span></span>
|<span data-ttu-id="ca47e-175">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ca47e-175">Relationship</span></span>|<span data-ttu-id="ca47e-176">型</span><span class="sxs-lookup"><span data-stu-id="ca47e-176">Type</span></span>|<span data-ttu-id="ca47e-177">説明</span><span class="sxs-lookup"><span data-stu-id="ca47e-177">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca47e-178">apps</span><span class="sxs-lookup"><span data-stu-id="ca47e-178">apps</span></span>|<span data-ttu-id="ca47e-179">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ca47e-179">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="ca47e-180">ポリシーが配置されたアプリのリスト。</span><span class="sxs-lookup"><span data-stu-id="ca47e-180">List of apps to which the policy is deployed.</span></span>|
|<span data-ttu-id="ca47e-181">deploymentSummary</span><span class="sxs-lookup"><span data-stu-id="ca47e-181">deploymentSummary</span></span>|[<span data-ttu-id="ca47e-182">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="ca47e-182">managedAppPolicyDeploymentSummary</span></span>](../resources/intune-mam-managedapppolicydeploymentsummary.md)|<span data-ttu-id="ca47e-183">構成の展開概要のナビゲーション プロパティ。</span><span class="sxs-lookup"><span data-stu-id="ca47e-183">Navigation property to deployment summary of the configuration.</span></span>|
|<span data-ttu-id="ca47e-184">assignments</span><span class="sxs-lookup"><span data-stu-id="ca47e-184">assignments</span></span>|<span data-ttu-id="ca47e-185">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ca47e-185">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="ca47e-186">ポリシーが配置される包含グループと除外グループのリストのナビゲーション プロパティです。</span><span class="sxs-lookup"><span data-stu-id="ca47e-186">Navigation property to list of inclusion and exclusion groups to which the policy is deployed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ca47e-187">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ca47e-187">JSON Representation</span></span>
<span data-ttu-id="ca47e-188">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ca47e-188">Here is a JSON representation of the resource.</span></span>
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



