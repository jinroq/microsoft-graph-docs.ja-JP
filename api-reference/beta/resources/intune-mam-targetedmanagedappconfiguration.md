---
title: targetedManagedAppConfiguration リソース タイプ
description: カスタム設定のセットをそのまま、ターゲット セキュリティ グループのすべてのユーザーに提供するために使用される構成
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 70a7d863b409d9447f42df49cd818787ab926c4f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940632"
---
# <a name="targetedmanagedappconfiguration-resource-type"></a><span data-ttu-id="88688-103">targetedManagedAppConfiguration リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="88688-103">targetedManagedAppConfiguration resource type</span></span>

> <span data-ttu-id="88688-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="88688-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88688-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="88688-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88688-106">カスタム設定のセットをそのまま、ターゲット セキュリティ グループのすべてのユーザーに提供するために使用される構成</span><span class="sxs-lookup"><span data-stu-id="88688-106">Configuration used to deliver a set of custom settings as-is to all users in the targeted security group</span></span>


<span data-ttu-id="88688-107">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="88688-107">Inherits from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="88688-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="88688-108">Methods</span></span>
|<span data-ttu-id="88688-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="88688-109">Method</span></span>|<span data-ttu-id="88688-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="88688-110">Return Type</span></span>|<span data-ttu-id="88688-111">説明</span><span class="sxs-lookup"><span data-stu-id="88688-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="88688-112">List targetedManagedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="88688-112">List targetedManagedAppConfigurations</span></span>](../api/intune-mam-targetedmanagedappconfiguration-list.md)|<span data-ttu-id="88688-113">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="88688-113">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) collection</span></span>|<span data-ttu-id="88688-114">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="88688-114">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="88688-115">Get targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="88688-115">Get targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-get.md)|[<span data-ttu-id="88688-116">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="88688-116">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="88688-117">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="88688-117">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="88688-118">Create targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="88688-118">Create targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-create.md)|[<span data-ttu-id="88688-119">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="88688-119">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="88688-120">新しい [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="88688-120">Create a new [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="88688-121">Delete targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="88688-121">Delete targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-delete.md)|<span data-ttu-id="88688-122">なし</span><span class="sxs-lookup"><span data-stu-id="88688-122">None</span></span>|<span data-ttu-id="88688-123">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="88688-123">Deletes a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>|
|[<span data-ttu-id="88688-124">Update targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="88688-124">Update targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-update.md)|[<span data-ttu-id="88688-125">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="88688-125">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="88688-126">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="88688-126">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="88688-127">assign action</span><span class="sxs-lookup"><span data-stu-id="88688-127">assign action</span></span>](../api/intune-mam-targetedmanagedappconfiguration-assign.md)|<span data-ttu-id="88688-128">None</span><span class="sxs-lookup"><span data-stu-id="88688-128">None</span></span>|<span data-ttu-id="88688-129">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="88688-129">Not yet documented</span></span>|
|[<span data-ttu-id="88688-130">targetApps action</span><span class="sxs-lookup"><span data-stu-id="88688-130">targetApps action</span></span>](../api/intune-mam-targetedmanagedappconfiguration-targetapps.md)|<span data-ttu-id="88688-131">None</span><span class="sxs-lookup"><span data-stu-id="88688-131">None</span></span>|<span data-ttu-id="88688-132">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="88688-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="88688-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="88688-133">Properties</span></span>
|<span data-ttu-id="88688-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="88688-134">Property</span></span>|<span data-ttu-id="88688-135">種類</span><span class="sxs-lookup"><span data-stu-id="88688-135">Type</span></span>|<span data-ttu-id="88688-136">説明</span><span class="sxs-lookup"><span data-stu-id="88688-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88688-137">displayName</span><span class="sxs-lookup"><span data-stu-id="88688-137">displayName</span></span>|<span data-ttu-id="88688-138">String</span><span class="sxs-lookup"><span data-stu-id="88688-138">String</span></span>|<span data-ttu-id="88688-139">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="88688-139">Policy display name.</span></span> <span data-ttu-id="88688-140">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="88688-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="88688-141">description</span><span class="sxs-lookup"><span data-stu-id="88688-141">description</span></span>|<span data-ttu-id="88688-142">String</span><span class="sxs-lookup"><span data-stu-id="88688-142">String</span></span>|<span data-ttu-id="88688-143">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="88688-143">The policy's description.</span></span> <span data-ttu-id="88688-144">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="88688-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="88688-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="88688-145">createdDateTime</span></span>|<span data-ttu-id="88688-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88688-146">DateTimeOffset</span></span>|<span data-ttu-id="88688-147">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="88688-147">The date and time the policy was created.</span></span> <span data-ttu-id="88688-148">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="88688-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="88688-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="88688-149">lastModifiedDateTime</span></span>|<span data-ttu-id="88688-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88688-150">DateTimeOffset</span></span>|<span data-ttu-id="88688-151">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="88688-151">Last time the policy was modified.</span></span> <span data-ttu-id="88688-152">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="88688-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="88688-153">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="88688-153">roleScopeTagIds</span></span>|<span data-ttu-id="88688-154">String collection</span><span class="sxs-lookup"><span data-stu-id="88688-154">String collection</span></span>|<span data-ttu-id="88688-155">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="88688-155">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="88688-156">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="88688-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="88688-157">id</span><span class="sxs-lookup"><span data-stu-id="88688-157">id</span></span>|<span data-ttu-id="88688-158">文字列</span><span class="sxs-lookup"><span data-stu-id="88688-158">String</span></span>|<span data-ttu-id="88688-159">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="88688-159">Key of the entity.</span></span> <span data-ttu-id="88688-160">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="88688-160">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="88688-161">version</span><span class="sxs-lookup"><span data-stu-id="88688-161">version</span></span>|<span data-ttu-id="88688-162">String</span><span class="sxs-lookup"><span data-stu-id="88688-162">String</span></span>|<span data-ttu-id="88688-163">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="88688-163">Version of the entity.</span></span> <span data-ttu-id="88688-164">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="88688-164">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="88688-165">customSettings</span><span class="sxs-lookup"><span data-stu-id="88688-165">customSettings</span></span>|<span data-ttu-id="88688-166">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="88688-166">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="88688-167">構成の対象であるユーザーに対して、このサービスで変更せずにアプリに送信される文字列キーと文字列値の一連のペア。[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="88688-167">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="88688-168">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="88688-168">deployedAppCount</span></span>|<span data-ttu-id="88688-169">Int32</span><span class="sxs-lookup"><span data-stu-id="88688-169">Int32</span></span>|<span data-ttu-id="88688-170">現在のポリシーが配置されたアプリの数。</span><span class="sxs-lookup"><span data-stu-id="88688-170">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="88688-171">isAssigned</span><span class="sxs-lookup"><span data-stu-id="88688-171">isAssigned</span></span>|<span data-ttu-id="88688-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="88688-172">Boolean</span></span>|<span data-ttu-id="88688-173">包含グループにポリシーを配置するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="88688-173">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="88688-174">関係</span><span class="sxs-lookup"><span data-stu-id="88688-174">Relationships</span></span>
|<span data-ttu-id="88688-175">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="88688-175">Relationship</span></span>|<span data-ttu-id="88688-176">型</span><span class="sxs-lookup"><span data-stu-id="88688-176">Type</span></span>|<span data-ttu-id="88688-177">説明</span><span class="sxs-lookup"><span data-stu-id="88688-177">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88688-178">apps</span><span class="sxs-lookup"><span data-stu-id="88688-178">apps</span></span>|<span data-ttu-id="88688-179">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="88688-179">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="88688-180">ポリシーが配置されたアプリのリスト。</span><span class="sxs-lookup"><span data-stu-id="88688-180">List of apps to which the policy is deployed.</span></span>|
|<span data-ttu-id="88688-181">deploymentSummary</span><span class="sxs-lookup"><span data-stu-id="88688-181">deploymentSummary</span></span>|[<span data-ttu-id="88688-182">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="88688-182">managedAppPolicyDeploymentSummary</span></span>](../resources/intune-mam-managedapppolicydeploymentsummary.md)|<span data-ttu-id="88688-183">構成の展開概要のナビゲーション プロパティ。</span><span class="sxs-lookup"><span data-stu-id="88688-183">Navigation property to deployment summary of the configuration.</span></span>|
|<span data-ttu-id="88688-184">assignments</span><span class="sxs-lookup"><span data-stu-id="88688-184">assignments</span></span>|<span data-ttu-id="88688-185">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="88688-185">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="88688-186">ポリシーが配置される包含グループと除外グループのリストのナビゲーション プロパティです。</span><span class="sxs-lookup"><span data-stu-id="88688-186">Navigation property to list of inclusion and exclusion groups to which the policy is deployed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="88688-187">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="88688-187">JSON Representation</span></span>
<span data-ttu-id="88688-188">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="88688-188">Here is a JSON representation of the resource.</span></span>
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




