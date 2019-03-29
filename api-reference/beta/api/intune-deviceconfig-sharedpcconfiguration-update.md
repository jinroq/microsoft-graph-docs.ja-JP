---
title: sharedPCConfiguration の更新
description: sharedPCConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9f250606e5c58d16b9edf6d266284c45ec437273
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30956710"
---
# <a name="update-sharedpcconfiguration"></a><span data-ttu-id="f91fc-103">sharedPCConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="f91fc-103">Update sharedPCConfiguration</span></span>

> <span data-ttu-id="f91fc-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f91fc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f91fc-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f91fc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f91fc-106">[sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f91fc-106">Update the properties of a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f91fc-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f91fc-107">Prerequisites</span></span>
<span data-ttu-id="f91fc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f91fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f91fc-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f91fc-110">Permission type</span></span>|<span data-ttu-id="f91fc-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f91fc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f91fc-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f91fc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f91fc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f91fc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f91fc-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f91fc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f91fc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f91fc-115">Not supported.</span></span>|
|<span data-ttu-id="f91fc-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f91fc-116">Application</span></span>|<span data-ttu-id="f91fc-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f91fc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f91fc-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f91fc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f91fc-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f91fc-119">Request headers</span></span>
|<span data-ttu-id="f91fc-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f91fc-120">Header</span></span>|<span data-ttu-id="f91fc-121">値</span><span class="sxs-lookup"><span data-stu-id="f91fc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f91fc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f91fc-122">Authorization</span></span>|<span data-ttu-id="f91fc-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f91fc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f91fc-124">承諾</span><span class="sxs-lookup"><span data-stu-id="f91fc-124">Accept</span></span>|<span data-ttu-id="f91fc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f91fc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f91fc-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f91fc-126">Request body</span></span>
<span data-ttu-id="f91fc-127">要求本文で、[sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) オブジェクト用の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f91fc-127">In the request body, supply a JSON representation for the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

<span data-ttu-id="f91fc-128">次の表に、[sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f91fc-128">The following table shows the properties that are required when you create the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span></span>

|<span data-ttu-id="f91fc-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f91fc-129">Property</span></span>|<span data-ttu-id="f91fc-130">型</span><span class="sxs-lookup"><span data-stu-id="f91fc-130">Type</span></span>|<span data-ttu-id="f91fc-131">説明</span><span class="sxs-lookup"><span data-stu-id="f91fc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f91fc-132">id</span><span class="sxs-lookup"><span data-stu-id="f91fc-132">id</span></span>|<span data-ttu-id="f91fc-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f91fc-133">String</span></span>|<span data-ttu-id="f91fc-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f91fc-134">Key of the entity.</span></span> <span data-ttu-id="f91fc-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f91fc-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f91fc-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f91fc-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f91fc-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f91fc-137">DateTimeOffset</span></span>|<span data-ttu-id="f91fc-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="f91fc-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f91fc-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f91fc-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f91fc-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f91fc-140">roleScopeTagIds</span></span>|<span data-ttu-id="f91fc-141">String collection</span><span class="sxs-lookup"><span data-stu-id="f91fc-141">String collection</span></span>|<span data-ttu-id="f91fc-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="f91fc-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f91fc-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f91fc-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f91fc-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f91fc-144">supportsScopeTags</span></span>|<span data-ttu-id="f91fc-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="f91fc-145">Boolean</span></span>|<span data-ttu-id="f91fc-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f91fc-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f91fc-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="f91fc-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f91fc-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="f91fc-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f91fc-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="f91fc-149">This property is read-only.</span></span> <span data-ttu-id="f91fc-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f91fc-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f91fc-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f91fc-151">createdDateTime</span></span>|<span data-ttu-id="f91fc-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f91fc-152">DateTimeOffset</span></span>|<span data-ttu-id="f91fc-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="f91fc-153">DateTime the object was created.</span></span> <span data-ttu-id="f91fc-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f91fc-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f91fc-155">description</span><span class="sxs-lookup"><span data-stu-id="f91fc-155">description</span></span>|<span data-ttu-id="f91fc-156">String</span><span class="sxs-lookup"><span data-stu-id="f91fc-156">String</span></span>|<span data-ttu-id="f91fc-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="f91fc-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f91fc-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f91fc-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f91fc-159">displayName</span><span class="sxs-lookup"><span data-stu-id="f91fc-159">displayName</span></span>|<span data-ttu-id="f91fc-160">String</span><span class="sxs-lookup"><span data-stu-id="f91fc-160">String</span></span>|<span data-ttu-id="f91fc-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="f91fc-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f91fc-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f91fc-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f91fc-163">version</span><span class="sxs-lookup"><span data-stu-id="f91fc-163">version</span></span>|<span data-ttu-id="f91fc-164">Int32</span><span class="sxs-lookup"><span data-stu-id="f91fc-164">Int32</span></span>|<span data-ttu-id="f91fc-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="f91fc-165">Version of the device configuration.</span></span> <span data-ttu-id="f91fc-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f91fc-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f91fc-167">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="f91fc-167">accountManagerPolicy</span></span>|[<span data-ttu-id="f91fc-168">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="f91fc-168">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="f91fc-169">共有の PC 上でアカウントを管理する方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="f91fc-169">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="f91fc-170">disableAccountManager が false の場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="f91fc-170">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="f91fc-171">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="f91fc-171">allowedAccounts</span></span>|[<span data-ttu-id="f91fc-172">sharedpcallowedaccounttype</span><span class="sxs-lookup"><span data-stu-id="f91fc-172">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="f91fc-173">共有の PC で使用できるアカウントの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="f91fc-173">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="f91fc-174">使用可能な値は、`notConfigured`、`guest`、`domain` です。</span><span class="sxs-lookup"><span data-stu-id="f91fc-174">Possible values are: `notConfigured`, `guest`, `domain`.</span></span>|
|<span data-ttu-id="f91fc-175">localStorage</span><span class="sxs-lookup"><span data-stu-id="f91fc-175">localStorage</span></span>|[<span data-ttu-id="f91fc-176">購入</span><span class="sxs-lookup"><span data-stu-id="f91fc-176">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f91fc-177">共有の PC でローカル ストレージを許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="f91fc-177">Specifies whether local storage is allowed on a shared PC.</span></span> <span data-ttu-id="f91fc-178">使用可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="f91fc-178">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="f91fc-179">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="f91fc-179">allowLocalStorage</span></span>|<span data-ttu-id="f91fc-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="f91fc-180">Boolean</span></span>|<span data-ttu-id="f91fc-181">共有の PC でローカル ストレージを許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="f91fc-181">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="f91fc-182">setaccountmanager</span><span class="sxs-lookup"><span data-stu-id="f91fc-182">setAccountManager</span></span>|[<span data-ttu-id="f91fc-183">購入</span><span class="sxs-lookup"><span data-stu-id="f91fc-183">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f91fc-184">共有 PC モードのアカウント マネージャーを無効にします。</span><span class="sxs-lookup"><span data-stu-id="f91fc-184">Disables the account manager for shared PC mode.</span></span> <span data-ttu-id="f91fc-185">使用可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="f91fc-185">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="f91fc-186">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="f91fc-186">disableAccountManager</span></span>|<span data-ttu-id="f91fc-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="f91fc-187">Boolean</span></span>|<span data-ttu-id="f91fc-188">共有 PC モードのアカウント マネージャーを無効にします。</span><span class="sxs-lookup"><span data-stu-id="f91fc-188">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="f91fc-189">setEduPolicies</span><span class="sxs-lookup"><span data-stu-id="f91fc-189">setEduPolicies</span></span>|[<span data-ttu-id="f91fc-190">購入</span><span class="sxs-lookup"><span data-stu-id="f91fc-190">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f91fc-191">既定の共有 PC 教育環境ポリシーを有効/無効にするか、構成しないかを指定します。</span><span class="sxs-lookup"><span data-stu-id="f91fc-191">Specifies whether the default shared PC education environment policies should be enabled/disabled/not configured.</span></span> <span data-ttu-id="f91fc-192">Windows 10 RS2 以降では、このポリシーは Enabled を true に設定しなくても適用されます。</span><span class="sxs-lookup"><span data-stu-id="f91fc-192">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span> <span data-ttu-id="f91fc-193">使用可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="f91fc-193">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="f91fc-194">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="f91fc-194">disableEduPolicies</span></span>|<span data-ttu-id="f91fc-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="f91fc-195">Boolean</span></span>|<span data-ttu-id="f91fc-196">既定の共有 PC 教育環境ポリシーを無効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="f91fc-196">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="f91fc-197">Windows 10 RS2 以降では、このポリシーは Enabled を true に設定しなくても適用されます。</span><span class="sxs-lookup"><span data-stu-id="f91fc-197">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="f91fc-198">setpowerpolicies</span><span class="sxs-lookup"><span data-stu-id="f91fc-198">setPowerPolicies</span></span>|[<span data-ttu-id="f91fc-199">購入</span><span class="sxs-lookup"><span data-stu-id="f91fc-199">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f91fc-200">既定の共有 PC 電源ポリシーを有効または無効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="f91fc-200">Specifies whether the default shared PC power policies should be enabled/disabled.</span></span> <span data-ttu-id="f91fc-201">使用可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="f91fc-201">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="f91fc-202">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="f91fc-202">disablePowerPolicies</span></span>|<span data-ttu-id="f91fc-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="f91fc-203">Boolean</span></span>|<span data-ttu-id="f91fc-204">既定の共有 PC 電源ポリシーを無効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="f91fc-204">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="f91fc-205">signInOnResume</span><span class="sxs-lookup"><span data-stu-id="f91fc-205">signInOnResume</span></span>|[<span data-ttu-id="f91fc-206">購入</span><span class="sxs-lookup"><span data-stu-id="f91fc-206">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f91fc-207">デバイスがスリープモードから復帰したときに毎回サインインする必要があることを指定します。</span><span class="sxs-lookup"><span data-stu-id="f91fc-207">Specifies the requirement to sign in whenever the device wakes up from sleep mode.</span></span> <span data-ttu-id="f91fc-208">使用可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="f91fc-208">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="f91fc-209">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="f91fc-209">disableSignInOnResume</span></span>|<span data-ttu-id="f91fc-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="f91fc-210">Boolean</span></span>|<span data-ttu-id="f91fc-211">デバイスがスリープ モードから再開するたびにサインインを求める設定を無効にします。</span><span class="sxs-lookup"><span data-stu-id="f91fc-211">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="f91fc-212">enabled</span><span class="sxs-lookup"><span data-stu-id="f91fc-212">enabled</span></span>|<span data-ttu-id="f91fc-213">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="f91fc-213">Boolean</span></span>|<span data-ttu-id="f91fc-214">共有 PC モードを有効にし、共有 PC のポリシーを適用します。</span><span class="sxs-lookup"><span data-stu-id="f91fc-214">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="f91fc-215">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="f91fc-215">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="f91fc-216">Int32</span><span class="sxs-lookup"><span data-stu-id="f91fc-216">Int32</span></span>|<span data-ttu-id="f91fc-217">PC がスリープ状態になるまでにデバイスがアイドル状態を続ける時間を秒単位で指定します。</span><span class="sxs-lookup"><span data-stu-id="f91fc-217">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="f91fc-218">この値を 0 に設定すると、スリープ タイムアウトは発生しなくなります。</span><span class="sxs-lookup"><span data-stu-id="f91fc-218">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="f91fc-219">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="f91fc-219">kioskAppDisplayName</span></span>|<span data-ttu-id="f91fc-220">String</span><span class="sxs-lookup"><span data-stu-id="f91fc-220">String</span></span>|<span data-ttu-id="f91fc-221">SetKioskAppUserModelId で指定されたアプリを起動するサインイン画面に表示されるアカウントの表示テキストを指定します。</span><span class="sxs-lookup"><span data-stu-id="f91fc-221">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="f91fc-222">KioskAppUserModelId が設定されている場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="f91fc-222">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="f91fc-223">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="f91fc-223">kioskAppUserModelId</span></span>|<span data-ttu-id="f91fc-224">String</span><span class="sxs-lookup"><span data-stu-id="f91fc-224">String</span></span>|<span data-ttu-id="f91fc-225">割り当てられたアクセスで使用するアプリのアプリケーション ユーザー モデル ID を指定します。</span><span class="sxs-lookup"><span data-stu-id="f91fc-225">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="f91fc-226">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="f91fc-226">maintenanceStartTime</span></span>|<span data-ttu-id="f91fc-227">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="f91fc-227">TimeOfDay</span></span>|<span data-ttu-id="f91fc-228">毎日のメンテナンス時間の開始時刻を指定します。</span><span class="sxs-lookup"><span data-stu-id="f91fc-228">Specifies the daily start time of maintenance hour.</span></span>|
|<span data-ttu-id="f91fc-229">fastfirstsignin</span><span class="sxs-lookup"><span data-stu-id="f91fc-229">fastFirstSignIn</span></span>|[<span data-ttu-id="f91fc-230">購入</span><span class="sxs-lookup"><span data-stu-id="f91fc-230">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f91fc-231">管理者以外の新しい Azure AD アカウントを事前に構成された候補ローカルアカウントに自動的に接続するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="f91fc-231">Specifies whether to auto connect new non-admin Azure AD accounts to pre-configured candidate local accounts.</span></span> <span data-ttu-id="f91fc-232">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="f91fc-232">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="f91fc-233">応答</span><span class="sxs-lookup"><span data-stu-id="f91fc-233">Response</span></span>
<span data-ttu-id="f91fc-234">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="f91fc-234">If successful, this method returns a `200 OK` response code and an updated [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f91fc-235">例</span><span class="sxs-lookup"><span data-stu-id="f91fc-235">Example</span></span>

### <a name="request"></a><span data-ttu-id="f91fc-236">要求</span><span class="sxs-lookup"><span data-stu-id="f91fc-236">Request</span></span>
<span data-ttu-id="f91fc-237">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f91fc-237">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1147

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
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
  "allowedAccounts": "guest",
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
  "maintenanceStartTime": "11:59:24.7240000",
  "fastFirstSignIn": "enabled"
}
```

### <a name="response"></a><span data-ttu-id="f91fc-238">応答</span><span class="sxs-lookup"><span data-stu-id="f91fc-238">Response</span></span>
<span data-ttu-id="f91fc-p121">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f91fc-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1319

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
  "allowedAccounts": "guest",
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
  "maintenanceStartTime": "11:59:24.7240000",
  "fastFirstSignIn": "enabled"
}
```




