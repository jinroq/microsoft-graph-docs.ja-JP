---
title: sharedPCConfiguration リソース タイプ
description: このトピックでは、sharedPCConfiguration リソースによって公開された、宣言されたメソッド、プロパティ、リレーションシップについて説明します。
ms.openlocfilehash: fec817184ed5027904b4afebcf867f45b2ac7808
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068112"
---
# <a name="sharedpcconfiguration-resource-type"></a><span data-ttu-id="3dec1-103">sharedPCConfiguration リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="3dec1-103">sharedPCConfiguration resource type</span></span>

> <span data-ttu-id="3dec1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3dec1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3dec1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3dec1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3dec1-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3dec1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3dec1-107">このトピックでは、sharedPCConfiguration リソースによって公開された、宣言されたメソッド、プロパティ、リレーションシップについて説明します。</span><span class="sxs-lookup"><span data-stu-id="3dec1-107">This topic provides descriptions of the declared methods, properties and relationships exposed by the sharedPCConfiguration resource.</span></span>

<span data-ttu-id="3dec1-108">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3dec1-108">Inherits from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="3dec1-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="3dec1-109">Methods</span></span>
|<span data-ttu-id="3dec1-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="3dec1-110">Method</span></span>|<span data-ttu-id="3dec1-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3dec1-111">Return Type</span></span>|<span data-ttu-id="3dec1-112">説明</span><span class="sxs-lookup"><span data-stu-id="3dec1-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3dec1-113">List sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="3dec1-113">List sharedPCConfigurations</span></span>](../api/intune-deviceconfig-sharedpcconfiguration-list.md)|<span data-ttu-id="3dec1-114">[sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="3dec1-114">[sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) collection</span></span>|<span data-ttu-id="3dec1-115">[sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="3dec1-115">List properties and relationships of the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="3dec1-116">Get sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="3dec1-116">Get sharedPCConfiguration</span></span>](../api/intune-deviceconfig-sharedpcconfiguration-get.md)|[<span data-ttu-id="3dec1-117">sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="3dec1-117">sharedPCConfiguration</span></span>](../resources/intune-deviceconfig-sharedpcconfiguration.md)|<span data-ttu-id="3dec1-118">[sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="3dec1-118">Read properties and relationships of the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>|
|[<span data-ttu-id="3dec1-119">Create sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="3dec1-119">Create sharedPCConfiguration</span></span>](../api/intune-deviceconfig-sharedpcconfiguration-create.md)|[<span data-ttu-id="3dec1-120">sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="3dec1-120">sharedPCConfiguration</span></span>](../resources/intune-deviceconfig-sharedpcconfiguration.md)|<span data-ttu-id="3dec1-121">新しい [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="3dec1-121">Create a new [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>|
|[<span data-ttu-id="3dec1-122">Delete sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="3dec1-122">Delete sharedPCConfiguration</span></span>](../api/intune-deviceconfig-sharedpcconfiguration-delete.md)|<span data-ttu-id="3dec1-123">なし</span><span class="sxs-lookup"><span data-stu-id="3dec1-123">None</span></span>|<span data-ttu-id="3dec1-124">[sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="3dec1-124">Deletes a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span></span>|
|[<span data-ttu-id="3dec1-125">Update sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="3dec1-125">Update sharedPCConfiguration</span></span>](../api/intune-deviceconfig-sharedpcconfiguration-update.md)|[<span data-ttu-id="3dec1-126">sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="3dec1-126">sharedPCConfiguration</span></span>](../resources/intune-deviceconfig-sharedpcconfiguration.md)|<span data-ttu-id="3dec1-127">[sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3dec1-127">Update the properties of a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3dec1-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3dec1-128">Properties</span></span>
|<span data-ttu-id="3dec1-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3dec1-129">Property</span></span>|<span data-ttu-id="3dec1-130">型</span><span class="sxs-lookup"><span data-stu-id="3dec1-130">Type</span></span>|<span data-ttu-id="3dec1-131">説明</span><span class="sxs-lookup"><span data-stu-id="3dec1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3dec1-132">id</span><span class="sxs-lookup"><span data-stu-id="3dec1-132">id</span></span>|<span data-ttu-id="3dec1-133">String</span><span class="sxs-lookup"><span data-stu-id="3dec1-133">String</span></span>|<span data-ttu-id="3dec1-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="3dec1-134">Key of the entity.</span></span> <span data-ttu-id="3dec1-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3dec1-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dec1-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3dec1-136">lastModifiedDateTime</span></span>|<span data-ttu-id="3dec1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3dec1-137">DateTimeOffset</span></span>|<span data-ttu-id="3dec1-138">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="3dec1-138">DateTime the object was last modified.</span></span> <span data-ttu-id="3dec1-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3dec1-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dec1-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3dec1-140">roleScopeTagIds</span></span>|<span data-ttu-id="3dec1-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="3dec1-141">String collection</span></span>|<span data-ttu-id="3dec1-142">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="3dec1-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3dec1-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3dec1-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dec1-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3dec1-144">supportsScopeTags</span></span>|<span data-ttu-id="3dec1-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dec1-145">Boolean</span></span>|<span data-ttu-id="3dec1-146">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3dec1-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3dec1-147">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="3dec1-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3dec1-148">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="3dec1-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3dec1-149">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="3dec1-149">This property is read-only.</span></span> <span data-ttu-id="3dec1-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3dec1-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dec1-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3dec1-151">createdDateTime</span></span>|<span data-ttu-id="3dec1-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3dec1-152">DateTimeOffset</span></span>|<span data-ttu-id="3dec1-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="3dec1-153">DateTime the object was created.</span></span> <span data-ttu-id="3dec1-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3dec1-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dec1-155">説明</span><span class="sxs-lookup"><span data-stu-id="3dec1-155">description</span></span>|<span data-ttu-id="3dec1-156">String</span><span class="sxs-lookup"><span data-stu-id="3dec1-156">String</span></span>|<span data-ttu-id="3dec1-157">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="3dec1-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3dec1-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3dec1-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dec1-159">displayName</span><span class="sxs-lookup"><span data-stu-id="3dec1-159">displayName</span></span>|<span data-ttu-id="3dec1-160">String</span><span class="sxs-lookup"><span data-stu-id="3dec1-160">String</span></span>|<span data-ttu-id="3dec1-161">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="3dec1-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3dec1-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3dec1-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dec1-163">version</span><span class="sxs-lookup"><span data-stu-id="3dec1-163">version</span></span>|<span data-ttu-id="3dec1-164">Int32</span><span class="sxs-lookup"><span data-stu-id="3dec1-164">Int32</span></span>|<span data-ttu-id="3dec1-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="3dec1-165">Version of the device configuration.</span></span> <span data-ttu-id="3dec1-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3dec1-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dec1-167">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="3dec1-167">accountManagerPolicy</span></span>|[<span data-ttu-id="3dec1-168">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="3dec1-168">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="3dec1-169">共有の PC 上でアカウントを管理する方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="3dec1-169">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="3dec1-170">disableAccountManager が false の場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="3dec1-170">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="3dec1-171">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="3dec1-171">allowedAccounts</span></span>|[<span data-ttu-id="3dec1-172">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="3dec1-172">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="3dec1-173">共有の PC で使用できるアカウントの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="3dec1-173">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="3dec1-174">可能な値は、`guest`、`domain` です。</span><span class="sxs-lookup"><span data-stu-id="3dec1-174">Possible values are: `guest`, `domain`.</span></span>|
|<span data-ttu-id="3dec1-175">localStorage</span><span class="sxs-lookup"><span data-stu-id="3dec1-175">localStorage</span></span>|[<span data-ttu-id="3dec1-176">有効化</span><span class="sxs-lookup"><span data-stu-id="3dec1-176">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="3dec1-177">共有の PC でローカル ストレージを許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="3dec1-177">Specifies whether local storage is allowed on a shared PC.</span></span> <span data-ttu-id="3dec1-178">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="3dec1-178">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="3dec1-179">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="3dec1-179">allowLocalStorage</span></span>|<span data-ttu-id="3dec1-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dec1-180">Boolean</span></span>|<span data-ttu-id="3dec1-181">共有の PC でローカル ストレージを許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="3dec1-181">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="3dec1-182">setAccountManager</span><span class="sxs-lookup"><span data-stu-id="3dec1-182">setAccountManager</span></span>|[<span data-ttu-id="3dec1-183">有効化</span><span class="sxs-lookup"><span data-stu-id="3dec1-183">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="3dec1-184">共有 PC モードのアカウント マネージャーを無効にします。</span><span class="sxs-lookup"><span data-stu-id="3dec1-184">Disables the account manager for shared PC mode.</span></span> <span data-ttu-id="3dec1-185">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="3dec1-185">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="3dec1-186">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="3dec1-186">disableAccountManager</span></span>|<span data-ttu-id="3dec1-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dec1-187">Boolean</span></span>|<span data-ttu-id="3dec1-188">共有 PC モードのアカウント マネージャーを無効にします。</span><span class="sxs-lookup"><span data-stu-id="3dec1-188">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="3dec1-189">setEduPolicies</span><span class="sxs-lookup"><span data-stu-id="3dec1-189">setEduPolicies</span></span>|[<span data-ttu-id="3dec1-190">有効化</span><span class="sxs-lookup"><span data-stu-id="3dec1-190">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="3dec1-191">PC 教育環境の既定の共有ポリシー構成かどうか、有効、無効としないことを指定します。</span><span class="sxs-lookup"><span data-stu-id="3dec1-191">Specifies whether the default shared PC education environment policies should be enabled/disabled/not configured.</span></span> <span data-ttu-id="3dec1-192">Windows 10 RS2 以降では、このポリシーは Enabled を true に設定しなくても適用されます。</span><span class="sxs-lookup"><span data-stu-id="3dec1-192">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span> <span data-ttu-id="3dec1-193">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="3dec1-193">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="3dec1-194">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="3dec1-194">disableEduPolicies</span></span>|<span data-ttu-id="3dec1-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dec1-195">Boolean</span></span>|<span data-ttu-id="3dec1-196">既定の共有 PC 教育環境ポリシーを無効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="3dec1-196">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="3dec1-197">Windows 10 RS2 以降では、このポリシーは Enabled を true に設定しなくても適用されます。</span><span class="sxs-lookup"><span data-stu-id="3dec1-197">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="3dec1-198">setPowerPolicies</span><span class="sxs-lookup"><span data-stu-id="3dec1-198">setPowerPolicies</span></span>|[<span data-ttu-id="3dec1-199">有効化</span><span class="sxs-lookup"><span data-stu-id="3dec1-199">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="3dec1-200">かどうか既定の共有の PC の電源ポリシーが有効または無効にするを指定します。</span><span class="sxs-lookup"><span data-stu-id="3dec1-200">Specifies whether the default shared PC power policies should be enabled/disabled.</span></span> <span data-ttu-id="3dec1-201">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="3dec1-201">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="3dec1-202">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="3dec1-202">disablePowerPolicies</span></span>|<span data-ttu-id="3dec1-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dec1-203">Boolean</span></span>|<span data-ttu-id="3dec1-204">既定の共有 PC 電源ポリシーを無効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="3dec1-204">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="3dec1-205">signInOnResume</span><span class="sxs-lookup"><span data-stu-id="3dec1-205">signInOnResume</span></span>|[<span data-ttu-id="3dec1-206">有効化</span><span class="sxs-lookup"><span data-stu-id="3dec1-206">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="3dec1-207">署名するための要件を指定のときに、デバイスのスリープ状態スリープ モードから。</span><span class="sxs-lookup"><span data-stu-id="3dec1-207">Specifies the requirement to sign in whenever the device wakes up from sleep mode.</span></span> <span data-ttu-id="3dec1-208">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="3dec1-208">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="3dec1-209">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="3dec1-209">disableSignInOnResume</span></span>|<span data-ttu-id="3dec1-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dec1-210">Boolean</span></span>|<span data-ttu-id="3dec1-211">デバイスがスリープ モードから再開するたびにサインインを求める設定を無効にします。</span><span class="sxs-lookup"><span data-stu-id="3dec1-211">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="3dec1-212">enabled</span><span class="sxs-lookup"><span data-stu-id="3dec1-212">enabled</span></span>|<span data-ttu-id="3dec1-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dec1-213">Boolean</span></span>|<span data-ttu-id="3dec1-214">共有 PC モードを有効にし、共有 PC のポリシーを適用します。</span><span class="sxs-lookup"><span data-stu-id="3dec1-214">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="3dec1-215">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="3dec1-215">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="3dec1-216">Int32</span><span class="sxs-lookup"><span data-stu-id="3dec1-216">Int32</span></span>|<span data-ttu-id="3dec1-217">PC がスリープ状態になるまでにデバイスがアイドル状態を続ける時間を秒単位で指定します。</span><span class="sxs-lookup"><span data-stu-id="3dec1-217">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="3dec1-218">この値を 0 に設定すると、スリープ タイムアウトは発生しなくなります。</span><span class="sxs-lookup"><span data-stu-id="3dec1-218">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="3dec1-219">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="3dec1-219">kioskAppDisplayName</span></span>|<span data-ttu-id="3dec1-220">String</span><span class="sxs-lookup"><span data-stu-id="3dec1-220">String</span></span>|<span data-ttu-id="3dec1-221">SetKioskAppUserModelId で指定されたアプリを起動するサインイン画面に表示されるアカウントの表示テキストを指定します。</span><span class="sxs-lookup"><span data-stu-id="3dec1-221">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="3dec1-222">KioskAppUserModelId が設定されている場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="3dec1-222">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="3dec1-223">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="3dec1-223">kioskAppUserModelId</span></span>|<span data-ttu-id="3dec1-224">String</span><span class="sxs-lookup"><span data-stu-id="3dec1-224">String</span></span>|<span data-ttu-id="3dec1-225">割り当てられたアクセスで使用するアプリのアプリケーション ユーザー モデル ID を指定します。</span><span class="sxs-lookup"><span data-stu-id="3dec1-225">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="3dec1-226">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="3dec1-226">maintenanceStartTime</span></span>|<span data-ttu-id="3dec1-227">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="3dec1-227">TimeOfDay</span></span>|<span data-ttu-id="3dec1-228">毎日のメンテナンス時間の開始時刻を指定します。</span><span class="sxs-lookup"><span data-stu-id="3dec1-228">Specifies the daily start time of maintenance hour.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3dec1-229">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3dec1-229">Relationships</span></span>
|<span data-ttu-id="3dec1-230">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3dec1-230">Relationship</span></span>|<span data-ttu-id="3dec1-231">型</span><span class="sxs-lookup"><span data-stu-id="3dec1-231">Type</span></span>|<span data-ttu-id="3dec1-232">説明</span><span class="sxs-lookup"><span data-stu-id="3dec1-232">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3dec1-233">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="3dec1-233">groupAssignments</span></span>|<span data-ttu-id="3dec1-234">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="3dec1-234">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="3dec1-235">デバイスの構成プロファイルのグループ割り当てのリストです。</span><span class="sxs-lookup"><span data-stu-id="3dec1-235">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="3dec1-236">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3dec1-236">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dec1-237">assignments</span><span class="sxs-lookup"><span data-stu-id="3dec1-237">assignments</span></span>|<span data-ttu-id="3dec1-238">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="3dec1-238">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="3dec1-239">デバイスの構成プロファイルの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="3dec1-239">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="3dec1-240">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3dec1-240">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dec1-241">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="3dec1-241">deviceStatuses</span></span>|<span data-ttu-id="3dec1-242">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="3dec1-242">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="3dec1-243">デバイスごとのデバイス構成のインストール状況。</span><span class="sxs-lookup"><span data-stu-id="3dec1-243">Device configuration installation status by device.</span></span> <span data-ttu-id="3dec1-244">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3dec1-244">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dec1-245">userStatuses</span><span class="sxs-lookup"><span data-stu-id="3dec1-245">userStatuses</span></span>|<span data-ttu-id="3dec1-246">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="3dec1-246">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="3dec1-247">ユーザーごとのデバイス構成のインストール状態です。</span><span class="sxs-lookup"><span data-stu-id="3dec1-247">Device configuration installation status by user.</span></span> <span data-ttu-id="3dec1-248">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3dec1-248">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dec1-249">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="3dec1-249">deviceStatusOverview</span></span>|[<span data-ttu-id="3dec1-250">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="3dec1-250">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="3dec1-251">デバイス構成のデバイス状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="3dec1-251">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dec1-252">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="3dec1-252">userStatusOverview</span></span>|[<span data-ttu-id="3dec1-253">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="3dec1-253">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="3dec1-254">デバイス構成のユーザー状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="3dec1-254">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dec1-255">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="3dec1-255">deviceSettingStateSummaries</span></span>|<span data-ttu-id="3dec1-256">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="3dec1-256">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="3dec1-257">デバイス構成設定状態のデバイスの要約 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="3dec1-257">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3dec1-258">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3dec1-258">JSON Representation</span></span>
<span data-ttu-id="3dec1-259">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3dec1-259">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sharedPCConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "accountManagerPolicy": {
    "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
    "accountDeletionPolicy": "String",
    "cacheAccountsAboveDiskFreePercentage": 1024,
    "inactiveThresholdDays": 1024,
    "removeAccountsBelowDiskFreePercentage": 1024
  },
  "allowedAccounts": "String",
  "localStorage": "String",
  "allowLocalStorage": true,
  "setAccountManager": "String",
  "disableAccountManager": true,
  "setEduPolicies": "String",
  "disableEduPolicies": true,
  "setPowerPolicies": "String",
  "disablePowerPolicies": true,
  "signInOnResume": "String",
  "disableSignInOnResume": true,
  "enabled": true,
  "idleTimeBeforeSleepInSeconds": 1024,
  "kioskAppDisplayName": "String",
  "kioskAppUserModelId": "String",
  "maintenanceStartTime": "String (time of day)"
}
```




