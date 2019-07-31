---
title: Create sharedPCConfiguration
description: 新しい sharedPCConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9e60231d60494df23f60dbd007f1c2cb702adc59
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35946405"
---
# <a name="create-sharedpcconfiguration"></a><span data-ttu-id="297aa-103">Create sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="297aa-103">Create sharedPCConfiguration</span></span>

> <span data-ttu-id="297aa-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="297aa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="297aa-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="297aa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="297aa-106">新しい [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="297aa-106">Create a new [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="297aa-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="297aa-107">Prerequisites</span></span>
<span data-ttu-id="297aa-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="297aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="297aa-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="297aa-110">Permission type</span></span>|<span data-ttu-id="297aa-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="297aa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="297aa-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="297aa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="297aa-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="297aa-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="297aa-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="297aa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="297aa-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="297aa-115">Not supported.</span></span>|
|<span data-ttu-id="297aa-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="297aa-116">Application</span></span>|<span data-ttu-id="297aa-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="297aa-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="297aa-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="297aa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="297aa-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="297aa-119">Request headers</span></span>
|<span data-ttu-id="297aa-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="297aa-120">Header</span></span>|<span data-ttu-id="297aa-121">値</span><span class="sxs-lookup"><span data-stu-id="297aa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="297aa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="297aa-122">Authorization</span></span>|<span data-ttu-id="297aa-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="297aa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="297aa-124">承諾</span><span class="sxs-lookup"><span data-stu-id="297aa-124">Accept</span></span>|<span data-ttu-id="297aa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="297aa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="297aa-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="297aa-126">Request body</span></span>
<span data-ttu-id="297aa-127">要求本文で、sharedPCConfiguration オブジェクト用の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="297aa-127">In the request body, supply a JSON representation for the sharedPCConfiguration object.</span></span>

<span data-ttu-id="297aa-128">次の表に、sharedPCConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="297aa-128">The following table shows the properties that are required when you create the sharedPCConfiguration.</span></span>

|<span data-ttu-id="297aa-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="297aa-129">Property</span></span>|<span data-ttu-id="297aa-130">型</span><span class="sxs-lookup"><span data-stu-id="297aa-130">Type</span></span>|<span data-ttu-id="297aa-131">説明</span><span class="sxs-lookup"><span data-stu-id="297aa-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="297aa-132">id</span><span class="sxs-lookup"><span data-stu-id="297aa-132">id</span></span>|<span data-ttu-id="297aa-133">文字列</span><span class="sxs-lookup"><span data-stu-id="297aa-133">String</span></span>|<span data-ttu-id="297aa-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="297aa-134">Key of the entity.</span></span> <span data-ttu-id="297aa-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="297aa-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="297aa-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="297aa-136">lastModifiedDateTime</span></span>|<span data-ttu-id="297aa-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="297aa-137">DateTimeOffset</span></span>|<span data-ttu-id="297aa-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="297aa-138">DateTime the object was last modified.</span></span> <span data-ttu-id="297aa-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="297aa-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="297aa-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="297aa-140">roleScopeTagIds</span></span>|<span data-ttu-id="297aa-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="297aa-141">String collection</span></span>|<span data-ttu-id="297aa-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="297aa-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="297aa-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="297aa-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="297aa-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="297aa-144">supportsScopeTags</span></span>|<span data-ttu-id="297aa-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="297aa-145">Boolean</span></span>|<span data-ttu-id="297aa-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="297aa-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="297aa-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="297aa-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="297aa-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="297aa-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="297aa-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="297aa-149">This property is read-only.</span></span> <span data-ttu-id="297aa-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="297aa-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="297aa-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="297aa-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="297aa-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="297aa-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="297aa-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="297aa-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="297aa-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="297aa-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="297aa-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="297aa-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="297aa-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="297aa-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="297aa-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="297aa-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="297aa-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="297aa-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="297aa-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="297aa-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="297aa-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="297aa-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="297aa-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="297aa-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="297aa-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="297aa-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="297aa-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="297aa-163">createdDateTime</span></span>|<span data-ttu-id="297aa-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="297aa-164">DateTimeOffset</span></span>|<span data-ttu-id="297aa-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="297aa-165">DateTime the object was created.</span></span> <span data-ttu-id="297aa-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="297aa-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="297aa-167">description</span><span class="sxs-lookup"><span data-stu-id="297aa-167">description</span></span>|<span data-ttu-id="297aa-168">String</span><span class="sxs-lookup"><span data-stu-id="297aa-168">String</span></span>|<span data-ttu-id="297aa-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="297aa-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="297aa-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="297aa-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="297aa-171">displayName</span><span class="sxs-lookup"><span data-stu-id="297aa-171">displayName</span></span>|<span data-ttu-id="297aa-172">String</span><span class="sxs-lookup"><span data-stu-id="297aa-172">String</span></span>|<span data-ttu-id="297aa-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="297aa-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="297aa-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="297aa-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="297aa-175">version</span><span class="sxs-lookup"><span data-stu-id="297aa-175">version</span></span>|<span data-ttu-id="297aa-176">Int32</span><span class="sxs-lookup"><span data-stu-id="297aa-176">Int32</span></span>|<span data-ttu-id="297aa-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="297aa-177">Version of the device configuration.</span></span> <span data-ttu-id="297aa-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="297aa-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="297aa-179">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="297aa-179">accountManagerPolicy</span></span>|[<span data-ttu-id="297aa-180">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="297aa-180">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="297aa-181">共有の PC 上でアカウントを管理する方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="297aa-181">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="297aa-182">disableAccountManager が false の場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="297aa-182">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="297aa-183">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="297aa-183">allowedAccounts</span></span>|[<span data-ttu-id="297aa-184">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="297aa-184">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="297aa-185">共有の PC で使用できるアカウントの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="297aa-185">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="297aa-186">可能な値は、`notConfigured`、`guest`、`domain` です。</span><span class="sxs-lookup"><span data-stu-id="297aa-186">Possible values are: `notConfigured`, `guest`, `domain`.</span></span>|
|<span data-ttu-id="297aa-187">localStorage</span><span class="sxs-lookup"><span data-stu-id="297aa-187">localStorage</span></span>|[<span data-ttu-id="297aa-188">購入</span><span class="sxs-lookup"><span data-stu-id="297aa-188">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="297aa-189">共有の PC でローカル ストレージを許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="297aa-189">Specifies whether local storage is allowed on a shared PC.</span></span> <span data-ttu-id="297aa-190">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="297aa-190">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="297aa-191">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="297aa-191">allowLocalStorage</span></span>|<span data-ttu-id="297aa-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="297aa-192">Boolean</span></span>|<span data-ttu-id="297aa-193">共有の PC でローカル ストレージを許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="297aa-193">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="297aa-194">setAccountManager</span><span class="sxs-lookup"><span data-stu-id="297aa-194">setAccountManager</span></span>|[<span data-ttu-id="297aa-195">購入</span><span class="sxs-lookup"><span data-stu-id="297aa-195">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="297aa-196">共有 PC モードのアカウント マネージャーを無効にします。</span><span class="sxs-lookup"><span data-stu-id="297aa-196">Disables the account manager for shared PC mode.</span></span> <span data-ttu-id="297aa-197">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="297aa-197">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="297aa-198">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="297aa-198">disableAccountManager</span></span>|<span data-ttu-id="297aa-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="297aa-199">Boolean</span></span>|<span data-ttu-id="297aa-200">共有 PC モードのアカウント マネージャーを無効にします。</span><span class="sxs-lookup"><span data-stu-id="297aa-200">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="297aa-201">setEduPolicies</span><span class="sxs-lookup"><span data-stu-id="297aa-201">setEduPolicies</span></span>|[<span data-ttu-id="297aa-202">購入</span><span class="sxs-lookup"><span data-stu-id="297aa-202">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="297aa-203">既定の共有 PC 教育環境ポリシーを有効/無効にするか、構成しないかを指定します。</span><span class="sxs-lookup"><span data-stu-id="297aa-203">Specifies whether the default shared PC education environment policies should be enabled/disabled/not configured.</span></span> <span data-ttu-id="297aa-204">Windows 10 RS2 以降では、このポリシーは Enabled を true に設定しなくても適用されます。</span><span class="sxs-lookup"><span data-stu-id="297aa-204">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span> <span data-ttu-id="297aa-205">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="297aa-205">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="297aa-206">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="297aa-206">disableEduPolicies</span></span>|<span data-ttu-id="297aa-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="297aa-207">Boolean</span></span>|<span data-ttu-id="297aa-208">既定の共有 PC 教育環境ポリシーを無効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="297aa-208">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="297aa-209">Windows 10 RS2 以降では、このポリシーは Enabled を true に設定しなくても適用されます。</span><span class="sxs-lookup"><span data-stu-id="297aa-209">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="297aa-210">setPowerPolicies</span><span class="sxs-lookup"><span data-stu-id="297aa-210">setPowerPolicies</span></span>|[<span data-ttu-id="297aa-211">購入</span><span class="sxs-lookup"><span data-stu-id="297aa-211">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="297aa-212">既定の共有 PC 電源ポリシーを有効または無効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="297aa-212">Specifies whether the default shared PC power policies should be enabled/disabled.</span></span> <span data-ttu-id="297aa-213">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="297aa-213">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="297aa-214">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="297aa-214">disablePowerPolicies</span></span>|<span data-ttu-id="297aa-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="297aa-215">Boolean</span></span>|<span data-ttu-id="297aa-216">既定の共有 PC 電源ポリシーを無効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="297aa-216">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="297aa-217">signInOnResume</span><span class="sxs-lookup"><span data-stu-id="297aa-217">signInOnResume</span></span>|[<span data-ttu-id="297aa-218">購入</span><span class="sxs-lookup"><span data-stu-id="297aa-218">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="297aa-219">デバイスがスリープモードから復帰したときに毎回サインインする必要があることを指定します。</span><span class="sxs-lookup"><span data-stu-id="297aa-219">Specifies the requirement to sign in whenever the device wakes up from sleep mode.</span></span> <span data-ttu-id="297aa-220">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="297aa-220">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="297aa-221">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="297aa-221">disableSignInOnResume</span></span>|<span data-ttu-id="297aa-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="297aa-222">Boolean</span></span>|<span data-ttu-id="297aa-223">デバイスがスリープ モードから再開するたびにサインインを求める設定を無効にします。</span><span class="sxs-lookup"><span data-stu-id="297aa-223">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="297aa-224">enabled</span><span class="sxs-lookup"><span data-stu-id="297aa-224">enabled</span></span>|<span data-ttu-id="297aa-225">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="297aa-225">Boolean</span></span>|<span data-ttu-id="297aa-226">共有 PC モードを有効にし、共有 PC のポリシーを適用します。</span><span class="sxs-lookup"><span data-stu-id="297aa-226">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="297aa-227">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="297aa-227">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="297aa-228">Int32</span><span class="sxs-lookup"><span data-stu-id="297aa-228">Int32</span></span>|<span data-ttu-id="297aa-229">PC がスリープ状態になるまでにデバイスがアイドル状態を続ける時間を秒単位で指定します。</span><span class="sxs-lookup"><span data-stu-id="297aa-229">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="297aa-230">この値を 0 に設定すると、スリープ タイムアウトは発生しなくなります。</span><span class="sxs-lookup"><span data-stu-id="297aa-230">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="297aa-231">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="297aa-231">kioskAppDisplayName</span></span>|<span data-ttu-id="297aa-232">String</span><span class="sxs-lookup"><span data-stu-id="297aa-232">String</span></span>|<span data-ttu-id="297aa-233">SetKioskAppUserModelId で指定されたアプリを起動するサインイン画面に表示されるアカウントの表示テキストを指定します。</span><span class="sxs-lookup"><span data-stu-id="297aa-233">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="297aa-234">KioskAppUserModelId が設定されている場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="297aa-234">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="297aa-235">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="297aa-235">kioskAppUserModelId</span></span>|<span data-ttu-id="297aa-236">String</span><span class="sxs-lookup"><span data-stu-id="297aa-236">String</span></span>|<span data-ttu-id="297aa-237">割り当てられたアクセスで使用するアプリのアプリケーション ユーザー モデル ID を指定します。</span><span class="sxs-lookup"><span data-stu-id="297aa-237">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="297aa-238">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="297aa-238">maintenanceStartTime</span></span>|<span data-ttu-id="297aa-239">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="297aa-239">TimeOfDay</span></span>|<span data-ttu-id="297aa-240">毎日のメンテナンス時間の開始時刻を指定します。</span><span class="sxs-lookup"><span data-stu-id="297aa-240">Specifies the daily start time of maintenance hour.</span></span>|
|<span data-ttu-id="297aa-241">fastFirstSignIn</span><span class="sxs-lookup"><span data-stu-id="297aa-241">fastFirstSignIn</span></span>|[<span data-ttu-id="297aa-242">購入</span><span class="sxs-lookup"><span data-stu-id="297aa-242">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="297aa-243">管理者以外の新しい Azure AD アカウントを事前に構成された候補ローカルアカウントに自動的に接続するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="297aa-243">Specifies whether to auto connect new non-admin Azure AD accounts to pre-configured candidate local accounts.</span></span> <span data-ttu-id="297aa-244">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="297aa-244">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="297aa-245">応答</span><span class="sxs-lookup"><span data-stu-id="297aa-245">Response</span></span>
<span data-ttu-id="297aa-246">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="297aa-246">If successful, this method returns a `201 Created` response code and a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="297aa-247">例</span><span class="sxs-lookup"><span data-stu-id="297aa-247">Example</span></span>

### <a name="request"></a><span data-ttu-id="297aa-248">要求</span><span class="sxs-lookup"><span data-stu-id="297aa-248">Request</span></span>
<span data-ttu-id="297aa-249">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="297aa-249">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="297aa-250">応答</span><span class="sxs-lookup"><span data-stu-id="297aa-250">Response</span></span>
<span data-ttu-id="297aa-p124">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="297aa-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





