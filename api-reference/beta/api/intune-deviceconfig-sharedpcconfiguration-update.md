---
title: sharedPCConfiguration の更新
description: sharedPCConfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e5d5de03710f37494243a30a50e1931ac410c2ab
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35946349"
---
# <a name="update-sharedpcconfiguration"></a><span data-ttu-id="f6d97-103">sharedPCConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="f6d97-103">Update sharedPCConfiguration</span></span>

> <span data-ttu-id="f6d97-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f6d97-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6d97-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f6d97-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6d97-106">[sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f6d97-106">Update the properties of a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6d97-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f6d97-107">Prerequisites</span></span>
<span data-ttu-id="f6d97-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f6d97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6d97-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f6d97-110">Permission type</span></span>|<span data-ttu-id="f6d97-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f6d97-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6d97-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f6d97-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f6d97-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6d97-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f6d97-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f6d97-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6d97-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f6d97-115">Not supported.</span></span>|
|<span data-ttu-id="f6d97-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f6d97-116">Application</span></span>|<span data-ttu-id="f6d97-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f6d97-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6d97-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f6d97-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f6d97-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f6d97-119">Request headers</span></span>
|<span data-ttu-id="f6d97-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f6d97-120">Header</span></span>|<span data-ttu-id="f6d97-121">値</span><span class="sxs-lookup"><span data-stu-id="f6d97-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6d97-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6d97-122">Authorization</span></span>|<span data-ttu-id="f6d97-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f6d97-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6d97-124">承諾</span><span class="sxs-lookup"><span data-stu-id="f6d97-124">Accept</span></span>|<span data-ttu-id="f6d97-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f6d97-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6d97-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f6d97-126">Request body</span></span>
<span data-ttu-id="f6d97-127">要求本文で、[sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) オブジェクト用の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f6d97-127">In the request body, supply a JSON representation for the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

<span data-ttu-id="f6d97-128">次の表に、[sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f6d97-128">The following table shows the properties that are required when you create the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span></span>

|<span data-ttu-id="f6d97-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f6d97-129">Property</span></span>|<span data-ttu-id="f6d97-130">型</span><span class="sxs-lookup"><span data-stu-id="f6d97-130">Type</span></span>|<span data-ttu-id="f6d97-131">説明</span><span class="sxs-lookup"><span data-stu-id="f6d97-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6d97-132">id</span><span class="sxs-lookup"><span data-stu-id="f6d97-132">id</span></span>|<span data-ttu-id="f6d97-133">文字列</span><span class="sxs-lookup"><span data-stu-id="f6d97-133">String</span></span>|<span data-ttu-id="f6d97-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f6d97-134">Key of the entity.</span></span> <span data-ttu-id="f6d97-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f6d97-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6d97-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f6d97-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f6d97-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6d97-137">DateTimeOffset</span></span>|<span data-ttu-id="f6d97-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="f6d97-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f6d97-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f6d97-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6d97-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f6d97-140">roleScopeTagIds</span></span>|<span data-ttu-id="f6d97-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="f6d97-141">String collection</span></span>|<span data-ttu-id="f6d97-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="f6d97-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f6d97-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f6d97-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6d97-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f6d97-144">supportsScopeTags</span></span>|<span data-ttu-id="f6d97-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6d97-145">Boolean</span></span>|<span data-ttu-id="f6d97-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f6d97-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f6d97-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="f6d97-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f6d97-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="f6d97-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f6d97-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="f6d97-149">This property is read-only.</span></span> <span data-ttu-id="f6d97-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f6d97-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6d97-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f6d97-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f6d97-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f6d97-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f6d97-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="f6d97-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f6d97-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f6d97-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6d97-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f6d97-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f6d97-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f6d97-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f6d97-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="f6d97-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f6d97-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f6d97-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6d97-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="f6d97-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f6d97-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="f6d97-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f6d97-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="f6d97-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f6d97-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f6d97-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6d97-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f6d97-163">createdDateTime</span></span>|<span data-ttu-id="f6d97-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6d97-164">DateTimeOffset</span></span>|<span data-ttu-id="f6d97-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="f6d97-165">DateTime the object was created.</span></span> <span data-ttu-id="f6d97-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f6d97-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6d97-167">description</span><span class="sxs-lookup"><span data-stu-id="f6d97-167">description</span></span>|<span data-ttu-id="f6d97-168">String</span><span class="sxs-lookup"><span data-stu-id="f6d97-168">String</span></span>|<span data-ttu-id="f6d97-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="f6d97-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f6d97-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f6d97-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6d97-171">displayName</span><span class="sxs-lookup"><span data-stu-id="f6d97-171">displayName</span></span>|<span data-ttu-id="f6d97-172">String</span><span class="sxs-lookup"><span data-stu-id="f6d97-172">String</span></span>|<span data-ttu-id="f6d97-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="f6d97-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f6d97-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f6d97-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6d97-175">version</span><span class="sxs-lookup"><span data-stu-id="f6d97-175">version</span></span>|<span data-ttu-id="f6d97-176">Int32</span><span class="sxs-lookup"><span data-stu-id="f6d97-176">Int32</span></span>|<span data-ttu-id="f6d97-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="f6d97-177">Version of the device configuration.</span></span> <span data-ttu-id="f6d97-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f6d97-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6d97-179">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="f6d97-179">accountManagerPolicy</span></span>|[<span data-ttu-id="f6d97-180">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="f6d97-180">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="f6d97-181">共有の PC 上でアカウントを管理する方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="f6d97-181">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="f6d97-182">disableAccountManager が false の場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="f6d97-182">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="f6d97-183">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="f6d97-183">allowedAccounts</span></span>|[<span data-ttu-id="f6d97-184">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="f6d97-184">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="f6d97-185">共有の PC で使用できるアカウントの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="f6d97-185">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="f6d97-186">可能な値は、`notConfigured`、`guest`、`domain` です。</span><span class="sxs-lookup"><span data-stu-id="f6d97-186">Possible values are: `notConfigured`, `guest`, `domain`.</span></span>|
|<span data-ttu-id="f6d97-187">localStorage</span><span class="sxs-lookup"><span data-stu-id="f6d97-187">localStorage</span></span>|[<span data-ttu-id="f6d97-188">購入</span><span class="sxs-lookup"><span data-stu-id="f6d97-188">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f6d97-189">共有の PC でローカル ストレージを許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="f6d97-189">Specifies whether local storage is allowed on a shared PC.</span></span> <span data-ttu-id="f6d97-190">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="f6d97-190">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="f6d97-191">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="f6d97-191">allowLocalStorage</span></span>|<span data-ttu-id="f6d97-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6d97-192">Boolean</span></span>|<span data-ttu-id="f6d97-193">共有の PC でローカル ストレージを許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="f6d97-193">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="f6d97-194">setAccountManager</span><span class="sxs-lookup"><span data-stu-id="f6d97-194">setAccountManager</span></span>|[<span data-ttu-id="f6d97-195">購入</span><span class="sxs-lookup"><span data-stu-id="f6d97-195">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f6d97-196">共有 PC モードのアカウント マネージャーを無効にします。</span><span class="sxs-lookup"><span data-stu-id="f6d97-196">Disables the account manager for shared PC mode.</span></span> <span data-ttu-id="f6d97-197">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="f6d97-197">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="f6d97-198">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="f6d97-198">disableAccountManager</span></span>|<span data-ttu-id="f6d97-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6d97-199">Boolean</span></span>|<span data-ttu-id="f6d97-200">共有 PC モードのアカウント マネージャーを無効にします。</span><span class="sxs-lookup"><span data-stu-id="f6d97-200">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="f6d97-201">setEduPolicies</span><span class="sxs-lookup"><span data-stu-id="f6d97-201">setEduPolicies</span></span>|[<span data-ttu-id="f6d97-202">購入</span><span class="sxs-lookup"><span data-stu-id="f6d97-202">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f6d97-203">既定の共有 PC 教育環境ポリシーを有効/無効にするか、構成しないかを指定します。</span><span class="sxs-lookup"><span data-stu-id="f6d97-203">Specifies whether the default shared PC education environment policies should be enabled/disabled/not configured.</span></span> <span data-ttu-id="f6d97-204">Windows 10 RS2 以降では、このポリシーは Enabled を true に設定しなくても適用されます。</span><span class="sxs-lookup"><span data-stu-id="f6d97-204">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span> <span data-ttu-id="f6d97-205">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="f6d97-205">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="f6d97-206">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="f6d97-206">disableEduPolicies</span></span>|<span data-ttu-id="f6d97-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6d97-207">Boolean</span></span>|<span data-ttu-id="f6d97-208">既定の共有 PC 教育環境ポリシーを無効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="f6d97-208">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="f6d97-209">Windows 10 RS2 以降では、このポリシーは Enabled を true に設定しなくても適用されます。</span><span class="sxs-lookup"><span data-stu-id="f6d97-209">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="f6d97-210">setPowerPolicies</span><span class="sxs-lookup"><span data-stu-id="f6d97-210">setPowerPolicies</span></span>|[<span data-ttu-id="f6d97-211">購入</span><span class="sxs-lookup"><span data-stu-id="f6d97-211">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f6d97-212">既定の共有 PC 電源ポリシーを有効または無効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="f6d97-212">Specifies whether the default shared PC power policies should be enabled/disabled.</span></span> <span data-ttu-id="f6d97-213">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="f6d97-213">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="f6d97-214">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="f6d97-214">disablePowerPolicies</span></span>|<span data-ttu-id="f6d97-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6d97-215">Boolean</span></span>|<span data-ttu-id="f6d97-216">既定の共有 PC 電源ポリシーを無効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="f6d97-216">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="f6d97-217">signInOnResume</span><span class="sxs-lookup"><span data-stu-id="f6d97-217">signInOnResume</span></span>|[<span data-ttu-id="f6d97-218">購入</span><span class="sxs-lookup"><span data-stu-id="f6d97-218">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f6d97-219">デバイスがスリープモードから復帰したときに毎回サインインする必要があることを指定します。</span><span class="sxs-lookup"><span data-stu-id="f6d97-219">Specifies the requirement to sign in whenever the device wakes up from sleep mode.</span></span> <span data-ttu-id="f6d97-220">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="f6d97-220">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="f6d97-221">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="f6d97-221">disableSignInOnResume</span></span>|<span data-ttu-id="f6d97-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6d97-222">Boolean</span></span>|<span data-ttu-id="f6d97-223">デバイスがスリープ モードから再開するたびにサインインを求める設定を無効にします。</span><span class="sxs-lookup"><span data-stu-id="f6d97-223">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="f6d97-224">enabled</span><span class="sxs-lookup"><span data-stu-id="f6d97-224">enabled</span></span>|<span data-ttu-id="f6d97-225">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="f6d97-225">Boolean</span></span>|<span data-ttu-id="f6d97-226">共有 PC モードを有効にし、共有 PC のポリシーを適用します。</span><span class="sxs-lookup"><span data-stu-id="f6d97-226">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="f6d97-227">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="f6d97-227">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="f6d97-228">Int32</span><span class="sxs-lookup"><span data-stu-id="f6d97-228">Int32</span></span>|<span data-ttu-id="f6d97-229">PC がスリープ状態になるまでにデバイスがアイドル状態を続ける時間を秒単位で指定します。</span><span class="sxs-lookup"><span data-stu-id="f6d97-229">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="f6d97-230">この値を 0 に設定すると、スリープ タイムアウトは発生しなくなります。</span><span class="sxs-lookup"><span data-stu-id="f6d97-230">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="f6d97-231">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="f6d97-231">kioskAppDisplayName</span></span>|<span data-ttu-id="f6d97-232">String</span><span class="sxs-lookup"><span data-stu-id="f6d97-232">String</span></span>|<span data-ttu-id="f6d97-233">SetKioskAppUserModelId で指定されたアプリを起動するサインイン画面に表示されるアカウントの表示テキストを指定します。</span><span class="sxs-lookup"><span data-stu-id="f6d97-233">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="f6d97-234">KioskAppUserModelId が設定されている場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="f6d97-234">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="f6d97-235">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="f6d97-235">kioskAppUserModelId</span></span>|<span data-ttu-id="f6d97-236">String</span><span class="sxs-lookup"><span data-stu-id="f6d97-236">String</span></span>|<span data-ttu-id="f6d97-237">割り当てられたアクセスで使用するアプリのアプリケーション ユーザー モデル ID を指定します。</span><span class="sxs-lookup"><span data-stu-id="f6d97-237">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="f6d97-238">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="f6d97-238">maintenanceStartTime</span></span>|<span data-ttu-id="f6d97-239">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="f6d97-239">TimeOfDay</span></span>|<span data-ttu-id="f6d97-240">毎日のメンテナンス時間の開始時刻を指定します。</span><span class="sxs-lookup"><span data-stu-id="f6d97-240">Specifies the daily start time of maintenance hour.</span></span>|
|<span data-ttu-id="f6d97-241">fastFirstSignIn</span><span class="sxs-lookup"><span data-stu-id="f6d97-241">fastFirstSignIn</span></span>|[<span data-ttu-id="f6d97-242">購入</span><span class="sxs-lookup"><span data-stu-id="f6d97-242">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f6d97-243">管理者以外の新しい Azure AD アカウントを事前に構成された候補ローカルアカウントに自動的に接続するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="f6d97-243">Specifies whether to auto connect new non-admin Azure AD accounts to pre-configured candidate local accounts.</span></span> <span data-ttu-id="f6d97-244">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="f6d97-244">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="f6d97-245">応答</span><span class="sxs-lookup"><span data-stu-id="f6d97-245">Response</span></span>
<span data-ttu-id="f6d97-246">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="f6d97-246">If successful, this method returns a `200 OK` response code and an updated [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6d97-247">例</span><span class="sxs-lookup"><span data-stu-id="f6d97-247">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6d97-248">要求</span><span class="sxs-lookup"><span data-stu-id="f6d97-248">Request</span></span>
<span data-ttu-id="f6d97-249">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f6d97-249">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f6d97-250">応答</span><span class="sxs-lookup"><span data-stu-id="f6d97-250">Response</span></span>
<span data-ttu-id="f6d97-p124">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f6d97-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





