---
title: sharedPCConfiguration の更新
description: sharedPCConfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9ce52841d71714dd4ebcd0226de2918de7ce4c58
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36314827"
---
# <a name="update-sharedpcconfiguration"></a><span data-ttu-id="ae276-103">sharedPCConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="ae276-103">Update sharedPCConfiguration</span></span>

> <span data-ttu-id="ae276-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae276-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae276-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ae276-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae276-106">[sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ae276-106">Update the properties of a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae276-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="ae276-107">Prerequisites</span></span>
<span data-ttu-id="ae276-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae276-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae276-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ae276-110">Permission type</span></span>|<span data-ttu-id="ae276-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ae276-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae276-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ae276-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ae276-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae276-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ae276-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ae276-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae276-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae276-115">Not supported.</span></span>|
|<span data-ttu-id="ae276-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ae276-116">Application</span></span>|<span data-ttu-id="ae276-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae276-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae276-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ae276-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ae276-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ae276-119">Request headers</span></span>
|<span data-ttu-id="ae276-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ae276-120">Header</span></span>|<span data-ttu-id="ae276-121">値</span><span class="sxs-lookup"><span data-stu-id="ae276-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae276-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae276-122">Authorization</span></span>|<span data-ttu-id="ae276-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ae276-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae276-124">承諾</span><span class="sxs-lookup"><span data-stu-id="ae276-124">Accept</span></span>|<span data-ttu-id="ae276-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ae276-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae276-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ae276-126">Request body</span></span>
<span data-ttu-id="ae276-127">要求本文で、[sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) オブジェクト用の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ae276-127">In the request body, supply a JSON representation for the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

<span data-ttu-id="ae276-128">次の表に、[sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ae276-128">The following table shows the properties that are required when you create the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span></span>

|<span data-ttu-id="ae276-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ae276-129">Property</span></span>|<span data-ttu-id="ae276-130">型</span><span class="sxs-lookup"><span data-stu-id="ae276-130">Type</span></span>|<span data-ttu-id="ae276-131">説明</span><span class="sxs-lookup"><span data-stu-id="ae276-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae276-132">id</span><span class="sxs-lookup"><span data-stu-id="ae276-132">id</span></span>|<span data-ttu-id="ae276-133">文字列</span><span class="sxs-lookup"><span data-stu-id="ae276-133">String</span></span>|<span data-ttu-id="ae276-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ae276-134">Key of the entity.</span></span> <span data-ttu-id="ae276-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ae276-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae276-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ae276-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ae276-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae276-137">DateTimeOffset</span></span>|<span data-ttu-id="ae276-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="ae276-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ae276-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ae276-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae276-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ae276-140">roleScopeTagIds</span></span>|<span data-ttu-id="ae276-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="ae276-141">String collection</span></span>|<span data-ttu-id="ae276-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="ae276-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ae276-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ae276-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae276-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ae276-144">supportsScopeTags</span></span>|<span data-ttu-id="ae276-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae276-145">Boolean</span></span>|<span data-ttu-id="ae276-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ae276-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ae276-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="ae276-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ae276-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="ae276-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ae276-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="ae276-149">This property is read-only.</span></span> <span data-ttu-id="ae276-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ae276-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae276-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ae276-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ae276-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ae276-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ae276-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="ae276-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ae276-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ae276-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae276-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ae276-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ae276-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ae276-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ae276-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="ae276-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ae276-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ae276-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae276-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="ae276-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ae276-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="ae276-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ae276-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="ae276-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ae276-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ae276-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae276-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ae276-163">createdDateTime</span></span>|<span data-ttu-id="ae276-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae276-164">DateTimeOffset</span></span>|<span data-ttu-id="ae276-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="ae276-165">DateTime the object was created.</span></span> <span data-ttu-id="ae276-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ae276-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae276-167">description</span><span class="sxs-lookup"><span data-stu-id="ae276-167">description</span></span>|<span data-ttu-id="ae276-168">String</span><span class="sxs-lookup"><span data-stu-id="ae276-168">String</span></span>|<span data-ttu-id="ae276-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="ae276-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ae276-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ae276-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae276-171">displayName</span><span class="sxs-lookup"><span data-stu-id="ae276-171">displayName</span></span>|<span data-ttu-id="ae276-172">String</span><span class="sxs-lookup"><span data-stu-id="ae276-172">String</span></span>|<span data-ttu-id="ae276-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="ae276-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ae276-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ae276-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae276-175">version</span><span class="sxs-lookup"><span data-stu-id="ae276-175">version</span></span>|<span data-ttu-id="ae276-176">Int32</span><span class="sxs-lookup"><span data-stu-id="ae276-176">Int32</span></span>|<span data-ttu-id="ae276-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="ae276-177">Version of the device configuration.</span></span> <span data-ttu-id="ae276-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ae276-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae276-179">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="ae276-179">accountManagerPolicy</span></span>|[<span data-ttu-id="ae276-180">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="ae276-180">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="ae276-181">共有の PC 上でアカウントを管理する方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="ae276-181">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="ae276-182">disableAccountManager が false の場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="ae276-182">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="ae276-183">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="ae276-183">allowedAccounts</span></span>|[<span data-ttu-id="ae276-184">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="ae276-184">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="ae276-185">共有の PC で使用できるアカウントの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="ae276-185">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="ae276-186">可能な値は、`notConfigured`、`guest`、`domain` です。</span><span class="sxs-lookup"><span data-stu-id="ae276-186">Possible values are: `notConfigured`, `guest`, `domain`.</span></span>|
|<span data-ttu-id="ae276-187">localStorage</span><span class="sxs-lookup"><span data-stu-id="ae276-187">localStorage</span></span>|[<span data-ttu-id="ae276-188">購入</span><span class="sxs-lookup"><span data-stu-id="ae276-188">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="ae276-189">共有の PC でローカル ストレージを許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="ae276-189">Specifies whether local storage is allowed on a shared PC.</span></span> <span data-ttu-id="ae276-190">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="ae276-190">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="ae276-191">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="ae276-191">allowLocalStorage</span></span>|<span data-ttu-id="ae276-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae276-192">Boolean</span></span>|<span data-ttu-id="ae276-193">共有の PC でローカル ストレージを許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="ae276-193">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="ae276-194">setAccountManager</span><span class="sxs-lookup"><span data-stu-id="ae276-194">setAccountManager</span></span>|[<span data-ttu-id="ae276-195">購入</span><span class="sxs-lookup"><span data-stu-id="ae276-195">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="ae276-196">共有 PC モードのアカウント マネージャーを無効にします。</span><span class="sxs-lookup"><span data-stu-id="ae276-196">Disables the account manager for shared PC mode.</span></span> <span data-ttu-id="ae276-197">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="ae276-197">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="ae276-198">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="ae276-198">disableAccountManager</span></span>|<span data-ttu-id="ae276-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae276-199">Boolean</span></span>|<span data-ttu-id="ae276-200">共有 PC モードのアカウント マネージャーを無効にします。</span><span class="sxs-lookup"><span data-stu-id="ae276-200">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="ae276-201">setEduPolicies</span><span class="sxs-lookup"><span data-stu-id="ae276-201">setEduPolicies</span></span>|[<span data-ttu-id="ae276-202">購入</span><span class="sxs-lookup"><span data-stu-id="ae276-202">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="ae276-203">既定の共有 PC 教育環境ポリシーを有効/無効にするか、構成しないかを指定します。</span><span class="sxs-lookup"><span data-stu-id="ae276-203">Specifies whether the default shared PC education environment policies should be enabled/disabled/not configured.</span></span> <span data-ttu-id="ae276-204">Windows 10 RS2 以降では、このポリシーは Enabled を true に設定しなくても適用されます。</span><span class="sxs-lookup"><span data-stu-id="ae276-204">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span> <span data-ttu-id="ae276-205">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="ae276-205">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="ae276-206">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="ae276-206">disableEduPolicies</span></span>|<span data-ttu-id="ae276-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae276-207">Boolean</span></span>|<span data-ttu-id="ae276-208">既定の共有 PC 教育環境ポリシーを無効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="ae276-208">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="ae276-209">Windows 10 RS2 以降では、このポリシーは Enabled を true に設定しなくても適用されます。</span><span class="sxs-lookup"><span data-stu-id="ae276-209">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="ae276-210">setPowerPolicies</span><span class="sxs-lookup"><span data-stu-id="ae276-210">setPowerPolicies</span></span>|[<span data-ttu-id="ae276-211">購入</span><span class="sxs-lookup"><span data-stu-id="ae276-211">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="ae276-212">既定の共有 PC 電源ポリシーを有効または無効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="ae276-212">Specifies whether the default shared PC power policies should be enabled/disabled.</span></span> <span data-ttu-id="ae276-213">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="ae276-213">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="ae276-214">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="ae276-214">disablePowerPolicies</span></span>|<span data-ttu-id="ae276-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae276-215">Boolean</span></span>|<span data-ttu-id="ae276-216">既定の共有 PC 電源ポリシーを無効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="ae276-216">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="ae276-217">signInOnResume</span><span class="sxs-lookup"><span data-stu-id="ae276-217">signInOnResume</span></span>|[<span data-ttu-id="ae276-218">購入</span><span class="sxs-lookup"><span data-stu-id="ae276-218">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="ae276-219">デバイスがスリープモードから復帰したときに毎回サインインする必要があることを指定します。</span><span class="sxs-lookup"><span data-stu-id="ae276-219">Specifies the requirement to sign in whenever the device wakes up from sleep mode.</span></span> <span data-ttu-id="ae276-220">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="ae276-220">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="ae276-221">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="ae276-221">disableSignInOnResume</span></span>|<span data-ttu-id="ae276-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae276-222">Boolean</span></span>|<span data-ttu-id="ae276-223">デバイスがスリープ モードから再開するたびにサインインを求める設定を無効にします。</span><span class="sxs-lookup"><span data-stu-id="ae276-223">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="ae276-224">enabled</span><span class="sxs-lookup"><span data-stu-id="ae276-224">enabled</span></span>|<span data-ttu-id="ae276-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae276-225">Boolean</span></span>|<span data-ttu-id="ae276-226">共有 PC モードを有効にし、共有 PC のポリシーを適用します。</span><span class="sxs-lookup"><span data-stu-id="ae276-226">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="ae276-227">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="ae276-227">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="ae276-228">Int32</span><span class="sxs-lookup"><span data-stu-id="ae276-228">Int32</span></span>|<span data-ttu-id="ae276-229">PC がスリープ状態になるまでにデバイスがアイドル状態を続ける時間を秒単位で指定します。</span><span class="sxs-lookup"><span data-stu-id="ae276-229">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="ae276-230">この値を 0 に設定すると、スリープ タイムアウトは発生しなくなります。</span><span class="sxs-lookup"><span data-stu-id="ae276-230">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="ae276-231">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="ae276-231">kioskAppDisplayName</span></span>|<span data-ttu-id="ae276-232">String</span><span class="sxs-lookup"><span data-stu-id="ae276-232">String</span></span>|<span data-ttu-id="ae276-233">SetKioskAppUserModelId で指定されたアプリを起動するサインイン画面に表示されるアカウントの表示テキストを指定します。</span><span class="sxs-lookup"><span data-stu-id="ae276-233">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="ae276-234">KioskAppUserModelId が設定されている場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="ae276-234">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="ae276-235">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="ae276-235">kioskAppUserModelId</span></span>|<span data-ttu-id="ae276-236">String</span><span class="sxs-lookup"><span data-stu-id="ae276-236">String</span></span>|<span data-ttu-id="ae276-237">割り当てられたアクセスで使用するアプリのアプリケーション ユーザー モデル ID を指定します。</span><span class="sxs-lookup"><span data-stu-id="ae276-237">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="ae276-238">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="ae276-238">maintenanceStartTime</span></span>|<span data-ttu-id="ae276-239">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="ae276-239">TimeOfDay</span></span>|<span data-ttu-id="ae276-240">毎日のメンテナンス時間の開始時刻を指定します。</span><span class="sxs-lookup"><span data-stu-id="ae276-240">Specifies the daily start time of maintenance hour.</span></span>|
|<span data-ttu-id="ae276-241">fastFirstSignIn</span><span class="sxs-lookup"><span data-stu-id="ae276-241">fastFirstSignIn</span></span>|[<span data-ttu-id="ae276-242">購入</span><span class="sxs-lookup"><span data-stu-id="ae276-242">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="ae276-243">管理者以外の新しい Azure AD アカウントを事前に構成された候補ローカルアカウントに自動的に接続するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="ae276-243">Specifies whether to auto connect new non-admin Azure AD accounts to pre-configured candidate local accounts.</span></span> <span data-ttu-id="ae276-244">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="ae276-244">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="ae276-245">応答</span><span class="sxs-lookup"><span data-stu-id="ae276-245">Response</span></span>
<span data-ttu-id="ae276-246">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="ae276-246">If successful, this method returns a `200 OK` response code and an updated [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae276-247">例</span><span class="sxs-lookup"><span data-stu-id="ae276-247">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae276-248">要求</span><span class="sxs-lookup"><span data-stu-id="ae276-248">Request</span></span>
<span data-ttu-id="ae276-249">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ae276-249">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1920

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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

### <a name="response"></a><span data-ttu-id="ae276-250">応答</span><span class="sxs-lookup"><span data-stu-id="ae276-250">Response</span></span>
<span data-ttu-id="ae276-p124">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ae276-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2092

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "id": "5206be3b-be3b-5206-3bbe-06523bbe0652",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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






