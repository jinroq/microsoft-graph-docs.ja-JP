---
title: Create sharedPCConfiguration
description: 新しい sharedPCConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6f30345bbf10bd0d0272dc4b87999951678e42db
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33922116"
---
# <a name="create-sharedpcconfiguration"></a><span data-ttu-id="8bb29-103">Create sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="8bb29-103">Create sharedPCConfiguration</span></span>

> <span data-ttu-id="8bb29-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8bb29-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8bb29-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8bb29-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8bb29-106">新しい [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="8bb29-106">Create a new [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8bb29-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="8bb29-107">Prerequisites</span></span>
<span data-ttu-id="8bb29-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8bb29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bb29-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8bb29-110">Permission type</span></span>|<span data-ttu-id="8bb29-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8bb29-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8bb29-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8bb29-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8bb29-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bb29-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8bb29-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8bb29-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8bb29-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8bb29-115">Not supported.</span></span>|
|<span data-ttu-id="8bb29-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8bb29-116">Application</span></span>|<span data-ttu-id="8bb29-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8bb29-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8bb29-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8bb29-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8bb29-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8bb29-119">Request headers</span></span>
|<span data-ttu-id="8bb29-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8bb29-120">Header</span></span>|<span data-ttu-id="8bb29-121">値</span><span class="sxs-lookup"><span data-stu-id="8bb29-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8bb29-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8bb29-122">Authorization</span></span>|<span data-ttu-id="8bb29-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="8bb29-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8bb29-124">承諾</span><span class="sxs-lookup"><span data-stu-id="8bb29-124">Accept</span></span>|<span data-ttu-id="8bb29-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8bb29-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8bb29-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8bb29-126">Request body</span></span>
<span data-ttu-id="8bb29-127">要求本文で、sharedPCConfiguration オブジェクト用の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8bb29-127">In the request body, supply a JSON representation for the sharedPCConfiguration object.</span></span>

<span data-ttu-id="8bb29-128">次の表に、sharedPCConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8bb29-128">The following table shows the properties that are required when you create the sharedPCConfiguration.</span></span>

|<span data-ttu-id="8bb29-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8bb29-129">Property</span></span>|<span data-ttu-id="8bb29-130">型</span><span class="sxs-lookup"><span data-stu-id="8bb29-130">Type</span></span>|<span data-ttu-id="8bb29-131">説明</span><span class="sxs-lookup"><span data-stu-id="8bb29-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bb29-132">id</span><span class="sxs-lookup"><span data-stu-id="8bb29-132">id</span></span>|<span data-ttu-id="8bb29-133">文字列</span><span class="sxs-lookup"><span data-stu-id="8bb29-133">String</span></span>|<span data-ttu-id="8bb29-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8bb29-134">Key of the entity.</span></span> <span data-ttu-id="8bb29-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8bb29-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bb29-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8bb29-136">lastModifiedDateTime</span></span>|<span data-ttu-id="8bb29-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bb29-137">DateTimeOffset</span></span>|<span data-ttu-id="8bb29-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="8bb29-138">DateTime the object was last modified.</span></span> <span data-ttu-id="8bb29-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8bb29-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bb29-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8bb29-140">roleScopeTagIds</span></span>|<span data-ttu-id="8bb29-141">String collection</span><span class="sxs-lookup"><span data-stu-id="8bb29-141">String collection</span></span>|<span data-ttu-id="8bb29-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="8bb29-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8bb29-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8bb29-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bb29-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8bb29-144">supportsScopeTags</span></span>|<span data-ttu-id="8bb29-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="8bb29-145">Boolean</span></span>|<span data-ttu-id="8bb29-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8bb29-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8bb29-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="8bb29-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8bb29-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="8bb29-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8bb29-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="8bb29-149">This property is read-only.</span></span> <span data-ttu-id="8bb29-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8bb29-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bb29-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8bb29-151">createdDateTime</span></span>|<span data-ttu-id="8bb29-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bb29-152">DateTimeOffset</span></span>|<span data-ttu-id="8bb29-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="8bb29-153">DateTime the object was created.</span></span> <span data-ttu-id="8bb29-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8bb29-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bb29-155">description</span><span class="sxs-lookup"><span data-stu-id="8bb29-155">description</span></span>|<span data-ttu-id="8bb29-156">String</span><span class="sxs-lookup"><span data-stu-id="8bb29-156">String</span></span>|<span data-ttu-id="8bb29-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="8bb29-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8bb29-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8bb29-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bb29-159">displayName</span><span class="sxs-lookup"><span data-stu-id="8bb29-159">displayName</span></span>|<span data-ttu-id="8bb29-160">String</span><span class="sxs-lookup"><span data-stu-id="8bb29-160">String</span></span>|<span data-ttu-id="8bb29-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="8bb29-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8bb29-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8bb29-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bb29-163">version</span><span class="sxs-lookup"><span data-stu-id="8bb29-163">version</span></span>|<span data-ttu-id="8bb29-164">Int32</span><span class="sxs-lookup"><span data-stu-id="8bb29-164">Int32</span></span>|<span data-ttu-id="8bb29-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="8bb29-165">Version of the device configuration.</span></span> <span data-ttu-id="8bb29-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8bb29-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bb29-167">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="8bb29-167">accountManagerPolicy</span></span>|[<span data-ttu-id="8bb29-168">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="8bb29-168">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="8bb29-169">共有の PC 上でアカウントを管理する方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="8bb29-169">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="8bb29-170">disableAccountManager が false の場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="8bb29-170">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="8bb29-171">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="8bb29-171">allowedAccounts</span></span>|[<span data-ttu-id="8bb29-172">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="8bb29-172">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="8bb29-173">共有の PC で使用できるアカウントの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="8bb29-173">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="8bb29-174">可能な値は、`notConfigured`、`guest`、`domain` です。</span><span class="sxs-lookup"><span data-stu-id="8bb29-174">Possible values are: `notConfigured`, `guest`, `domain`.</span></span>|
|<span data-ttu-id="8bb29-175">localStorage</span><span class="sxs-lookup"><span data-stu-id="8bb29-175">localStorage</span></span>|[<span data-ttu-id="8bb29-176">購入</span><span class="sxs-lookup"><span data-stu-id="8bb29-176">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="8bb29-177">共有の PC でローカル ストレージを許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="8bb29-177">Specifies whether local storage is allowed on a shared PC.</span></span> <span data-ttu-id="8bb29-178">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="8bb29-178">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="8bb29-179">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="8bb29-179">allowLocalStorage</span></span>|<span data-ttu-id="8bb29-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="8bb29-180">Boolean</span></span>|<span data-ttu-id="8bb29-181">共有の PC でローカル ストレージを許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="8bb29-181">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="8bb29-182">setAccountManager</span><span class="sxs-lookup"><span data-stu-id="8bb29-182">setAccountManager</span></span>|[<span data-ttu-id="8bb29-183">購入</span><span class="sxs-lookup"><span data-stu-id="8bb29-183">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="8bb29-184">共有 PC モードのアカウント マネージャーを無効にします。</span><span class="sxs-lookup"><span data-stu-id="8bb29-184">Disables the account manager for shared PC mode.</span></span> <span data-ttu-id="8bb29-185">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="8bb29-185">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="8bb29-186">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="8bb29-186">disableAccountManager</span></span>|<span data-ttu-id="8bb29-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="8bb29-187">Boolean</span></span>|<span data-ttu-id="8bb29-188">共有 PC モードのアカウント マネージャーを無効にします。</span><span class="sxs-lookup"><span data-stu-id="8bb29-188">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="8bb29-189">setEduPolicies</span><span class="sxs-lookup"><span data-stu-id="8bb29-189">setEduPolicies</span></span>|[<span data-ttu-id="8bb29-190">購入</span><span class="sxs-lookup"><span data-stu-id="8bb29-190">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="8bb29-191">既定の共有 PC 教育環境ポリシーを有効/無効にするか、構成しないかを指定します。</span><span class="sxs-lookup"><span data-stu-id="8bb29-191">Specifies whether the default shared PC education environment policies should be enabled/disabled/not configured.</span></span> <span data-ttu-id="8bb29-192">Windows 10 RS2 以降では、このポリシーは Enabled を true に設定しなくても適用されます。</span><span class="sxs-lookup"><span data-stu-id="8bb29-192">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span> <span data-ttu-id="8bb29-193">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="8bb29-193">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="8bb29-194">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="8bb29-194">disableEduPolicies</span></span>|<span data-ttu-id="8bb29-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="8bb29-195">Boolean</span></span>|<span data-ttu-id="8bb29-196">既定の共有 PC 教育環境ポリシーを無効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="8bb29-196">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="8bb29-197">Windows 10 RS2 以降では、このポリシーは Enabled を true に設定しなくても適用されます。</span><span class="sxs-lookup"><span data-stu-id="8bb29-197">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="8bb29-198">setPowerPolicies</span><span class="sxs-lookup"><span data-stu-id="8bb29-198">setPowerPolicies</span></span>|[<span data-ttu-id="8bb29-199">購入</span><span class="sxs-lookup"><span data-stu-id="8bb29-199">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="8bb29-200">既定の共有 PC 電源ポリシーを有効または無効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="8bb29-200">Specifies whether the default shared PC power policies should be enabled/disabled.</span></span> <span data-ttu-id="8bb29-201">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="8bb29-201">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="8bb29-202">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="8bb29-202">disablePowerPolicies</span></span>|<span data-ttu-id="8bb29-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="8bb29-203">Boolean</span></span>|<span data-ttu-id="8bb29-204">既定の共有 PC 電源ポリシーを無効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="8bb29-204">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="8bb29-205">signInOnResume</span><span class="sxs-lookup"><span data-stu-id="8bb29-205">signInOnResume</span></span>|[<span data-ttu-id="8bb29-206">購入</span><span class="sxs-lookup"><span data-stu-id="8bb29-206">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="8bb29-207">デバイスがスリープモードから復帰したときに毎回サインインする必要があることを指定します。</span><span class="sxs-lookup"><span data-stu-id="8bb29-207">Specifies the requirement to sign in whenever the device wakes up from sleep mode.</span></span> <span data-ttu-id="8bb29-208">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="8bb29-208">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="8bb29-209">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="8bb29-209">disableSignInOnResume</span></span>|<span data-ttu-id="8bb29-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="8bb29-210">Boolean</span></span>|<span data-ttu-id="8bb29-211">デバイスがスリープ モードから再開するたびにサインインを求める設定を無効にします。</span><span class="sxs-lookup"><span data-stu-id="8bb29-211">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="8bb29-212">enabled</span><span class="sxs-lookup"><span data-stu-id="8bb29-212">enabled</span></span>|<span data-ttu-id="8bb29-213">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="8bb29-213">Boolean</span></span>|<span data-ttu-id="8bb29-214">共有 PC モードを有効にし、共有 PC のポリシーを適用します。</span><span class="sxs-lookup"><span data-stu-id="8bb29-214">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="8bb29-215">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="8bb29-215">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="8bb29-216">Int32</span><span class="sxs-lookup"><span data-stu-id="8bb29-216">Int32</span></span>|<span data-ttu-id="8bb29-217">PC がスリープ状態になるまでにデバイスがアイドル状態を続ける時間を秒単位で指定します。</span><span class="sxs-lookup"><span data-stu-id="8bb29-217">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="8bb29-218">この値を 0 に設定すると、スリープ タイムアウトは発生しなくなります。</span><span class="sxs-lookup"><span data-stu-id="8bb29-218">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="8bb29-219">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="8bb29-219">kioskAppDisplayName</span></span>|<span data-ttu-id="8bb29-220">String</span><span class="sxs-lookup"><span data-stu-id="8bb29-220">String</span></span>|<span data-ttu-id="8bb29-221">SetKioskAppUserModelId で指定されたアプリを起動するサインイン画面に表示されるアカウントの表示テキストを指定します。</span><span class="sxs-lookup"><span data-stu-id="8bb29-221">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="8bb29-222">KioskAppUserModelId が設定されている場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="8bb29-222">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="8bb29-223">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="8bb29-223">kioskAppUserModelId</span></span>|<span data-ttu-id="8bb29-224">String</span><span class="sxs-lookup"><span data-stu-id="8bb29-224">String</span></span>|<span data-ttu-id="8bb29-225">割り当てられたアクセスで使用するアプリのアプリケーション ユーザー モデル ID を指定します。</span><span class="sxs-lookup"><span data-stu-id="8bb29-225">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="8bb29-226">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="8bb29-226">maintenanceStartTime</span></span>|<span data-ttu-id="8bb29-227">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="8bb29-227">TimeOfDay</span></span>|<span data-ttu-id="8bb29-228">毎日のメンテナンス時間の開始時刻を指定します。</span><span class="sxs-lookup"><span data-stu-id="8bb29-228">Specifies the daily start time of maintenance hour.</span></span>|
|<span data-ttu-id="8bb29-229">fastFirstSignIn</span><span class="sxs-lookup"><span data-stu-id="8bb29-229">fastFirstSignIn</span></span>|[<span data-ttu-id="8bb29-230">購入</span><span class="sxs-lookup"><span data-stu-id="8bb29-230">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="8bb29-231">管理者以外の新しい Azure AD アカウントを事前に構成された候補ローカルアカウントに自動的に接続するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="8bb29-231">Specifies whether to auto connect new non-admin Azure AD accounts to pre-configured candidate local accounts.</span></span> <span data-ttu-id="8bb29-232">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="8bb29-232">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="8bb29-233">応答</span><span class="sxs-lookup"><span data-stu-id="8bb29-233">Response</span></span>
<span data-ttu-id="8bb29-234">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8bb29-234">If successful, this method returns a `201 Created` response code and a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8bb29-235">例</span><span class="sxs-lookup"><span data-stu-id="8bb29-235">Example</span></span>

### <a name="request"></a><span data-ttu-id="8bb29-236">要求</span><span class="sxs-lookup"><span data-stu-id="8bb29-236">Request</span></span>
<span data-ttu-id="8bb29-237">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8bb29-237">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="8bb29-238">応答</span><span class="sxs-lookup"><span data-stu-id="8bb29-238">Response</span></span>
<span data-ttu-id="8bb29-p121">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8bb29-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




