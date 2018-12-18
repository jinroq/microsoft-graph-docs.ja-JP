---
title: Create sharedPCConfiguration
description: 新しい sharedPCConfiguration オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: a9a4dce6a0ab13d8f28b9b7c532c02baf180bfa2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336100"
---
# <a name="create-sharedpcconfiguration"></a><span data-ttu-id="73c53-103">Create sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="73c53-103">Create sharedPCConfiguration</span></span>

> <span data-ttu-id="73c53-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="73c53-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="73c53-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="73c53-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="73c53-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="73c53-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="73c53-107">新しい [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="73c53-107">Create a new [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="73c53-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="73c53-108">Prerequisites</span></span>
<span data-ttu-id="73c53-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="73c53-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73c53-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="73c53-111">Permission type</span></span>|<span data-ttu-id="73c53-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="73c53-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73c53-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="73c53-113">Delegated (work or school account)</span></span>|<span data-ttu-id="73c53-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73c53-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="73c53-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="73c53-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73c53-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="73c53-116">Not supported.</span></span>|
|<span data-ttu-id="73c53-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="73c53-117">Application</span></span>|<span data-ttu-id="73c53-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="73c53-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73c53-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="73c53-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="73c53-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="73c53-120">Request headers</span></span>
|<span data-ttu-id="73c53-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="73c53-121">Header</span></span>|<span data-ttu-id="73c53-122">値</span><span class="sxs-lookup"><span data-stu-id="73c53-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73c53-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="73c53-123">Authorization</span></span>|<span data-ttu-id="73c53-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="73c53-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73c53-125">Accept</span><span class="sxs-lookup"><span data-stu-id="73c53-125">Accept</span></span>|<span data-ttu-id="73c53-126">application/json</span><span class="sxs-lookup"><span data-stu-id="73c53-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73c53-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="73c53-127">Request body</span></span>
<span data-ttu-id="73c53-128">要求本文で、sharedPCConfiguration オブジェクト用の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="73c53-128">In the request body, supply a JSON representation for the sharedPCConfiguration object.</span></span>

<span data-ttu-id="73c53-129">次の表に、sharedPCConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="73c53-129">The following table shows the properties that are required when you create the sharedPCConfiguration.</span></span>

|<span data-ttu-id="73c53-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="73c53-130">Property</span></span>|<span data-ttu-id="73c53-131">種類</span><span class="sxs-lookup"><span data-stu-id="73c53-131">Type</span></span>|<span data-ttu-id="73c53-132">説明</span><span class="sxs-lookup"><span data-stu-id="73c53-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73c53-133">ID</span><span class="sxs-lookup"><span data-stu-id="73c53-133">id</span></span>|<span data-ttu-id="73c53-134">String</span><span class="sxs-lookup"><span data-stu-id="73c53-134">String</span></span>|<span data-ttu-id="73c53-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="73c53-135">Key of the entity.</span></span> <span data-ttu-id="73c53-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="73c53-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73c53-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="73c53-137">lastModifiedDateTime</span></span>|<span data-ttu-id="73c53-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73c53-138">DateTimeOffset</span></span>|<span data-ttu-id="73c53-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="73c53-139">DateTime the object was last modified.</span></span> <span data-ttu-id="73c53-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="73c53-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73c53-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="73c53-141">roleScopeTagIds</span></span>|<span data-ttu-id="73c53-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="73c53-142">String collection</span></span>|<span data-ttu-id="73c53-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="73c53-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="73c53-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="73c53-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73c53-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="73c53-145">supportsScopeTags</span></span>|<span data-ttu-id="73c53-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="73c53-146">Boolean</span></span>|<span data-ttu-id="73c53-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="73c53-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="73c53-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="73c53-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="73c53-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="73c53-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="73c53-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="73c53-150">This property is read-only.</span></span> <span data-ttu-id="73c53-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="73c53-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73c53-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="73c53-152">createdDateTime</span></span>|<span data-ttu-id="73c53-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73c53-153">DateTimeOffset</span></span>|<span data-ttu-id="73c53-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="73c53-154">DateTime the object was created.</span></span> <span data-ttu-id="73c53-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="73c53-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73c53-156">説明</span><span class="sxs-lookup"><span data-stu-id="73c53-156">description</span></span>|<span data-ttu-id="73c53-157">String</span><span class="sxs-lookup"><span data-stu-id="73c53-157">String</span></span>|<span data-ttu-id="73c53-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="73c53-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="73c53-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="73c53-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73c53-160">displayName</span><span class="sxs-lookup"><span data-stu-id="73c53-160">displayName</span></span>|<span data-ttu-id="73c53-161">String</span><span class="sxs-lookup"><span data-stu-id="73c53-161">String</span></span>|<span data-ttu-id="73c53-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="73c53-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="73c53-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="73c53-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73c53-164">version</span><span class="sxs-lookup"><span data-stu-id="73c53-164">version</span></span>|<span data-ttu-id="73c53-165">Int32</span><span class="sxs-lookup"><span data-stu-id="73c53-165">Int32</span></span>|<span data-ttu-id="73c53-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="73c53-166">Version of the device configuration.</span></span> <span data-ttu-id="73c53-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="73c53-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73c53-168">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="73c53-168">accountManagerPolicy</span></span>|[<span data-ttu-id="73c53-169">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="73c53-169">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="73c53-170">共有の PC 上でアカウントを管理する方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="73c53-170">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="73c53-171">disableAccountManager が false の場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="73c53-171">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="73c53-172">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="73c53-172">allowedAccounts</span></span>|[<span data-ttu-id="73c53-173">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="73c53-173">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="73c53-174">共有の PC で使用できるアカウントの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="73c53-174">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="73c53-175">可能な値は、`guest`、`domain` です。</span><span class="sxs-lookup"><span data-stu-id="73c53-175">Possible values are: `guest`, `domain`.</span></span>|
|<span data-ttu-id="73c53-176">localStorage</span><span class="sxs-lookup"><span data-stu-id="73c53-176">localStorage</span></span>|[<span data-ttu-id="73c53-177">有効化</span><span class="sxs-lookup"><span data-stu-id="73c53-177">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="73c53-178">共有の PC でローカル ストレージを許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="73c53-178">Specifies whether local storage is allowed on a shared PC.</span></span> <span data-ttu-id="73c53-179">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="73c53-179">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="73c53-180">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="73c53-180">allowLocalStorage</span></span>|<span data-ttu-id="73c53-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="73c53-181">Boolean</span></span>|<span data-ttu-id="73c53-182">共有の PC でローカル ストレージを許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="73c53-182">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="73c53-183">setAccountManager</span><span class="sxs-lookup"><span data-stu-id="73c53-183">setAccountManager</span></span>|[<span data-ttu-id="73c53-184">有効化</span><span class="sxs-lookup"><span data-stu-id="73c53-184">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="73c53-185">共有 PC モードのアカウント マネージャーを無効にします。</span><span class="sxs-lookup"><span data-stu-id="73c53-185">Disables the account manager for shared PC mode.</span></span> <span data-ttu-id="73c53-186">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="73c53-186">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="73c53-187">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="73c53-187">disableAccountManager</span></span>|<span data-ttu-id="73c53-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="73c53-188">Boolean</span></span>|<span data-ttu-id="73c53-189">共有 PC モードのアカウント マネージャーを無効にします。</span><span class="sxs-lookup"><span data-stu-id="73c53-189">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="73c53-190">setEduPolicies</span><span class="sxs-lookup"><span data-stu-id="73c53-190">setEduPolicies</span></span>|[<span data-ttu-id="73c53-191">有効化</span><span class="sxs-lookup"><span data-stu-id="73c53-191">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="73c53-192">PC 教育環境の既定の共有ポリシー構成かどうか、有効、無効としないことを指定します。</span><span class="sxs-lookup"><span data-stu-id="73c53-192">Specifies whether the default shared PC education environment policies should be enabled/disabled/not configured.</span></span> <span data-ttu-id="73c53-193">Windows 10 RS2 以降では、このポリシーは Enabled を true に設定しなくても適用されます。</span><span class="sxs-lookup"><span data-stu-id="73c53-193">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span> <span data-ttu-id="73c53-194">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="73c53-194">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="73c53-195">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="73c53-195">disableEduPolicies</span></span>|<span data-ttu-id="73c53-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="73c53-196">Boolean</span></span>|<span data-ttu-id="73c53-197">既定の共有 PC 教育環境ポリシーを無効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="73c53-197">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="73c53-198">Windows 10 RS2 以降では、このポリシーは Enabled を true に設定しなくても適用されます。</span><span class="sxs-lookup"><span data-stu-id="73c53-198">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="73c53-199">setPowerPolicies</span><span class="sxs-lookup"><span data-stu-id="73c53-199">setPowerPolicies</span></span>|[<span data-ttu-id="73c53-200">有効化</span><span class="sxs-lookup"><span data-stu-id="73c53-200">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="73c53-201">かどうか既定の共有の PC の電源ポリシーが有効または無効にするを指定します。</span><span class="sxs-lookup"><span data-stu-id="73c53-201">Specifies whether the default shared PC power policies should be enabled/disabled.</span></span> <span data-ttu-id="73c53-202">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="73c53-202">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="73c53-203">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="73c53-203">disablePowerPolicies</span></span>|<span data-ttu-id="73c53-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="73c53-204">Boolean</span></span>|<span data-ttu-id="73c53-205">既定の共有 PC 電源ポリシーを無効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="73c53-205">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="73c53-206">signInOnResume</span><span class="sxs-lookup"><span data-stu-id="73c53-206">signInOnResume</span></span>|[<span data-ttu-id="73c53-207">有効化</span><span class="sxs-lookup"><span data-stu-id="73c53-207">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="73c53-208">署名するための要件を指定のときに、デバイスのスリープ状態スリープ モードから。</span><span class="sxs-lookup"><span data-stu-id="73c53-208">Specifies the requirement to sign in whenever the device wakes up from sleep mode.</span></span> <span data-ttu-id="73c53-209">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="73c53-209">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="73c53-210">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="73c53-210">disableSignInOnResume</span></span>|<span data-ttu-id="73c53-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="73c53-211">Boolean</span></span>|<span data-ttu-id="73c53-212">デバイスがスリープ モードから再開するたびにサインインを求める設定を無効にします。</span><span class="sxs-lookup"><span data-stu-id="73c53-212">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="73c53-213">enabled</span><span class="sxs-lookup"><span data-stu-id="73c53-213">enabled</span></span>|<span data-ttu-id="73c53-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="73c53-214">Boolean</span></span>|<span data-ttu-id="73c53-215">共有 PC モードを有効にし、共有 PC のポリシーを適用します。</span><span class="sxs-lookup"><span data-stu-id="73c53-215">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="73c53-216">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="73c53-216">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="73c53-217">Int32</span><span class="sxs-lookup"><span data-stu-id="73c53-217">Int32</span></span>|<span data-ttu-id="73c53-218">PC がスリープ状態になるまでにデバイスがアイドル状態を続ける時間を秒単位で指定します。</span><span class="sxs-lookup"><span data-stu-id="73c53-218">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="73c53-219">この値を 0 に設定すると、スリープ タイムアウトは発生しなくなります。</span><span class="sxs-lookup"><span data-stu-id="73c53-219">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="73c53-220">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="73c53-220">kioskAppDisplayName</span></span>|<span data-ttu-id="73c53-221">String</span><span class="sxs-lookup"><span data-stu-id="73c53-221">String</span></span>|<span data-ttu-id="73c53-222">SetKioskAppUserModelId で指定されたアプリを起動するサインイン画面に表示されるアカウントの表示テキストを指定します。</span><span class="sxs-lookup"><span data-stu-id="73c53-222">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="73c53-223">KioskAppUserModelId が設定されている場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="73c53-223">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="73c53-224">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="73c53-224">kioskAppUserModelId</span></span>|<span data-ttu-id="73c53-225">String</span><span class="sxs-lookup"><span data-stu-id="73c53-225">String</span></span>|<span data-ttu-id="73c53-226">割り当てられたアクセスで使用するアプリのアプリケーション ユーザー モデル ID を指定します。</span><span class="sxs-lookup"><span data-stu-id="73c53-226">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="73c53-227">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="73c53-227">maintenanceStartTime</span></span>|<span data-ttu-id="73c53-228">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="73c53-228">TimeOfDay</span></span>|<span data-ttu-id="73c53-229">毎日のメンテナンス時間の開始時刻を指定します。</span><span class="sxs-lookup"><span data-stu-id="73c53-229">Specifies the daily start time of maintenance hour.</span></span>|



## <a name="response"></a><span data-ttu-id="73c53-230">応答</span><span class="sxs-lookup"><span data-stu-id="73c53-230">Response</span></span>
<span data-ttu-id="73c53-231">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="73c53-231">If successful, this method returns a `201 Created` response code and a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73c53-232">例</span><span class="sxs-lookup"><span data-stu-id="73c53-232">Example</span></span>
### <a name="request"></a><span data-ttu-id="73c53-233">要求</span><span class="sxs-lookup"><span data-stu-id="73c53-233">Request</span></span>
<span data-ttu-id="73c53-234">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="73c53-234">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1179

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountManagerPolicy": {
    "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
    "accountDeletionPolicy": "diskSpaceThreshold",
    "cacheAccountsAboveDiskFreePercentage": 4,
    "inactiveThresholdDays": 5,
    "removeAccountsBelowDiskFreePercentage": 5
  },
  "allowedAccounts": "domain",
  "localStorage": "enabled",
  "allowLocalStorage": true,
  "setAccountManager": "enabled",
  "disableAccountManager": true,
  "setEduPolicies": "enabled",
  "disableEduPolicies": true,
  "setPowerPolicies": "enabled",
  "disablePowerPolicies": true,
  "signInOnResume": "enabled",
  "disableSignInOnResume": true,
  "enabled": true,
  "idleTimeBeforeSleepInSeconds": 12,
  "kioskAppDisplayName": "Kiosk App Display Name value",
  "kioskAppUserModelId": "Kiosk App User Model Id value",
  "maintenanceStartTime": "11:59:24.7240000"
}
```

### <a name="response"></a><span data-ttu-id="73c53-235">応答</span><span class="sxs-lookup"><span data-stu-id="73c53-235">Response</span></span>
<span data-ttu-id="73c53-p121">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="73c53-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1287

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "id": "5206be3b-be3b-5206-3bbe-06523bbe0652",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountManagerPolicy": {
    "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
    "accountDeletionPolicy": "diskSpaceThreshold",
    "cacheAccountsAboveDiskFreePercentage": 4,
    "inactiveThresholdDays": 5,
    "removeAccountsBelowDiskFreePercentage": 5
  },
  "allowedAccounts": "domain",
  "localStorage": "enabled",
  "allowLocalStorage": true,
  "setAccountManager": "enabled",
  "disableAccountManager": true,
  "setEduPolicies": "enabled",
  "disableEduPolicies": true,
  "setPowerPolicies": "enabled",
  "disablePowerPolicies": true,
  "signInOnResume": "enabled",
  "disableSignInOnResume": true,
  "enabled": true,
  "idleTimeBeforeSleepInSeconds": 12,
  "kioskAppDisplayName": "Kiosk App Display Name value",
  "kioskAppUserModelId": "Kiosk App User Model Id value",
  "maintenanceStartTime": "11:59:24.7240000"
}
```





