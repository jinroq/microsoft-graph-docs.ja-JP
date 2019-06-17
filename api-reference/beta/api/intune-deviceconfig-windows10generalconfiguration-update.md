---
title: Update windows10GeneralConfiguration
description: windows10GeneralConfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 60c9585de891471358eb6a56e5cd91d9b848fd16
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34975981"
---
# <a name="update-windows10generalconfiguration"></a><span data-ttu-id="ad9c7-103">Update windows10GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="ad9c7-103">Update windows10GeneralConfiguration</span></span>

> <span data-ttu-id="ad9c7-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ad9c7-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad9c7-106">[windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-106">Update the properties of a [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ad9c7-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="ad9c7-107">Prerequisites</span></span>
<span data-ttu-id="ad9c7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad9c7-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ad9c7-110">Permission type</span></span>|<span data-ttu-id="ad9c7-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ad9c7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad9c7-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ad9c7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ad9c7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad9c7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ad9c7-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ad9c7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad9c7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-115">Not supported.</span></span>|
|<span data-ttu-id="ad9c7-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ad9c7-116">Application</span></span>|<span data-ttu-id="ad9c7-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad9c7-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ad9c7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ad9c7-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ad9c7-119">Request headers</span></span>
|<span data-ttu-id="ad9c7-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ad9c7-120">Header</span></span>|<span data-ttu-id="ad9c7-121">値</span><span class="sxs-lookup"><span data-stu-id="ad9c7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad9c7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad9c7-122">Authorization</span></span>|<span data-ttu-id="ad9c7-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad9c7-124">承諾</span><span class="sxs-lookup"><span data-stu-id="ad9c7-124">Accept</span></span>|<span data-ttu-id="ad9c7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ad9c7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad9c7-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ad9c7-126">Request body</span></span>
<span data-ttu-id="ad9c7-127">要求本文で、[windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-127">In the request body, supply a JSON representation for the [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object.</span></span>

<span data-ttu-id="ad9c7-128">次の表に、[windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-128">The following table shows the properties that are required when you create the [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).</span></span>

|<span data-ttu-id="ad9c7-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ad9c7-129">Property</span></span>|<span data-ttu-id="ad9c7-130">型</span><span class="sxs-lookup"><span data-stu-id="ad9c7-130">Type</span></span>|<span data-ttu-id="ad9c7-131">説明</span><span class="sxs-lookup"><span data-stu-id="ad9c7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad9c7-132">id</span><span class="sxs-lookup"><span data-stu-id="ad9c7-132">id</span></span>|<span data-ttu-id="ad9c7-133">文字列</span><span class="sxs-lookup"><span data-stu-id="ad9c7-133">String</span></span>|<span data-ttu-id="ad9c7-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-134">Key of the entity.</span></span> <span data-ttu-id="ad9c7-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ad9c7-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad9c7-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ad9c7-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ad9c7-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad9c7-137">DateTimeOffset</span></span>|<span data-ttu-id="ad9c7-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ad9c7-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ad9c7-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad9c7-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ad9c7-140">roleScopeTagIds</span></span>|<span data-ttu-id="ad9c7-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="ad9c7-141">String collection</span></span>|<span data-ttu-id="ad9c7-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ad9c7-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ad9c7-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad9c7-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ad9c7-144">supportsScopeTags</span></span>|<span data-ttu-id="ad9c7-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-145">Boolean</span></span>|<span data-ttu-id="ad9c7-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ad9c7-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ad9c7-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ad9c7-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-149">This property is read-only.</span></span> <span data-ttu-id="ad9c7-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ad9c7-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad9c7-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ad9c7-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ad9c7-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ad9c7-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ad9c7-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ad9c7-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ad9c7-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad9c7-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ad9c7-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ad9c7-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ad9c7-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ad9c7-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ad9c7-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ad9c7-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad9c7-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="ad9c7-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ad9c7-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="ad9c7-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ad9c7-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ad9c7-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ad9c7-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad9c7-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ad9c7-163">createdDateTime</span></span>|<span data-ttu-id="ad9c7-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad9c7-164">DateTimeOffset</span></span>|<span data-ttu-id="ad9c7-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-165">DateTime the object was created.</span></span> <span data-ttu-id="ad9c7-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ad9c7-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad9c7-167">description</span><span class="sxs-lookup"><span data-stu-id="ad9c7-167">description</span></span>|<span data-ttu-id="ad9c7-168">String</span><span class="sxs-lookup"><span data-stu-id="ad9c7-168">String</span></span>|<span data-ttu-id="ad9c7-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ad9c7-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ad9c7-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad9c7-171">displayName</span><span class="sxs-lookup"><span data-stu-id="ad9c7-171">displayName</span></span>|<span data-ttu-id="ad9c7-172">String</span><span class="sxs-lookup"><span data-stu-id="ad9c7-172">String</span></span>|<span data-ttu-id="ad9c7-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ad9c7-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ad9c7-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad9c7-175">version</span><span class="sxs-lookup"><span data-stu-id="ad9c7-175">version</span></span>|<span data-ttu-id="ad9c7-176">Int32</span><span class="sxs-lookup"><span data-stu-id="ad9c7-176">Int32</span></span>|<span data-ttu-id="ad9c7-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-177">Version of the device configuration.</span></span> <span data-ttu-id="ad9c7-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ad9c7-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad9c7-179">taskManagerBlockEndTask</span><span class="sxs-lookup"><span data-stu-id="ad9c7-179">taskManagerBlockEndTask</span></span>|<span data-ttu-id="ad9c7-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-180">Boolean</span></span>|<span data-ttu-id="ad9c7-181">管理者以外がタスクマネージャーを使用してタスクを終了できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-181">Specify whether non-administrators can use Task Manager to end tasks.</span></span>|
|<span data-ttu-id="ad9c7-182">windows10AppsForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="ad9c7-182">windows10AppsForceUpdateSchedule</span></span>|[<span data-ttu-id="ad9c7-183">windows10AppsForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="ad9c7-183">windows10AppsForceUpdateSchedule</span></span>](../resources/intune-deviceconfig-windows10appsforceupdateschedule.md)|<span data-ttu-id="ad9c7-184">Windows 10 アプリの更新スケジュールを強制します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-184">Windows 10 force update schedule for Apps.</span></span>|
|<span data-ttu-id="ad9c7-185">Enable自動再展開</span><span class="sxs-lookup"><span data-stu-id="ad9c7-185">enableAutomaticRedeployment</span></span>|<span data-ttu-id="ad9c7-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-186">Boolean</span></span>|<span data-ttu-id="ad9c7-187">管理者権限を持つユーザーが、デバイスのロック画面で CTRL + Win + R を使用してすべてのユーザーデータと設定を削除できるようにし、デバイスを自動的に再構成して管理に再登録できるようにします。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-187">Allow users with administrative rights to delete all user data and settings using CTRL + Win + R at the device lock screen so that the device can be automatically re-configured and re-enrolled into management.</span></span>|
|<span data-ttu-id="ad9c7-188">Authenticationallowsecondarydevice</span><span class="sxs-lookup"><span data-stu-id="ad9c7-188">microsoftAccountSignInAssistantSettings</span></span>|[<span data-ttu-id="ad9c7-189">signInAssistantOptions</span><span class="sxs-lookup"><span data-stu-id="ad9c7-189">signInAssistantOptions</span></span>](../resources/intune-deviceconfig-signinassistantoptions.md)|<span data-ttu-id="ad9c7-190">Microsoft アカウントサインインアシスタント (wlidsvc) NT サービスを制御します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-190">Controls the Microsoft Account Sign-In Assistant (wlidsvc) NT service.</span></span> <span data-ttu-id="ad9c7-191">可能な値は、`notConfigured`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-191">Possible values are: `notConfigured`, `disabled`.</span></span>|
|<span data-ttu-id="ad9c7-192">authenticationAllowSecondaryDevice</span><span class="sxs-lookup"><span data-stu-id="ad9c7-192">authenticationAllowSecondaryDevice</span></span>|<span data-ttu-id="ad9c7-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-193">Boolean</span></span>|<span data-ttu-id="ad9c7-194">Windows でセカンダリ認証デバイスを使用できるようにします。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-194">Allows secondary authentication devices to work with Windows.</span></span>|
|<span data-ttu-id="ad9c7-195">authenticationWebSignIn</span><span class="sxs-lookup"><span data-stu-id="ad9c7-195">authenticationWebSignIn</span></span>|[<span data-ttu-id="ad9c7-196">購入</span><span class="sxs-lookup"><span data-stu-id="ad9c7-196">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="ad9c7-197">Web 資格情報プロバイダーを有効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-197">Indicates whether or not Web Credential Provider will be enabled.</span></span> <span data-ttu-id="ad9c7-198">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-198">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="ad9c7-199">authenticationPreferredAzureADTenantDomainName</span><span class="sxs-lookup"><span data-stu-id="ad9c7-199">authenticationPreferredAzureADTenantDomainName</span></span>|<span data-ttu-id="ad9c7-200">String</span><span class="sxs-lookup"><span data-stu-id="ad9c7-200">String</span></span>|<span data-ttu-id="ad9c7-201">Azure AD テナント内の使用可能なドメイン間で優先ドメインを指定します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-201">Specifies the preferred domain among available domains in the Azure AD tenant.</span></span>|
|<span data-ttu-id="ad9c7-202">cryptographyAllowFipsAlgorithmPolicy</span><span class="sxs-lookup"><span data-stu-id="ad9c7-202">cryptographyAllowFipsAlgorithmPolicy</span></span>|<span data-ttu-id="ad9c7-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-203">Boolean</span></span>|<span data-ttu-id="ad9c7-204">連邦情報処理規格 (FIPS) ポリシーを許可または禁止するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-204">Specify whether to allow or disallow the Federal Information Processing Standard (FIPS) policy.</span></span>|
|<span data-ttu-id="ad9c7-205">displayAppListWithGdiDPIScalingTurnedOn</span><span class="sxs-lookup"><span data-stu-id="ad9c7-205">displayAppListWithGdiDPIScalingTurnedOn</span></span>|<span data-ttu-id="ad9c7-206">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="ad9c7-206">String collection</span></span>|<span data-ttu-id="ad9c7-207">GDI DPI スケールが有効になっているレガシアプリケーションの一覧。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-207">List of legacy applications that have GDI DPI Scaling turned on.</span></span>|
|<span data-ttu-id="ad9c7-208">displayAppListWithGdiDPIScalingTurnedOff</span><span class="sxs-lookup"><span data-stu-id="ad9c7-208">displayAppListWithGdiDPIScalingTurnedOff</span></span>|<span data-ttu-id="ad9c7-209">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="ad9c7-209">String collection</span></span>|<span data-ttu-id="ad9c7-210">GDI DPI スケールがオフになっているレガシアプリケーションの一覧。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-210">List of legacy applications that have GDI DPI Scaling turned off.</span></span>|
|<span data-ttu-id="ad9c7-211">enterpriseCloudPrintDiscoveryEndPoint</span><span class="sxs-lookup"><span data-stu-id="ad9c7-211">enterpriseCloudPrintDiscoveryEndPoint</span></span>|<span data-ttu-id="ad9c7-212">String</span><span class="sxs-lookup"><span data-stu-id="ad9c7-212">String</span></span>|<span data-ttu-id="ad9c7-213">クラウド プリンターを検出するエンドポイント。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-213">Endpoint for discovering cloud printers.</span></span>|
|<span data-ttu-id="ad9c7-214">enterpriseCloudPrintOAuthAuthority</span><span class="sxs-lookup"><span data-stu-id="ad9c7-214">enterpriseCloudPrintOAuthAuthority</span></span>|<span data-ttu-id="ad9c7-215">String</span><span class="sxs-lookup"><span data-stu-id="ad9c7-215">String</span></span>|<span data-ttu-id="ad9c7-216">OAuth トークンを取得するための認証エンドポイント。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-216">Authentication endpoint for acquiring OAuth tokens.</span></span>|
|<span data-ttu-id="ad9c7-217">enterpriseCloudPrintOAuthClientIdentifier</span><span class="sxs-lookup"><span data-stu-id="ad9c7-217">enterpriseCloudPrintOAuthClientIdentifier</span></span>|<span data-ttu-id="ad9c7-218">String</span><span class="sxs-lookup"><span data-stu-id="ad9c7-218">String</span></span>|<span data-ttu-id="ad9c7-219">OAuth 認証機関から OAuth トークンを取得することを承認されているクライアント アプリケーションの GUID。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-219">GUID of a client application authorized to retrieve OAuth tokens from the OAuth Authority.</span></span>|
|<span data-ttu-id="ad9c7-220">enterpriseCloudPrintResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="ad9c7-220">enterpriseCloudPrintResourceIdentifier</span></span>|<span data-ttu-id="ad9c7-221">String</span><span class="sxs-lookup"><span data-stu-id="ad9c7-221">String</span></span>|<span data-ttu-id="ad9c7-222">Azure Portal で構成されている印刷サービスの OAuth リソース URI。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-222">OAuth resource URI for print service as configured in the Azure portal.</span></span>|
|<span data-ttu-id="ad9c7-223">enterpriseCloudPrintDiscoveryMaxLimit</span><span class="sxs-lookup"><span data-stu-id="ad9c7-223">enterpriseCloudPrintDiscoveryMaxLimit</span></span>|<span data-ttu-id="ad9c7-224">Int32</span><span class="sxs-lookup"><span data-stu-id="ad9c7-224">Int32</span></span>|<span data-ttu-id="ad9c7-225">検出エンドポイントからクエリを実行する必要があるプリンターの最大数。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-225">Maximum number of printers that should be queried from a discovery endpoint.</span></span> <span data-ttu-id="ad9c7-226">これはモバイルのみでの設定です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-226">This is a mobile only setting.</span></span> <span data-ttu-id="ad9c7-227">有効な値は 1 から 65535 までです</span><span class="sxs-lookup"><span data-stu-id="ad9c7-227">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="ad9c7-228">enterpriseCloudPrintMopriaDiscoveryResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="ad9c7-228">enterpriseCloudPrintMopriaDiscoveryResourceIdentifier</span></span>|<span data-ttu-id="ad9c7-229">String</span><span class="sxs-lookup"><span data-stu-id="ad9c7-229">String</span></span>|<span data-ttu-id="ad9c7-230">Azure Portal で構成されているプリンター検出サービスの OAuth リソース URI。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-230">OAuth resource URI for printer discovery service as configured in Azure portal.</span></span>|
|<span data-ttu-id="ad9c7-231">experienceDoNotSyncBrowserSettings</span><span class="sxs-lookup"><span data-stu-id="ad9c7-231">experienceDoNotSyncBrowserSettings</span></span>|[<span data-ttu-id="ad9c7-232">browserSyncSetting</span><span class="sxs-lookup"><span data-stu-id="ad9c7-232">browserSyncSetting</span></span>](../resources/intune-deviceconfig-browsersyncsetting.md)|<span data-ttu-id="ad9c7-233">Microsoft Edge ブラウザーの設定の同期を許可または禁止します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-233">Allow or prevent the syncing of Microsoft Edge Browser settings.</span></span> <span data-ttu-id="ad9c7-234">デバイス間の同期を禁止し、ユーザーによる上書きを許可する IT 管理者のオプション。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-234">Option for IT admins to prevent syncing across devices, but allow user override.</span></span> <span data-ttu-id="ad9c7-235">可能な値は、`notConfigured`、`blockedWithUserOverride`、`blocked` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-235">Possible values are: `notConfigured`, `blockedWithUserOverride`, `blocked`.</span></span>|
|<span data-ttu-id="ad9c7-236">messagingBlockSync</span><span class="sxs-lookup"><span data-stu-id="ad9c7-236">messagingBlockSync</span></span>|<span data-ttu-id="ad9c7-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-237">Boolean</span></span>|<span data-ttu-id="ad9c7-238">テキストメッセージのバックアップと復元、およびメッセージングのすべてをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-238">Indicates whether or not to block text message back up and restore and Messaging Everywhere.</span></span>|
|<span data-ttu-id="ad9c7-239">messagingBlockMMS</span><span class="sxs-lookup"><span data-stu-id="ad9c7-239">messagingBlockMMS</span></span>|<span data-ttu-id="ad9c7-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-240">Boolean</span></span>|<span data-ttu-id="ad9c7-241">デバイス上での MMS 送受信機能をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-241">Indicates whether or not to block the MMS send/receive functionality on the device.</span></span>|
|<span data-ttu-id="ad9c7-242">messagingBlockRichCommunicationServices</span><span class="sxs-lookup"><span data-stu-id="ad9c7-242">messagingBlockRichCommunicationServices</span></span>|<span data-ttu-id="ad9c7-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-243">Boolean</span></span>|<span data-ttu-id="ad9c7-244">デバイス上での RCS の送受信機能を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-244">Indicates whether or not to block the RCS send/receive functionality on the device.</span></span>|
|<span data-ttu-id="ad9c7-245">printerNames</span><span class="sxs-lookup"><span data-stu-id="ad9c7-245">printerNames</span></span>|<span data-ttu-id="ad9c7-246">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="ad9c7-246">String collection</span></span>|<span data-ttu-id="ad9c7-247">名前 (ネットワークホスト名) に基づいて、プリンターを自動的にプロビジョニングします。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-247">Automatically provision printers based on their names (network host names).</span></span>|
|<span data-ttu-id="ad9c7-248">プリンター Defaultname</span><span class="sxs-lookup"><span data-stu-id="ad9c7-248">printerDefaultName</span></span>|<span data-ttu-id="ad9c7-249">String</span><span class="sxs-lookup"><span data-stu-id="ad9c7-249">String</span></span>|<span data-ttu-id="ad9c7-250">インストールされているプリンターの名前 (ネットワークホスト名)。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-250">Name (network host name) of an installed printer.</span></span>|
|<span data-ttu-id="ad9c7-251">プリンターブロックの追加</span><span class="sxs-lookup"><span data-stu-id="ad9c7-251">printerBlockAddition</span></span>|<span data-ttu-id="ad9c7-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-252">Boolean</span></span>|<span data-ttu-id="ad9c7-253">ユーザーがプリンター設定から追加のプリンターをインストールできないようにします。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-253">Prevent user installation of additional printers from printers settings.</span></span>|
|<span data-ttu-id="ad9c7-254">searchBlockDiacritics</span><span class="sxs-lookup"><span data-stu-id="ad9c7-254">searchBlockDiacritics</span></span>|<span data-ttu-id="ad9c7-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-255">Boolean</span></span>|<span data-ttu-id="ad9c7-256">検索で分音記号を使用できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-256">Specifies if search can use diacritics.</span></span>|
|<span data-ttu-id="ad9c7-257">searchDisableAutoLanguageDetection</span><span class="sxs-lookup"><span data-stu-id="ad9c7-257">searchDisableAutoLanguageDetection</span></span>|<span data-ttu-id="ad9c7-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-258">Boolean</span></span>|<span data-ttu-id="ad9c7-259">コンテンツとプロパティのインデックスを作成するときに、自動言語検出を使用するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-259">Specifies whether to use automatic language detection when indexing content and properties.</span></span>|
|<span data-ttu-id="ad9c7-260">searchDisableIndexingEncryptedItems</span><span class="sxs-lookup"><span data-stu-id="ad9c7-260">searchDisableIndexingEncryptedItems</span></span>|<span data-ttu-id="ad9c7-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-261">Boolean</span></span>|<span data-ttu-id="ad9c7-262">Cortana またはエクスプローラーの検索結果に表示されないようにするため、WIP で保護されているアイテムのインデックス作成を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-262">Indicates whether or not to block indexing of WIP-protected items to prevent them from appearing in search results for Cortana or Explorer.</span></span>|
|<span data-ttu-id="ad9c7-263">searchEnableRemoteQueries</span><span class="sxs-lookup"><span data-stu-id="ad9c7-263">searchEnableRemoteQueries</span></span>|<span data-ttu-id="ad9c7-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-264">Boolean</span></span>|<span data-ttu-id="ad9c7-265">このコンピューターのインデックスに対するリモート クエリをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-265">Indicates whether or not to block remote queries of this computer’s index.</span></span>|
|<span data-ttu-id="ad9c7-266">searchDisableUseLocation</span><span class="sxs-lookup"><span data-stu-id="ad9c7-266">searchDisableUseLocation</span></span>|<span data-ttu-id="ad9c7-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-267">Boolean</span></span>|<span data-ttu-id="ad9c7-268">検索で場所情報を使用できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-268">Specifies if search can use location information.</span></span>|
|<span data-ttu-id="ad9c7-269">searchDisableLocation</span><span class="sxs-lookup"><span data-stu-id="ad9c7-269">searchDisableLocation</span></span>|<span data-ttu-id="ad9c7-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-270">Boolean</span></span>|<span data-ttu-id="ad9c7-271">検索で場所情報を使用できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-271">Specifies if search can use location information.</span></span>|
|<span data-ttu-id="ad9c7-272">searchDisableIndexerBackoff</span><span class="sxs-lookup"><span data-stu-id="ad9c7-272">searchDisableIndexerBackoff</span></span>|<span data-ttu-id="ad9c7-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-273">Boolean</span></span>|<span data-ttu-id="ad9c7-274">インデクサー バックオフの検索機能を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-274">Indicates whether or not to disable the search indexer backoff feature.</span></span>|
|<span data-ttu-id="ad9c7-275">searchDisableIndexingRemovableDrive</span><span class="sxs-lookup"><span data-stu-id="ad9c7-275">searchDisableIndexingRemovableDrive</span></span>|<span data-ttu-id="ad9c7-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-276">Boolean</span></span>|<span data-ttu-id="ad9c7-277">リムーバブル ドライブ上の場所をライブラリに追加してインデックスを作成することをユーザーに許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-277">Indicates whether or not to allow users to add locations on removable drives to libraries and to be indexed.</span></span>|
|<span data-ttu-id="ad9c7-278">searchEnableAutomaticIndexSizeManangement</span><span class="sxs-lookup"><span data-stu-id="ad9c7-278">searchEnableAutomaticIndexSizeManangement</span></span>|<span data-ttu-id="ad9c7-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-279">Boolean</span></span>|<span data-ttu-id="ad9c7-280">インデックスの場所と同じドライブ上のハード ドライブ領域の最小値を指定して、その最小値を下回ったらインデックス作成を停止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-280">Specifies minimum amount of hard drive space on the same drive as the index location before indexing stops.</span></span>|
|<span data-ttu-id="ad9c7-281">searchBlockWebResults</span><span class="sxs-lookup"><span data-stu-id="ad9c7-281">searchBlockWebResults</span></span>|<span data-ttu-id="ad9c7-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-282">Boolean</span></span>|<span data-ttu-id="ad9c7-283">Web 検索をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-283">Indicates whether or not to block the web search.</span></span>|
|<span data-ttu-id="ad9c7-284">securityBlockAzureADJoinedDevicesAutoEncryption</span><span class="sxs-lookup"><span data-stu-id="ad9c7-284">securityBlockAzureADJoinedDevicesAutoEncryption</span></span>|<span data-ttu-id="ad9c7-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-285">Boolean</span></span>|<span data-ttu-id="ad9c7-286">デバイスが Azure AD に参加しているときに、OOBE 中に自動デバイス暗号化を許可するかどうかを指定します (デスクトップのみ)。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-286">Specify whether to allow automatic device encryption during OOBE when the device is Azure AD joined (desktop only).</span></span>|
|<span data-ttu-id="ad9c7-287">diagnosticsDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="ad9c7-287">diagnosticsDataSubmissionMode</span></span>|[<span data-ttu-id="ad9c7-288">diagnosticDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="ad9c7-288">diagnosticDataSubmissionMode</span></span>](../resources/intune-deviceconfig-diagnosticdatasubmissionmode.md)|<span data-ttu-id="ad9c7-289">診断データと利用統計情報データ (Watson など) の送信をデバイスに許可する値を取得または設定します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-289">Gets or sets a value allowing the device to send diagnostic and usage telemetry data, such as Watson.</span></span> <span data-ttu-id="ad9c7-290">可能な値は、`userDefined`、`none`、`basic`、`enhanced`、`full` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-290">Possible values are: `userDefined`, `none`, `basic`, `enhanced`, `full`.</span></span>|
|<span data-ttu-id="ad9c7-291">oneDriveDisableFileSync</span><span class="sxs-lookup"><span data-stu-id="ad9c7-291">oneDriveDisableFileSync</span></span>|<span data-ttu-id="ad9c7-292">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-292">Boolean</span></span>|<span data-ttu-id="ad9c7-293">アプリや機能から OneDrive 上のファイルを操作することを IT 管理者が禁止できるかどうかを示す値を取得または設定します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-293">Gets or sets a value allowing IT admins to prevent apps and features from working with files on OneDrive.</span></span>|
|<span data-ttu-id="ad9c7-294">systemTelemetryProxyServer</span><span class="sxs-lookup"><span data-stu-id="ad9c7-294">systemTelemetryProxyServer</span></span>|<span data-ttu-id="ad9c7-295">String</span><span class="sxs-lookup"><span data-stu-id="ad9c7-295">String</span></span>|<span data-ttu-id="ad9c7-296">接続されたユーザーエクスペリエンスとテレメトリ要求を転送するためのプロキシサーバーの完全修飾ドメイン名 (FQDN) または IP アドレスを取得または設定します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-296">Gets or sets the fully qualified domain name (FQDN) or IP address of a proxy server to forward Connected User Experiences and Telemetry requests.</span></span>|
|<span data-ttu-id="ad9c7-297">edgeTelemetryForMicrosoft365Analytics</span><span class="sxs-lookup"><span data-stu-id="ad9c7-297">edgeTelemetryForMicrosoft365Analytics</span></span>|[<span data-ttu-id="ad9c7-298">edgeTelemetryMode</span><span class="sxs-lookup"><span data-stu-id="ad9c7-298">edgeTelemetryMode</span></span>](../resources/intune-deviceconfig-edgetelemetrymode.md)|<span data-ttu-id="ad9c7-299">Microsoft 365 Analytics に送信されるテレメトリデータの種類 (none、intranet、internet など) を指定します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-299">Specifies what type of telemetry data (none, intranet, internet, both) is sent to Microsoft 365 Analytics.</span></span> <span data-ttu-id="ad9c7-300">使用可能な値は、`notConfigured`、`intranet`、`internet`、`intranetAndInternet` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-300">Possible values are: `notConfigured`, `intranet`, `internet`, `intranetAndInternet`.</span></span>|
|<span data-ttu-id="ad9c7-301">inkWorkspaceAccess</span><span class="sxs-lookup"><span data-stu-id="ad9c7-301">inkWorkspaceAccess</span></span>|[<span data-ttu-id="ad9c7-302">inkAccessSetting</span><span class="sxs-lookup"><span data-stu-id="ad9c7-302">inkAccessSetting</span></span>](../resources/intune-deviceconfig-inkaccesssetting.md)|<span data-ttu-id="ad9c7-303">インクワークスペースへのユーザーアクセスをデスクトップから、またはロック画面の上から制御します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-303">Controls the user access to the ink workspace, from the desktop and from above the lock screen.</span></span> <span data-ttu-id="ad9c7-304">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-304">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="ad9c7-305">inkWorkspaceAccessState</span><span class="sxs-lookup"><span data-stu-id="ad9c7-305">inkWorkspaceAccessState</span></span>|[<span data-ttu-id="ad9c7-306">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="ad9c7-306">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="ad9c7-307">インクワークスペースへのユーザーアクセスをデスクトップから、またはロック画面の上から制御します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-307">Controls the user access to the ink workspace, from the desktop and from above the lock screen.</span></span> <span data-ttu-id="ad9c7-308">可能な値は、`notConfigured`、`blocked`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-308">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="ad9c7-309">inkWorkspaceBlockSuggestedApps</span><span class="sxs-lookup"><span data-stu-id="ad9c7-309">inkWorkspaceBlockSuggestedApps</span></span>|<span data-ttu-id="ad9c7-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-310">Boolean</span></span>|<span data-ttu-id="ad9c7-311">インクワークスペースに推奨されるアプリ候補を表示するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-311">Specify whether to show recommended app suggestions in the ink workspace.</span></span>|
|<span data-ttu-id="ad9c7-312">smartScreenEnableAppInstallControl</span><span class="sxs-lookup"><span data-stu-id="ad9c7-312">smartScreenEnableAppInstallControl</span></span>|<span data-ttu-id="ad9c7-313">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-313">Boolean</span></span>|<span data-ttu-id="ad9c7-314">このプロパティは2019年7月に廃止され、プロパティ SmartScreenAppInstallControl に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-314">This property will be deprecated in July 2019 and will be replaced by property SmartScreenAppInstallControl.</span></span> <span data-ttu-id="ad9c7-315">ユーザーがストア以外の場所からアプリをインストールできるかどうかを IT 管理者が制御することを許可します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-315">Allows IT Admins to control whether users are allowed to install apps from places other than the Store.</span></span>|
|<span data-ttu-id="ad9c7-316">smartScreenAppInstallControl</span><span class="sxs-lookup"><span data-stu-id="ad9c7-316">smartScreenAppInstallControl</span></span>|[<span data-ttu-id="ad9c7-317">appInstallControlType</span><span class="sxs-lookup"><span data-stu-id="ad9c7-317">appInstallControlType</span></span>](../resources/intune-deviceconfig-appinstallcontroltype.md)|<span data-ttu-id="ad9c7-318">Windows 10 バージョン1703で追加されました。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-318">Added in Windows 10, version 1703.</span></span> <span data-ttu-id="ad9c7-319">ユーザーがストア以外の場所からアプリをインストールできるかどうかを IT 管理者が制御することを許可します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-319">Allows IT Admins to control whether users are allowed to install apps from places other than the Store.</span></span> <span data-ttu-id="ad9c7-320">可能な値は、`notConfigured`、`anywhere`、`storeOnly`、`recommendations`、`preferStore` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-320">Possible values are: `notConfigured`, `anywhere`, `storeOnly`, `recommendations`, `preferStore`.</span></span>|
|<span data-ttu-id="ad9c7-321">personalizationDesktopImageUrl</span><span class="sxs-lookup"><span data-stu-id="ad9c7-321">personalizationDesktopImageUrl</span></span>|<span data-ttu-id="ad9c7-322">String</span><span class="sxs-lookup"><span data-stu-id="ad9c7-322">String</span></span>|<span data-ttu-id="ad9c7-323">ダウンロードしてデスクトップ画像として使用する必要がある jpg、jpeg、png 画像の http または https URL、あるいはデスクトップ画像として使用する必要があるファイル システム上のローカル画像のファイル URL。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-323">A http or https Url to a jpg, jpeg or png image that needs to be downloaded and used as the Desktop Image or a file Url to a local image on the file system that needs to used as the Desktop Image.</span></span>|
|<span data-ttu-id="ad9c7-324">personalizationLockScreenImageUrl</span><span class="sxs-lookup"><span data-stu-id="ad9c7-324">personalizationLockScreenImageUrl</span></span>|<span data-ttu-id="ad9c7-325">String</span><span class="sxs-lookup"><span data-stu-id="ad9c7-325">String</span></span>|<span data-ttu-id="ad9c7-326">ダウンロードしてロック画面画像として使用する必要がある jpg、jpeg、png 画像の http または https URL、あるいはロック画面画像として使用する必要があるファイル システム上のローカル画像のファイル URL。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-326">A http or https Url to a jpg, jpeg or png image that neeeds to be downloaded and used as the Lock Screen Image or a file Url to a local image on the file system that needs to be used as the Lock Screen Image.</span></span>|
|<span data-ttu-id="ad9c7-327">bluetoothAllowedServices</span><span class="sxs-lookup"><span data-stu-id="ad9c7-327">bluetoothAllowedServices</span></span>|<span data-ttu-id="ad9c7-328">String コレクション</span><span class="sxs-lookup"><span data-stu-id="ad9c7-328">String collection</span></span>|<span data-ttu-id="ad9c7-329">許可されている Bluetooth サービスおよびプロファイルの一覧を 16 進形式の文字列として指定します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-329">Specify a list of allowed Bluetooth services and profiles in hex formatted strings.</span></span>|
|<span data-ttu-id="ad9c7-330">bluetoothBlockAdvertising</span><span class="sxs-lookup"><span data-stu-id="ad9c7-330">bluetoothBlockAdvertising</span></span>|<span data-ttu-id="ad9c7-331">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-331">Boolean</span></span>|<span data-ttu-id="ad9c7-332">ユーザーが Bluetooth 広告を使用することを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-332">Whether or not to Block the user from using bluetooth advertising.</span></span>|
|<span data-ttu-id="ad9c7-333">bluetoothBlockPromptedProximalConnections</span><span class="sxs-lookup"><span data-stu-id="ad9c7-333">bluetoothBlockPromptedProximalConnections</span></span>|<span data-ttu-id="ad9c7-334">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-334">Boolean</span></span>|<span data-ttu-id="ad9c7-335">ユーザーが Swift ペアや他の近接ベースのシナリオを使用することを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-335">Whether or not to block the users from using Swift Pair and other proximity based scenarios.</span></span>|
|<span data-ttu-id="ad9c7-336">bluetoothBlockDiscoverableMode</span><span class="sxs-lookup"><span data-stu-id="ad9c7-336">bluetoothBlockDiscoverableMode</span></span>|<span data-ttu-id="ad9c7-337">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-337">Boolean</span></span>|<span data-ttu-id="ad9c7-338">ユーザーが Bluetooth の発見可能モードを使用することを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-338">Whether or not to Block the user from using bluetooth discoverable mode.</span></span>|
|<span data-ttu-id="ad9c7-339">bluetoothBlockPrePairing</span><span class="sxs-lookup"><span data-stu-id="ad9c7-339">bluetoothBlockPrePairing</span></span>|<span data-ttu-id="ad9c7-340">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-340">Boolean</span></span>|<span data-ttu-id="ad9c7-341">バンドルされた特定のいくつかの Bluetooth 周辺機器を自動的にホスト デバイスとペアにすることを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-341">Whether or not to block specific bundled Bluetooth peripherals to automatically pair with the host device.</span></span>|
|<span data-ttu-id="ad9c7-342">edgeBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="ad9c7-342">edgeBlockAutofill</span></span>|<span data-ttu-id="ad9c7-343">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-343">Boolean</span></span>|<span data-ttu-id="ad9c7-344">自動入力を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-344">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="ad9c7-345">edgeBlocked</span><span class="sxs-lookup"><span data-stu-id="ad9c7-345">edgeBlocked</span></span>|<span data-ttu-id="ad9c7-346">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-346">Boolean</span></span>|<span data-ttu-id="ad9c7-347">ユーザーが Edge ブラウザーを使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-347">Indicates whether or not to Block the user from using the Edge browser.</span></span>|
|<span data-ttu-id="ad9c7-348">edgeCookiePolicy</span><span class="sxs-lookup"><span data-stu-id="ad9c7-348">edgeCookiePolicy</span></span>|[<span data-ttu-id="ad9c7-349">edgeCookiePolicy</span><span class="sxs-lookup"><span data-stu-id="ad9c7-349">edgeCookiePolicy</span></span>](../resources/intune-deviceconfig-edgecookiepolicy.md)|<span data-ttu-id="ad9c7-350">Edge ブラウザーでどの Cookie を禁止するかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-350">Indicates which cookies to block in the Edge browser.</span></span> <span data-ttu-id="ad9c7-351">可能な値は、`userDefined`、`allow`、`blockThirdParty`、`blockAll` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-351">Possible values are: `userDefined`, `allow`, `blockThirdParty`, `blockAll`.</span></span>|
|<span data-ttu-id="ad9c7-352">edgeBlockDeveloperTools</span><span class="sxs-lookup"><span data-stu-id="ad9c7-352">edgeBlockDeveloperTools</span></span>|<span data-ttu-id="ad9c7-353">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-353">Boolean</span></span>|<span data-ttu-id="ad9c7-354">Edge ブラウザー内の開発者ツールを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-354">Indicates whether or not to block developer tools in the Edge browser.</span></span>|
|<span data-ttu-id="ad9c7-355">edgeBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="ad9c7-355">edgeBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="ad9c7-356">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-356">Boolean</span></span>|<span data-ttu-id="ad9c7-357">ユーザーがトラッキング拒否ヘッダーを送信することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-357">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="ad9c7-358">edgeBlockExtensions</span><span class="sxs-lookup"><span data-stu-id="ad9c7-358">edgeBlockExtensions</span></span>|<span data-ttu-id="ad9c7-359">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-359">Boolean</span></span>|<span data-ttu-id="ad9c7-360">Edge ブラウザーの拡張機能を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-360">Indicates whether or not to block extensions in the Edge browser.</span></span>|
|<span data-ttu-id="ad9c7-361">edgeBlockInPrivateBrowsing</span><span class="sxs-lookup"><span data-stu-id="ad9c7-361">edgeBlockInPrivateBrowsing</span></span>|<span data-ttu-id="ad9c7-362">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-362">Boolean</span></span>|<span data-ttu-id="ad9c7-363">Edge ブラウザーで会社のネットワークの InPrivate ブラウズを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-363">Indicates whether or not to block InPrivate browsing on corporate networks, in the Edge browser.</span></span>|
|<span data-ttu-id="ad9c7-364">edgeBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="ad9c7-364">edgeBlockJavaScript</span></span>|<span data-ttu-id="ad9c7-365">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-365">Boolean</span></span>|<span data-ttu-id="ad9c7-366">ユーザーが JavaScript を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-366">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="ad9c7-367">edgeBlockPasswordManager</span><span class="sxs-lookup"><span data-stu-id="ad9c7-367">edgeBlockPasswordManager</span></span>|<span data-ttu-id="ad9c7-368">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-368">Boolean</span></span>|<span data-ttu-id="ad9c7-369">パスワード マネージャーを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-369">Indicates whether or not to Block password manager.</span></span>|
|<span data-ttu-id="ad9c7-370">edgeBlockAddressBarDropdown</span><span class="sxs-lookup"><span data-stu-id="ad9c7-370">edgeBlockAddressBarDropdown</span></span>|<span data-ttu-id="ad9c7-371">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-371">Boolean</span></span>|<span data-ttu-id="ad9c7-372">Microsoft Edge のアドレス バー ドロップダウン機能を禁止します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-372">Block the address bar dropdown functionality in Microsoft Edge.</span></span> <span data-ttu-id="ad9c7-373">Microsoft Edge から Microsoft サービスへのネットワーク接続を最小限に抑えるには、この設定を無効にします。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-373">Disable this settings to minimize network connections from Microsoft Edge to Microsoft services.</span></span>|
|<span data-ttu-id="ad9c7-374">edgeBlockCompatibilityList</span><span class="sxs-lookup"><span data-stu-id="ad9c7-374">edgeBlockCompatibilityList</span></span>|<span data-ttu-id="ad9c7-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-375">Boolean</span></span>|<span data-ttu-id="ad9c7-376">Microsoft Edge での Microsoft 互換性リストを禁止します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-376">Block Microsoft compatibility list in Microsoft Edge.</span></span> <span data-ttu-id="ad9c7-377">Microsoft ではこのリストを利用して、既知の互換性の問題があるサイトを Edge で正しく表示できるようにします。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-377">This list from Microsoft helps Edge properly display sites with known compatibility issues.</span></span>|
|<span data-ttu-id="ad9c7-378">edgeClearBrowsingDataOnExit</span><span class="sxs-lookup"><span data-stu-id="ad9c7-378">edgeClearBrowsingDataOnExit</span></span>|<span data-ttu-id="ad9c7-379">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-379">Boolean</span></span>|<span data-ttu-id="ad9c7-380">Microsoft Edge の終了時にブラウズ データを消去します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-380">Clear browsing data on exiting Microsoft Edge.</span></span>|
|<span data-ttu-id="ad9c7-381">edgeAllowStartPagesModification</span><span class="sxs-lookup"><span data-stu-id="ad9c7-381">edgeAllowStartPagesModification</span></span>|<span data-ttu-id="ad9c7-382">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-382">Boolean</span></span>|<span data-ttu-id="ad9c7-383">Edge のスタート ページをユーザーが変更することを許可します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-383">Allow users to change Start pages on Edge.</span></span> <span data-ttu-id="ad9c7-384">ユーザーが Edge を開いたときに既定で表示されるスタート ページを指定するには、EdgeHomepageUrls を使用します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-384">Use the EdgeHomepageUrls to specify the Start pages that the user would see by default when they open Edge.</span></span>|
|<span data-ttu-id="ad9c7-385">edgeDisableFirstRunPage</span><span class="sxs-lookup"><span data-stu-id="ad9c7-385">edgeDisableFirstRunPage</span></span>|<span data-ttu-id="ad9c7-386">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-386">Boolean</span></span>|<span data-ttu-id="ad9c7-387">Microsoft Edge の初回使用時に表示される Microsoft の Web ページを禁止します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-387">Block the Microsoft web page that opens on the first use of Microsoft Edge.</span></span> <span data-ttu-id="ad9c7-388">このポリシーでは、ゼロ エミッション構成に登録している企業などが、このページの表示を禁止できます。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-388">This policy allows enterprises, like those enrolled in zero emissions configurations, to block this page.</span></span>|
|<span data-ttu-id="ad9c7-389">edgeBlockLiveTileDataCollection</span><span class="sxs-lookup"><span data-stu-id="ad9c7-389">edgeBlockLiveTileDataCollection</span></span>|<span data-ttu-id="ad9c7-390">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-390">Boolean</span></span>|<span data-ttu-id="ad9c7-391">ユーザーが Microsoft Edge からスタートにサイトをピン留めしたときに、ライブ タイルを作成するために Microsoft が情報を収集することを禁止します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-391">Block the collection of information by Microsoft for live tile creation when users pin a site to Start from Microsoft Edge.</span></span>|
|<span data-ttu-id="ad9c7-392">edgeSyncFavoritesWithInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="ad9c7-392">edgeSyncFavoritesWithInternetExplorer</span></span>|<span data-ttu-id="ad9c7-393">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-393">Boolean</span></span>|<span data-ttu-id="ad9c7-394">Internet Explorer と Microsoft Edge の間でお気に入りの同期を有効にします。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-394">Enable favorites sync between Internet Explorer and Microsoft Edge.</span></span> <span data-ttu-id="ad9c7-395">お気に入りの追加、削除、変更、順序変更が、ブラウザー間で共有されます。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-395">Additions, deletions, modifications and order changes to favorites are shared between browsers.</span></span>|
|<span data-ttu-id="ad9c7-396">edgeFavoritesListLocation</span><span class="sxs-lookup"><span data-stu-id="ad9c7-396">edgeFavoritesListLocation</span></span>|<span data-ttu-id="ad9c7-397">String</span><span class="sxs-lookup"><span data-stu-id="ad9c7-397">String</span></span>|<span data-ttu-id="ad9c7-398">準備するお気に入りの一覧の場所です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-398">The location of the favorites list to provision.</span></span> <span data-ttu-id="ad9c7-399">ローカル ファイル、ローカル ネットワーク、http の場所が該当します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-399">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="ad9c7-400">edgeBlockEditFavorites</span><span class="sxs-lookup"><span data-stu-id="ad9c7-400">edgeBlockEditFavorites</span></span>|<span data-ttu-id="ad9c7-401">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-401">Boolean</span></span>|<span data-ttu-id="ad9c7-402">ユーザーがお気に入りを変更することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-402">Indicates whether or not to Block the user from making changes to Favorites.</span></span>|
|<span data-ttu-id="ad9c7-403">edgeNewTabPageURL</span><span class="sxs-lookup"><span data-stu-id="ad9c7-403">edgeNewTabPageURL</span></span>|<span data-ttu-id="ad9c7-404">String</span><span class="sxs-lookup"><span data-stu-id="ad9c7-404">String</span></span>|<span data-ttu-id="ad9c7-405">新しいタブが作成されたときに開かれるページを指定します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-405">Specify the page opened when new tabs are created.</span></span>|
|<span data-ttu-id="ad9c7-406">edgeHomeButtonConfiguration</span><span class="sxs-lookup"><span data-stu-id="ad9c7-406">edgeHomeButtonConfiguration</span></span>|[<span data-ttu-id="ad9c7-407">edgeHomeButtonConfiguration</span><span class="sxs-lookup"><span data-stu-id="ad9c7-407">edgeHomeButtonConfiguration</span></span>](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)|<span data-ttu-id="ad9c7-408">[ホーム] ボタンを非表示にし、既定の開始ページを読み込むか、新しいタブページを読み込むか、またはカスタム URL を読み込みます。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-408">Causes the Home button to either hide, load the default Start page, load a New tab page, or a custom URL</span></span>|
|<span data-ttu-id="ad9c7-409">edgeHomeButtonConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="ad9c7-409">edgeHomeButtonConfigurationEnabled</span></span>|<span data-ttu-id="ad9c7-410">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-410">Boolean</span></span>|<span data-ttu-id="ad9c7-411">ホームボタンの構成を有効にします。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-411">Enable the Home button configuration.</span></span>|
|<span data-ttu-id="ad9c7-412">edgeOpensWith</span><span class="sxs-lookup"><span data-stu-id="ad9c7-412">edgeOpensWith</span></span>|[<span data-ttu-id="ad9c7-413">edgeOpenOptions</span><span class="sxs-lookup"><span data-stu-id="ad9c7-413">edgeOpenOptions</span></span>](../resources/intune-deviceconfig-edgeopenoptions.md)|<span data-ttu-id="ad9c7-414">開始時に開くページの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-414">Specify what kind of pages are open at start.</span></span> <span data-ttu-id="ad9c7-415">可能な値は、`notConfigured`、`startPage`、`newTabPage`、`previousPages`、`specificPages` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-415">Possible values are: `notConfigured`, `startPage`, `newTabPage`, `previousPages`, `specificPages`.</span></span>|
|<span data-ttu-id="ad9c7-416">edgeBlockSideloadingExtensions</span><span class="sxs-lookup"><span data-stu-id="ad9c7-416">edgeBlockSideloadingExtensions</span></span>|<span data-ttu-id="ad9c7-417">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-417">Boolean</span></span>|<span data-ttu-id="ad9c7-418">ユーザーが拡張機能をサイドロードできるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-418">Indicates whether the user can sideload extensions.</span></span>|
|<span data-ttu-id="ad9c7-419">edgeRequiredExtensionPackageFamilyNames</span><span class="sxs-lookup"><span data-stu-id="ad9c7-419">edgeRequiredExtensionPackageFamilyNames</span></span>|<span data-ttu-id="ad9c7-420">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="ad9c7-420">String collection</span></span>|<span data-ttu-id="ad9c7-421">必要なブラウザー拡張機能のパッケージファミリ名のリストを指定します。ユーザーが無効にすることはできません。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-421">Specify the list of package family names of browser extensions that are required and cannot be turned off by the user.</span></span>|
|<span data-ttu-id="ad9c7-422">edgeBlockPrinting</span><span class="sxs-lookup"><span data-stu-id="ad9c7-422">edgeBlockPrinting</span></span>|<span data-ttu-id="ad9c7-423">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-423">Boolean</span></span>|<span data-ttu-id="ad9c7-424">印刷を許可またはブロックするようにエッジを構成します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-424">Configure Edge to allow or block printing.</span></span>|
|<span data-ttu-id="ad9c7-425">edgeFavoritesBarVisibility</span><span class="sxs-lookup"><span data-stu-id="ad9c7-425">edgeFavoritesBarVisibility</span></span>|[<span data-ttu-id="ad9c7-426">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="ad9c7-426">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="ad9c7-427">[お気に入り] バーを常に表示または非表示に設定するかどうかを指定する値を取得または設定します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-427">Get or set a value that specifies whether to set the favorites bar to always be visible or hidden on any page.</span></span> <span data-ttu-id="ad9c7-428">可能な値は、`notConfigured`、`hide`、`show` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-428">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="ad9c7-429">edgeBlockSavingHistory</span><span class="sxs-lookup"><span data-stu-id="ad9c7-429">edgeBlockSavingHistory</span></span>|<span data-ttu-id="ad9c7-430">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-430">Boolean</span></span>|<span data-ttu-id="ad9c7-431">閲覧履歴を保存できるようにエッジを構成するか、閲覧履歴を保存しないようにします。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-431">Configure Edge to allow browsing history to be saved or to never save browsing history.</span></span>|
|<span data-ttu-id="ad9c7-432">edgeBlockFullScreenMode</span><span class="sxs-lookup"><span data-stu-id="ad9c7-432">edgeBlockFullScreenMode</span></span>|<span data-ttu-id="ad9c7-433">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-433">Boolean</span></span>|<span data-ttu-id="ad9c7-434">エッジが全画面表示モードに入るのを許可または禁止します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-434">Allow or prevent Edge from entering the full screen mode.</span></span>|
|<span data-ttu-id="ad9c7-435">edgeBlockWebContentOnNewTabPage</span><span class="sxs-lookup"><span data-stu-id="ad9c7-435">edgeBlockWebContentOnNewTabPage</span></span>|<span data-ttu-id="ad9c7-436">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-436">Boolean</span></span>|<span data-ttu-id="ad9c7-437">既定の新しいタブページの代わりに、エッジに空白ページを読み込むように構成し、ユーザーがそれを変更できないようにします。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-437">Configure to load a blank page in Edge instead of the default New tab page and prevent users from changing it.</span></span>|
|<span data-ttu-id="ad9c7-438">edgeBlockTabPreloading</span><span class="sxs-lookup"><span data-stu-id="ad9c7-438">edgeBlockTabPreloading</span></span>|<span data-ttu-id="ad9c7-439">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-439">Boolean</span></span>|<span data-ttu-id="ad9c7-440">Windows 起動時にエッジが新しいタブページをプリロードするかどうかを構成します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-440">Configure whether Edge preloads the new tab page at Windows startup.</span></span>|
|<span data-ttu-id="ad9c7-441">edgeBlockPrelaunch</span><span class="sxs-lookup"><span data-stu-id="ad9c7-441">edgeBlockPrelaunch</span></span>|<span data-ttu-id="ad9c7-442">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-442">Boolean</span></span>|<span data-ttu-id="ad9c7-443">Microsoft Edge を Windows 起動時に事前に起動するかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-443">Decide whether Microsoft Edge is prelaunched at Windows startup.</span></span>|
|<span data-ttu-id="ad9c7-444">edgeShowMessageWhenOpeningInternetExplorerSites</span><span class="sxs-lookup"><span data-stu-id="ad9c7-444">edgeShowMessageWhenOpeningInternetExplorerSites</span></span>|[<span data-ttu-id="ad9c7-445">internetExplorerMessageSetting</span><span class="sxs-lookup"><span data-stu-id="ad9c7-445">internetExplorerMessageSetting</span></span>](../resources/intune-deviceconfig-internetexplorermessagesetting.md)|<span data-ttu-id="ad9c7-446">Internet Explorer に切り替える前に、エッジによって表示されるメッセージを制御します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-446">Controls the message displayed by Edge before switching to Internet Explorer.</span></span> <span data-ttu-id="ad9c7-447">使用可能な値は、`notConfigured`、`disabled`、`enabled`、`keepGoing` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-447">Possible values are: `notConfigured`, `disabled`, `enabled`, `keepGoing`.</span></span>|
|<span data-ttu-id="ad9c7-448">edgePreventCertificateErrorOverride</span><span class="sxs-lookup"><span data-stu-id="ad9c7-448">edgePreventCertificateErrorOverride</span></span>|<span data-ttu-id="ad9c7-449">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-449">Boolean</span></span>|<span data-ttu-id="ad9c7-450">ユーザーが証明書のエラーを上書きすることを許可または禁止します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-450">Allow or prevent users from overriding certificate errors.</span></span>|
|<span data-ttu-id="ad9c7-451">edgeKioskModeRestriction</span><span class="sxs-lookup"><span data-stu-id="ad9c7-451">edgeKioskModeRestriction</span></span>|[<span data-ttu-id="ad9c7-452">edgeKioskModeRestrictionType</span><span class="sxs-lookup"><span data-stu-id="ad9c7-452">edgeKioskModeRestrictionType</span></span>](../resources/intune-deviceconfig-edgekioskmoderestrictiontype.md)|<span data-ttu-id="ad9c7-453">[キオスクの構成] モードに基づいて、Microsoft Edge の設定が制限される方法を制御します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-453">Controls how the Microsoft Edge settings are restricted based on the configure kiosk mode.</span></span> <span data-ttu-id="ad9c7-454">可能な値は、`notConfigured`、`digitalSignage`、`normalMode`、`publicBrowsingSingleApp`、`publicBrowsingMultiApp` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-454">Possible values are: `notConfigured`, `digitalSignage`, `normalMode`, `publicBrowsingSingleApp`, `publicBrowsingMultiApp`.</span></span>|
|<span data-ttu-id="ad9c7-455">edgeKioskResetAfterIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="ad9c7-455">edgeKioskResetAfterIdleTimeInMinutes</span></span>|<span data-ttu-id="ad9c7-456">Int32</span><span class="sxs-lookup"><span data-stu-id="ad9c7-456">Int32</span></span>|<span data-ttu-id="ad9c7-457">前回のユーザーアクティビティから、Microsoft Edge キオスクがリセットされるまでの時間を分単位で指定します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-457">Specifies the time in minutes from the last user activity before Microsoft Edge kiosk resets.</span></span>  <span data-ttu-id="ad9c7-458">有効な値は0-1440 です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-458">Valid values are 0-1440.</span></span> <span data-ttu-id="ad9c7-459">既定は 5 です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-459">The default is 5.</span></span> <span data-ttu-id="ad9c7-460">0はリセットしないことを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-460">0 indicates no reset.</span></span> <span data-ttu-id="ad9c7-461">有効な値は 0 ~ 1440</span><span class="sxs-lookup"><span data-stu-id="ad9c7-461">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="ad9c7-462">cellularBlockDataWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="ad9c7-462">cellularBlockDataWhenRoaming</span></span>|<span data-ttu-id="ad9c7-463">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-463">Boolean</span></span>|<span data-ttu-id="ad9c7-464">ローミング中に携帯電話上でユーザーがデータを使用することを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-464">Whether or not to Block the user from using data over cellular while roaming.</span></span>|
|<span data-ttu-id="ad9c7-465">cellularBlockVpn</span><span class="sxs-lookup"><span data-stu-id="ad9c7-465">cellularBlockVpn</span></span>|<span data-ttu-id="ad9c7-466">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-466">Boolean</span></span>|<span data-ttu-id="ad9c7-467">携帯電話上でユーザーが VPN を使用することを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-467">Whether or not to Block the user from using VPN over cellular.</span></span>|
|<span data-ttu-id="ad9c7-468">cellularBlockVpnWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="ad9c7-468">cellularBlockVpnWhenRoaming</span></span>|<span data-ttu-id="ad9c7-469">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-469">Boolean</span></span>|<span data-ttu-id="ad9c7-470">ローミング時に携帯電話上でユーザーが VPN を使用することを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-470">Whether or not to Block the user from using VPN when roaming over cellular.</span></span>|
|<span data-ttu-id="ad9c7-471">cellularData</span><span class="sxs-lookup"><span data-stu-id="ad9c7-471">cellularData</span></span>|[<span data-ttu-id="ad9c7-472">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="ad9c7-472">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="ad9c7-473">デバイス上の携帯データチャネルを許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-473">Whether or not to allow the cellular data channel on the device.</span></span> <span data-ttu-id="ad9c7-474">構成されていない場合は、携帯データチャネルが許可され、ユーザーはこれをオフにすることができます。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-474">If not configured, the cellular data channel is allowed and the user can turn it off.</span></span> <span data-ttu-id="ad9c7-475">可能な値は、`blocked`、`required`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-475">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="ad9c7-476">defenderBlockEndUserAccess</span><span class="sxs-lookup"><span data-stu-id="ad9c7-476">defenderBlockEndUserAccess</span></span>|<span data-ttu-id="ad9c7-477">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-477">Boolean</span></span>|<span data-ttu-id="ad9c7-478">エンド ユーザーが Defender にアクセスすることを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-478">Whether or not to block end user access to Defender.</span></span>|
|<span data-ttu-id="ad9c7-479">defenderDaysBeforeDeletingQuarantinedMalware</span><span class="sxs-lookup"><span data-stu-id="ad9c7-479">defenderDaysBeforeDeletingQuarantinedMalware</span></span>|<span data-ttu-id="ad9c7-480">Int32</span><span class="sxs-lookup"><span data-stu-id="ad9c7-480">Int32</span></span>|<span data-ttu-id="ad9c7-481">検疫済みのマルウェアを削除するまでの日数。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-481">Number of days before deleting quarantined malware.</span></span> <span data-ttu-id="ad9c7-482">有効な値は 0 から 90 までです</span><span class="sxs-lookup"><span data-stu-id="ad9c7-482">Valid values 0 to 90</span></span>|
|<span data-ttu-id="ad9c7-483">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="ad9c7-483">defenderDetectedMalwareActions</span></span>|[<span data-ttu-id="ad9c7-484">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="ad9c7-484">defenderDetectedMalwareActions</span></span>](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|<span data-ttu-id="ad9c7-485">検出されたマルウェアに対する Defender のアクションを脅威レベルごとに取得または設定します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-485">Gets or sets Defender’s actions to take on detected Malware per threat level.</span></span>|
|<span data-ttu-id="ad9c7-486">defenderSystemScanSchedule</span><span class="sxs-lookup"><span data-stu-id="ad9c7-486">defenderSystemScanSchedule</span></span>|[<span data-ttu-id="ad9c7-487">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="ad9c7-487">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="ad9c7-488">Defender がシステムをスキャンする曜日。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-488">Defender day of the week for the system scan.</span></span> <span data-ttu-id="ad9c7-489">可能な値は、`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-489">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="ad9c7-490">defenderFilesAndFoldersToExclude</span><span class="sxs-lookup"><span data-stu-id="ad9c7-490">defenderFilesAndFoldersToExclude</span></span>|<span data-ttu-id="ad9c7-491">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="ad9c7-491">String collection</span></span>|<span data-ttu-id="ad9c7-492">スキャンとリアルタイム保護から除外するファイルとフォルダー。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-492">Files and folder to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="ad9c7-493">defenderFileExtensionsToExclude</span><span class="sxs-lookup"><span data-stu-id="ad9c7-493">defenderFileExtensionsToExclude</span></span>|<span data-ttu-id="ad9c7-494">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="ad9c7-494">String collection</span></span>|<span data-ttu-id="ad9c7-495">スキャンとリアルタイム保護から除外するファイル拡張子。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-495">File extensions to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="ad9c7-496">defenderScanMaxCpu</span><span class="sxs-lookup"><span data-stu-id="ad9c7-496">defenderScanMaxCpu</span></span>|<span data-ttu-id="ad9c7-497">Int32</span><span class="sxs-lookup"><span data-stu-id="ad9c7-497">Int32</span></span>|<span data-ttu-id="ad9c7-498">スキャン中の最大 CPU 使用率。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-498">Max CPU usage percentage during scan.</span></span> <span data-ttu-id="ad9c7-499">有効な値は 0 から 100 までです</span><span class="sxs-lookup"><span data-stu-id="ad9c7-499">Valid values 0 to 100</span></span>|
|<span data-ttu-id="ad9c7-500">defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="ad9c7-500">defenderMonitorFileActivity</span></span>|[<span data-ttu-id="ad9c7-501">defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="ad9c7-501">defenderMonitorFileActivity</span></span>](../resources/intune-deviceconfig-defendermonitorfileactivity.md)|<span data-ttu-id="ad9c7-502">ファイル アクティビティを監視する値。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-502">Value for monitoring file activity.</span></span> <span data-ttu-id="ad9c7-503">可能な値は、`userDefined`、`disable`、`monitorAllFiles`、`monitorIncomingFilesOnly`、`monitorOutgoingFilesOnly` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-503">Possible values are: `userDefined`, `disable`, `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.</span></span>|
|<span data-ttu-id="ad9c7-504">defenderPotentiallyUnwantedAppAction</span><span class="sxs-lookup"><span data-stu-id="ad9c7-504">defenderPotentiallyUnwantedAppAction</span></span>|[<span data-ttu-id="ad9c7-505">defenderPotentiallyUnwantedAppAction</span><span class="sxs-lookup"><span data-stu-id="ad9c7-505">defenderPotentiallyUnwantedAppAction</span></span>](../resources/intune-deviceconfig-defenderpotentiallyunwantedappaction.md)|<span data-ttu-id="ad9c7-506">望ましくない可能性があるアプリケーション (PUA) に対して実行する Defender のアクションを取得または設定します。これには、ad インジェクション、ソフトウェアバンドル、支払いまたはサブスクリプションのための永続的な勧誘などの動作を備えたソフトウェアが含まれます。PUA がダウンロードされているとき、またはインストールしようとしているときに、Defender でユーザーに通知します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-506">Gets or sets Defender’s action to take on Potentially Unwanted Application (PUA), which includes software with behaviors of ad-injection, software bundling, persistent solicitation for payment or subscription, etc. Defender alerts user when PUA is being downloaded or attempts to install itself.</span></span> <span data-ttu-id="ad9c7-507">Windows 10 でデスクトップ用に追加されました。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-507">Added in Windows 10 for desktop.</span></span> <span data-ttu-id="ad9c7-508">可能な値は、`deviceDefault`、`block`、`audit` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-508">Possible values are: `deviceDefault`, `block`, `audit`.</span></span>|
|<span data-ttu-id="ad9c7-509">defenderPotentiallyUnwantedAppActionSetting</span><span class="sxs-lookup"><span data-stu-id="ad9c7-509">defenderPotentiallyUnwantedAppActionSetting</span></span>|[<span data-ttu-id="ad9c7-510">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="ad9c7-510">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="ad9c7-511">望ましくない可能性があるアプリケーション (PUA) に対して実行する Defender のアクションを取得または設定します。これには、ad インジェクション、ソフトウェアバンドル、支払いまたはサブスクリプションのための永続的な勧誘などの動作を備えたソフトウェアが含まれます。PUA がダウンロードされているとき、またはインストールしようとしているときに、Defender でユーザーに通知します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-511">Gets or sets Defender’s action to take on Potentially Unwanted Application (PUA), which includes software with behaviors of ad-injection, software bundling, persistent solicitation for payment or subscription, etc. Defender alerts user when PUA is being downloaded or attempts to install itself.</span></span> <span data-ttu-id="ad9c7-512">Windows 10 でデスクトップ用に追加されました。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-512">Added in Windows 10 for desktop.</span></span> <span data-ttu-id="ad9c7-513">可能な値は、`userDefined`、`enable`、`auditMode` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-513">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="ad9c7-514">defenderProcessesToExclude</span><span class="sxs-lookup"><span data-stu-id="ad9c7-514">defenderProcessesToExclude</span></span>|<span data-ttu-id="ad9c7-515">String コレクション</span><span class="sxs-lookup"><span data-stu-id="ad9c7-515">String collection</span></span>|<span data-ttu-id="ad9c7-516">スキャンとリアルタイム保護から除外するプロセス。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-516">Processes to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="ad9c7-517">defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="ad9c7-517">defenderPromptForSampleSubmission</span></span>|[<span data-ttu-id="ad9c7-518">defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="ad9c7-518">defenderPromptForSampleSubmission</span></span>](../resources/intune-deviceconfig-defenderpromptforsamplesubmission.md)|<span data-ttu-id="ad9c7-519">ユーザーにサンプルの送信を要求する方法の構成。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-519">The configuration for how to prompt user for sample submission.</span></span> <span data-ttu-id="ad9c7-520">可能な値は、`userDefined`、`alwaysPrompt`、`promptBeforeSendingPersonalData`、`neverSendData`、`sendAllDataWithoutPrompting` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-520">Possible values are: `userDefined`, `alwaysPrompt`, `promptBeforeSendingPersonalData`, `neverSendData`, `sendAllDataWithoutPrompting`.</span></span>|
|<span data-ttu-id="ad9c7-521">defenderRequireBehaviorMonitoring</span><span class="sxs-lookup"><span data-stu-id="ad9c7-521">defenderRequireBehaviorMonitoring</span></span>|<span data-ttu-id="ad9c7-522">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-522">Boolean</span></span>|<span data-ttu-id="ad9c7-523">動作の監視が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-523">Indicates whether or not to require behavior monitoring.</span></span>|
|<span data-ttu-id="ad9c7-524">defenderRequireCloudProtection</span><span class="sxs-lookup"><span data-stu-id="ad9c7-524">defenderRequireCloudProtection</span></span>|<span data-ttu-id="ad9c7-525">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-525">Boolean</span></span>|<span data-ttu-id="ad9c7-526">クラウドの保護が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-526">Indicates whether or not to require cloud protection.</span></span>|
|<span data-ttu-id="ad9c7-527">defenderRequireNetworkInspectionSystem</span><span class="sxs-lookup"><span data-stu-id="ad9c7-527">defenderRequireNetworkInspectionSystem</span></span>|<span data-ttu-id="ad9c7-528">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-528">Boolean</span></span>|<span data-ttu-id="ad9c7-529">ネットワーク検査システムが必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-529">Indicates whether or not to require network inspection system.</span></span>|
|<span data-ttu-id="ad9c7-530">defenderRequireRealTimeMonitoring</span><span class="sxs-lookup"><span data-stu-id="ad9c7-530">defenderRequireRealTimeMonitoring</span></span>|<span data-ttu-id="ad9c7-531">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-531">Boolean</span></span>|<span data-ttu-id="ad9c7-532">リアルタイムの監視が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-532">Indicates whether or not to require real time monitoring.</span></span>|
|<span data-ttu-id="ad9c7-533">defenderScanArchiveFiles</span><span class="sxs-lookup"><span data-stu-id="ad9c7-533">defenderScanArchiveFiles</span></span>|<span data-ttu-id="ad9c7-534">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-534">Boolean</span></span>|<span data-ttu-id="ad9c7-535">アーカイブ ファイルをスキャンするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-535">Indicates whether or not to scan archive files.</span></span>|
|<span data-ttu-id="ad9c7-536">defenderScanDownloads</span><span class="sxs-lookup"><span data-stu-id="ad9c7-536">defenderScanDownloads</span></span>|<span data-ttu-id="ad9c7-537">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-537">Boolean</span></span>|<span data-ttu-id="ad9c7-538">ダウンロードをスキャンするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-538">Indicates whether or not to scan downloads.</span></span>|
|<span data-ttu-id="ad9c7-539">defenderScheduleScanEnableLowCpuPriority</span><span class="sxs-lookup"><span data-stu-id="ad9c7-539">defenderScheduleScanEnableLowCpuPriority</span></span>|<span data-ttu-id="ad9c7-540">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-540">Boolean</span></span>|<span data-ttu-id="ad9c7-541">有効にすると、スケジュールされたスキャン中に低い CPU 優先度が使用されます。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-541">When enabled, low CPU priority will be used during scheduled scans.</span></span>|
|<span data-ttu-id="ad9c7-542">defenderDisableCatchupQuickScan</span><span class="sxs-lookup"><span data-stu-id="ad9c7-542">defenderDisableCatchupQuickScan</span></span>|<span data-ttu-id="ad9c7-543">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-543">Boolean</span></span>|<span data-ttu-id="ad9c7-544">ブロックされている場合は、スケジュールされたクイックスキャンのキャッチアップスキャンが無効になります。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-544">When blocked, catch-up scans for scheduled quick scans will be turned off.</span></span>|
|<span data-ttu-id="ad9c7-545">defenderDisableCatchupFullScan</span><span class="sxs-lookup"><span data-stu-id="ad9c7-545">defenderDisableCatchupFullScan</span></span>|<span data-ttu-id="ad9c7-546">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-546">Boolean</span></span>|<span data-ttu-id="ad9c7-547">ブロックされている場合は、スケジュールされたフルスキャンのキャッチアップスキャンがオフになります。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-547">When blocked, catch-up scans for scheduled full scans will be turned off.</span></span>|
|<span data-ttu-id="ad9c7-548">defenderScanNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="ad9c7-548">defenderScanNetworkFiles</span></span>|<span data-ttu-id="ad9c7-549">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-549">Boolean</span></span>|<span data-ttu-id="ad9c7-550">ネットワーク フォルダーから開かれたファイルをスキャンするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-550">Indicates whether or not to scan files opened from a network folder.</span></span>|
|<span data-ttu-id="ad9c7-551">defenderScanIncomingMail</span><span class="sxs-lookup"><span data-stu-id="ad9c7-551">defenderScanIncomingMail</span></span>|<span data-ttu-id="ad9c7-552">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-552">Boolean</span></span>|<span data-ttu-id="ad9c7-553">受信メール メッセージをスキャンするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-553">Indicates whether or not to scan incoming mail messages.</span></span>|
|<span data-ttu-id="ad9c7-554">defenderScanMappedNetworkDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="ad9c7-554">defenderScanMappedNetworkDrivesDuringFullScan</span></span>|<span data-ttu-id="ad9c7-555">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-555">Boolean</span></span>|<span data-ttu-id="ad9c7-556">フル スキャン時に、マップされたネットワーク ドライブをスキャンするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-556">Indicates whether or not to scan mapped network drives during full scan.</span></span>|
|<span data-ttu-id="ad9c7-557">defenderScanRemovableDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="ad9c7-557">defenderScanRemovableDrivesDuringFullScan</span></span>|<span data-ttu-id="ad9c7-558">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-558">Boolean</span></span>|<span data-ttu-id="ad9c7-559">フル スキャン時に、リムーバブル ドライブをスキャンするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-559">Indicates whether or not to scan removable drives during full scan.</span></span>|
|<span data-ttu-id="ad9c7-560">defenderScanScriptsLoadedInInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="ad9c7-560">defenderScanScriptsLoadedInInternetExplorer</span></span>|<span data-ttu-id="ad9c7-561">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-561">Boolean</span></span>|<span data-ttu-id="ad9c7-562">Internet Explorer ブラウザーに読み込まれるスクリプトをスキャンするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-562">Indicates whether or not to scan scripts loaded in Internet Explorer browser.</span></span>|
|<span data-ttu-id="ad9c7-563">defenderSignatureUpdateIntervalInHours</span><span class="sxs-lookup"><span data-stu-id="ad9c7-563">defenderSignatureUpdateIntervalInHours</span></span>|<span data-ttu-id="ad9c7-564">Int32</span><span class="sxs-lookup"><span data-stu-id="ad9c7-564">Int32</span></span>|<span data-ttu-id="ad9c7-565">署名を更新する間隔 (時間)。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-565">The signature update interval in hours.</span></span> <span data-ttu-id="ad9c7-566">確認しない場合は 0 を指定します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-566">Specify 0 not to check.</span></span> <span data-ttu-id="ad9c7-567">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="ad9c7-567">Valid values 0 to 24</span></span>|
|<span data-ttu-id="ad9c7-568">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="ad9c7-568">defenderScanType</span></span>|[<span data-ttu-id="ad9c7-569">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="ad9c7-569">defenderScanType</span></span>](../resources/intune-deviceconfig-defenderscantype.md)|<span data-ttu-id="ad9c7-570">Defender システム スキャンの種類。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-570">The defender system scan type.</span></span> <span data-ttu-id="ad9c7-571">使用可能な値は、`userDefined`、`disabled`、`quick`、`full` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-571">Possible values are: `userDefined`, `disabled`, `quick`, `full`.</span></span>|
|<span data-ttu-id="ad9c7-572">defenderScheduledScanTime</span><span class="sxs-lookup"><span data-stu-id="ad9c7-572">defenderScheduledScanTime</span></span>|<span data-ttu-id="ad9c7-573">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="ad9c7-573">TimeOfDay</span></span>|<span data-ttu-id="ad9c7-574">システムのスキャンの Defender 時刻。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-574">The defender time for the system scan.</span></span>|
|<span data-ttu-id="ad9c7-575">defenderScheduledQuickScanTime</span><span class="sxs-lookup"><span data-stu-id="ad9c7-575">defenderScheduledQuickScanTime</span></span>|<span data-ttu-id="ad9c7-576">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="ad9c7-576">TimeOfDay</span></span>|<span data-ttu-id="ad9c7-577">毎日のクイック スキャンを実行する時刻。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-577">The time to perform a daily quick scan.</span></span>|
|<span data-ttu-id="ad9c7-578">defenderCloudBlockLevel</span><span class="sxs-lookup"><span data-stu-id="ad9c7-578">defenderCloudBlockLevel</span></span>|[<span data-ttu-id="ad9c7-579">defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="ad9c7-579">defenderCloudBlockLevelType</span></span>](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|<span data-ttu-id="ad9c7-580">クラウド配信の保護レベルを指定します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-580">Specifies the level of cloud-delivered protection.</span></span> <span data-ttu-id="ad9c7-581">可能な値は、`notConfigured`、`high`、`highPlus`、`zeroTolerance` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-581">Possible values are: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.</span></span>|
|<span data-ttu-id="ad9c7-582">defenderCloudExtendedTimeout</span><span class="sxs-lookup"><span data-stu-id="ad9c7-582">defenderCloudExtendedTimeout</span></span>|<span data-ttu-id="ad9c7-583">Int32</span><span class="sxs-lookup"><span data-stu-id="ad9c7-583">Int32</span></span>|<span data-ttu-id="ad9c7-584">クラウドによるファイルスキャンのタイムアウト拡張機能。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-584">Timeout extension for file scanning by the cloud.</span></span> <span data-ttu-id="ad9c7-585">有効な値は 0 から 50 までです</span><span class="sxs-lookup"><span data-stu-id="ad9c7-585">Valid values 0 to 50</span></span>|
|<span data-ttu-id="ad9c7-586">defenderCloudExtendedTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="ad9c7-586">defenderCloudExtendedTimeoutInSeconds</span></span>|<span data-ttu-id="ad9c7-587">Int32</span><span class="sxs-lookup"><span data-stu-id="ad9c7-587">Int32</span></span>|<span data-ttu-id="ad9c7-588">クラウドによるファイルスキャンのタイムアウト拡張機能。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-588">Timeout extension for file scanning by the cloud.</span></span> <span data-ttu-id="ad9c7-589">有効な値は 0 から 50 までです</span><span class="sxs-lookup"><span data-stu-id="ad9c7-589">Valid values 0 to 50</span></span>|
|<span data-ttu-id="ad9c7-590">defenderBlockOnAccessProtection</span><span class="sxs-lookup"><span data-stu-id="ad9c7-590">defenderBlockOnAccessProtection</span></span>|<span data-ttu-id="ad9c7-591">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-591">Boolean</span></span>|<span data-ttu-id="ad9c7-592">アクセス保護機能に対して Windows Defender を許可または拒否します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-592">Allows or disallows Windows Defender On Access Protection functionality.</span></span>|
|<span data-ttu-id="ad9c7-593">defenderSubmitSamplesConsentType</span><span class="sxs-lookup"><span data-stu-id="ad9c7-593">defenderSubmitSamplesConsentType</span></span>|[<span data-ttu-id="ad9c7-594">defenderSubmitSamplesConsentType</span><span class="sxs-lookup"><span data-stu-id="ad9c7-594">defenderSubmitSamplesConsentType</span></span>](../resources/intune-deviceconfig-defendersubmitsamplesconsenttype.md)|<span data-ttu-id="ad9c7-595">Windows Defender でデータを送信するためのユーザーの同意レベルを確認します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-595">Checks for the user consent level in Windows Defender to send data.</span></span> <span data-ttu-id="ad9c7-596">可能な値は、`sendSafeSamplesAutomatically`、`alwaysPrompt`、`neverSend`、`sendAllSamplesAutomatically` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-596">Possible values are: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.</span></span>|
|<span data-ttu-id="ad9c7-597">lockScreenAllowTimeoutConfiguration</span><span class="sxs-lookup"><span data-stu-id="ad9c7-597">lockScreenAllowTimeoutConfiguration</span></span>|<span data-ttu-id="ad9c7-598">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-598">Boolean</span></span>|<span data-ttu-id="ad9c7-599">Windows 10 Mobile デバイスのロック画面で、画面のタイムアウトを制御するユーザー構成可能な設定を表示するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-599">Specify whether to show a user-configurable setting to control the screen timeout while on the lock screen of Windows 10 Mobile devices.</span></span> <span data-ttu-id="ad9c7-600">このポリシーが [許可] に設定されている場合は、lockScreenTimeoutInSeconds によって設定された値は無視されます。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-600">If this policy is set to Allow, the value set by lockScreenTimeoutInSeconds is ignored.</span></span>|
|<span data-ttu-id="ad9c7-601">lockScreenBlockActionCenterNotifications</span><span class="sxs-lookup"><span data-stu-id="ad9c7-601">lockScreenBlockActionCenterNotifications</span></span>|<span data-ttu-id="ad9c7-602">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-602">Boolean</span></span>|<span data-ttu-id="ad9c7-603">ロック画面上のアクション センター通知を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-603">Indicates whether or not to block action center notifications over lock screen.</span></span>|
|<span data-ttu-id="ad9c7-604">lockScreenBlockCortana</span><span class="sxs-lookup"><span data-stu-id="ad9c7-604">lockScreenBlockCortana</span></span>|<span data-ttu-id="ad9c7-605">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-605">Boolean</span></span>|<span data-ttu-id="ad9c7-606">システムのロック中にユーザーが音声認識を使用して Cortana と対話できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-606">Indicates whether or not the user can interact with Cortana using speech while the system is locked.</span></span>|
|<span data-ttu-id="ad9c7-607">lockScreenBlockToastNotifications</span><span class="sxs-lookup"><span data-stu-id="ad9c7-607">lockScreenBlockToastNotifications</span></span>|<span data-ttu-id="ad9c7-608">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-608">Boolean</span></span>|<span data-ttu-id="ad9c7-609">デバイスのロック画面へのトースト通知を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-609">Indicates whether to allow toast notifications above the device lock screen.</span></span>|
|<span data-ttu-id="ad9c7-610">lockScreenTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="ad9c7-610">lockScreenTimeoutInSeconds</span></span>|<span data-ttu-id="ad9c7-611">Int32</span><span class="sxs-lookup"><span data-stu-id="ad9c7-611">Int32</span></span>|<span data-ttu-id="ad9c7-612">Windows 10 Mobile デバイスで画面をロックしてから画面をオフにするまでの時間 (秒) を設定します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-612">Set the duration (in seconds) from the screen locking to the screen turning off for Windows 10 Mobile devices.</span></span> <span data-ttu-id="ad9c7-613">サポートされている値は 11 から 1800 までです。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-613">Supported values are 11-1800.</span></span> <span data-ttu-id="ad9c7-614">有効な値は 11 から 1800 までです</span><span class="sxs-lookup"><span data-stu-id="ad9c7-614">Valid values 11 to 1800</span></span>|
|<span data-ttu-id="ad9c7-615">Lockscreen/Appswithvoice</span><span class="sxs-lookup"><span data-stu-id="ad9c7-615">lockScreenActivateAppsWithVoice</span></span>|[<span data-ttu-id="ad9c7-616">購入</span><span class="sxs-lookup"><span data-stu-id="ad9c7-616">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="ad9c7-617">このポリシー設定では、システムがロックされている間に、Windows アプリを音声でアクティブ化できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-617">This policy setting specifies whether Windows apps can be activated by voice while the system is locked.</span></span> <span data-ttu-id="ad9c7-618">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-618">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="ad9c7-619">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="ad9c7-619">passwordBlockSimple</span></span>|<span data-ttu-id="ad9c7-620">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-620">Boolean</span></span>|<span data-ttu-id="ad9c7-621">"1111" や "1234" などの PIN またはパスワードを許可するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-621">Specify whether PINs or passwords such as "1111" or "1234" are allowed.</span></span> <span data-ttu-id="ad9c7-622">Windows 10 デスクトップでは、ピクチャ パスワードの使用も制御します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-622">For Windows 10 desktops, it also controls the use of picture passwords.</span></span>|
|<span data-ttu-id="ad9c7-623">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="ad9c7-623">passwordExpirationDays</span></span>|<span data-ttu-id="ad9c7-624">Int32</span><span class="sxs-lookup"><span data-stu-id="ad9c7-624">Int32</span></span>|<span data-ttu-id="ad9c7-625">パスワードの有効期限 (日数)。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-625">The password expiration in days.</span></span> <span data-ttu-id="ad9c7-626">有効な値は 0 から 730 までです</span><span class="sxs-lookup"><span data-stu-id="ad9c7-626">Valid values 0 to 730</span></span>|
|<span data-ttu-id="ad9c7-627">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="ad9c7-627">passwordMinimumLength</span></span>|<span data-ttu-id="ad9c7-628">Int32</span><span class="sxs-lookup"><span data-stu-id="ad9c7-628">Int32</span></span>|<span data-ttu-id="ad9c7-629">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-629">The minimum password length.</span></span> <span data-ttu-id="ad9c7-630">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="ad9c7-630">Valid values 4 to 16</span></span>|
|<span data-ttu-id="ad9c7-631">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="ad9c7-631">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="ad9c7-632">Int32</span><span class="sxs-lookup"><span data-stu-id="ad9c7-632">Int32</span></span>|<span data-ttu-id="ad9c7-633">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-633">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="ad9c7-634">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="ad9c7-634">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="ad9c7-635">Int32</span><span class="sxs-lookup"><span data-stu-id="ad9c7-635">Int32</span></span>|<span data-ttu-id="ad9c7-636">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-636">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="ad9c7-637">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="ad9c7-637">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="ad9c7-638">Int32</span><span class="sxs-lookup"><span data-stu-id="ad9c7-638">Int32</span></span>|<span data-ttu-id="ad9c7-639">再使用を禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-639">The number of previous passwords to prevent reuse of.</span></span> <span data-ttu-id="ad9c7-640">有効な値は 0 から 50 までです</span><span class="sxs-lookup"><span data-stu-id="ad9c7-640">Valid values 0 to 50</span></span>|
|<span data-ttu-id="ad9c7-641">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="ad9c7-641">passwordRequired</span></span>|<span data-ttu-id="ad9c7-642">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-642">Boolean</span></span>|<span data-ttu-id="ad9c7-643">ユーザーにパスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-643">Indicates whether or not to require the user to have a password.</span></span>|
|<span data-ttu-id="ad9c7-644">passwordRequireWhenResumeFromIdleState</span><span class="sxs-lookup"><span data-stu-id="ad9c7-644">passwordRequireWhenResumeFromIdleState</span></span>|<span data-ttu-id="ad9c7-645">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-645">Boolean</span></span>|<span data-ttu-id="ad9c7-646">アイドル状態からの再開時にパスワードを要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-646">Indicates whether or not to require a password upon resuming from an idle state.</span></span>|
|<span data-ttu-id="ad9c7-647">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="ad9c7-647">passwordRequiredType</span></span>|[<span data-ttu-id="ad9c7-648">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="ad9c7-648">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="ad9c7-649">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-649">The required password type.</span></span> <span data-ttu-id="ad9c7-650">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-650">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="ad9c7-651">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="ad9c7-651">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="ad9c7-652">Int32</span><span class="sxs-lookup"><span data-stu-id="ad9c7-652">Int32</span></span>|<span data-ttu-id="ad9c7-653">出荷時の設定にリセットされるサインインの失敗回数。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-653">The number of sign in failures before factory reset.</span></span> <span data-ttu-id="ad9c7-654">有効な値は 0 から 999 までです</span><span class="sxs-lookup"><span data-stu-id="ad9c7-654">Valid values 0 to 999</span></span>|
|<span data-ttu-id="ad9c7-655">Passwordminimumagein Days</span><span class="sxs-lookup"><span data-stu-id="ad9c7-655">passwordMinimumAgeInDays</span></span>|<span data-ttu-id="ad9c7-656">Int32</span><span class="sxs-lookup"><span data-stu-id="ad9c7-656">Int32</span></span>|<span data-ttu-id="ad9c7-657">このセキュリティ設定では、ユーザーがパスワードを変更できるようになるまでの期間 (日数) を指定します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-657">This security setting determines the period of time (in days) that a password must be used before the user can change it.</span></span> <span data-ttu-id="ad9c7-658">有効な値は 0 ~ 998</span><span class="sxs-lookup"><span data-stu-id="ad9c7-658">Valid values 0 to 998</span></span>|
|<span data-ttu-id="ad9c7-659">privacyAdvertisingId</span><span class="sxs-lookup"><span data-stu-id="ad9c7-659">privacyAdvertisingId</span></span>|[<span data-ttu-id="ad9c7-660">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="ad9c7-660">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="ad9c7-661">広告識別子の使用を有効または無効にします。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-661">Enables or disables the use of advertising ID.</span></span> <span data-ttu-id="ad9c7-662">Windows 10 バージョン 1607 で追加されました。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-662">Added in Windows 10, version 1607.</span></span> <span data-ttu-id="ad9c7-663">可能な値は、`notConfigured`、`blocked`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-663">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="ad9c7-664">privacyAutoAcceptPairingAndConsentPrompts</span><span class="sxs-lookup"><span data-stu-id="ad9c7-664">privacyAutoAcceptPairingAndConsentPrompts</span></span>|<span data-ttu-id="ad9c7-665">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-665">Boolean</span></span>|<span data-ttu-id="ad9c7-666">アプリの起動時に、ペアリングとプライバシーに関するユーザーの同意ダイアログの自動受け入れを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-666">Indicates whether or not to allow the automatic acceptance of the pairing and privacy user consent dialog when launching apps.</span></span>|
|<span data-ttu-id="ad9c7-667">privacyDisableLaunchExperience</span><span class="sxs-lookup"><span data-stu-id="ad9c7-667">privacyDisableLaunchExperience</span></span>|<span data-ttu-id="ad9c7-668">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-668">Boolean</span></span>|<span data-ttu-id="ad9c7-669">このポリシーを使用すると、新規およびアップグレードされたユーザーに対して、ユーザーのログオン時にプライバシーを保護することができなくなります。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-669">This policy prevents the privacy experience from launching during user logon for new and upgraded users.</span></span>|
|<span data-ttu-id="ad9c7-670">privacyBlockInputPersonalization</span><span class="sxs-lookup"><span data-stu-id="ad9c7-670">privacyBlockInputPersonalization</span></span>|<span data-ttu-id="ad9c7-671">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-671">Boolean</span></span>|<span data-ttu-id="ad9c7-672">Cortana、音声入力、ストア アプリケーションに対するクラウド ベースの音声サービスの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-672">Indicates whether or not to block the usage of cloud based speech services for Cortana, Dictation, or Store applications.</span></span>|
|<span data-ttu-id="ad9c7-673">privacyBlockPublishUserActivities</span><span class="sxs-lookup"><span data-stu-id="ad9c7-673">privacyBlockPublishUserActivities</span></span>|<span data-ttu-id="ad9c7-674">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-674">Boolean</span></span>|<span data-ttu-id="ad9c7-675">タスクの切り替えなどで最近使用したリソースの共有エクスペリエンス/検出をブロックします。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-675">Blocks the shared experiences/discovery of recently used resources in task switcher etc.</span></span>|
|<span data-ttu-id="ad9c7-676">privacyBlockActivityFeed</span><span class="sxs-lookup"><span data-stu-id="ad9c7-676">privacyBlockActivityFeed</span></span>|<span data-ttu-id="ad9c7-677">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-677">Boolean</span></span>|<span data-ttu-id="ad9c7-678">Cortana、音声入力、またはストアアプリケーションに対するクラウドベースの音声サービスの使用をブロックします。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-678">Blocks the usage of cloud based speech services for Cortana, Dictation, or Store applications.</span></span>|
|<span data-ttu-id="ad9c7-679">startBlockUnpinningAppsFromTaskbar</span><span class="sxs-lookup"><span data-stu-id="ad9c7-679">startBlockUnpinningAppsFromTaskbar</span></span>|<span data-ttu-id="ad9c7-680">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-680">Boolean</span></span>|<span data-ttu-id="ad9c7-681">ユーザーがタスク バーからアプリのピン留めを外すことを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-681">Indicates whether or not to block the user from unpinning apps from taskbar.</span></span>|
|<span data-ttu-id="ad9c7-682">startMenuAppListVisibility</span><span class="sxs-lookup"><span data-stu-id="ad9c7-682">startMenuAppListVisibility</span></span>|[<span data-ttu-id="ad9c7-683">windowsStartMenuAppListVisibilityType</span><span class="sxs-lookup"><span data-stu-id="ad9c7-683">windowsStartMenuAppListVisibilityType</span></span>](../resources/intune-deviceconfig-windowsstartmenuapplistvisibilitytype.md)|<span data-ttu-id="ad9c7-684">この値を設定すると、アプリ リストを折りたたんだり、アプリ リスト全体を削除したり、設定アプリで対応する切り替えを無効にしたりできます。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-684">Setting the value of this collapses the app list, removes the app list entirely, or disables the corresponding toggle in the Settings app.</span></span> <span data-ttu-id="ad9c7-685">可能な値は、`userDefined`、`collapse`、`remove`、`disableSettingsApp` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-685">Possible values are: `userDefined`, `collapse`, `remove`, `disableSettingsApp`.</span></span>|
|<span data-ttu-id="ad9c7-686">startMenuHideChangeAccountSettings</span><span class="sxs-lookup"><span data-stu-id="ad9c7-686">startMenuHideChangeAccountSettings</span></span>|<span data-ttu-id="ad9c7-687">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-687">Boolean</span></span>|<span data-ttu-id="ad9c7-688">このポリシーを有効にすると、スタート メニューのユーザー タイルに [アカウント設定の変更] が表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-688">Enabling this policy hides the change account setting from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="ad9c7-689">startMenuHideFrequentlyUsedApps</span><span class="sxs-lookup"><span data-stu-id="ad9c7-689">startMenuHideFrequentlyUsedApps</span></span>|<span data-ttu-id="ad9c7-690">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-690">Boolean</span></span>|<span data-ttu-id="ad9c7-691">このポリシーを有効にすると、よく使われるアプリがスタート メニューに表示されなくなり、設定アプリで対応する切り替えが無効になります。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-691">Enabling this policy hides the most used apps from appearing on the start menu and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="ad9c7-692">startMenuHideHibernate</span><span class="sxs-lookup"><span data-stu-id="ad9c7-692">startMenuHideHibernate</span></span>|<span data-ttu-id="ad9c7-693">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-693">Boolean</span></span>|<span data-ttu-id="ad9c7-694">このポリシーを有効にすると、スタート メニューの電源ボタンに [休止状態] が表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-694">Enabling this policy hides hibernate from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="ad9c7-695">startMenuHideLock</span><span class="sxs-lookup"><span data-stu-id="ad9c7-695">startMenuHideLock</span></span>|<span data-ttu-id="ad9c7-696">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-696">Boolean</span></span>|<span data-ttu-id="ad9c7-697">このポリシーを有効にすると、スタート メニューのユーザー タイルに [ロック] が表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-697">Enabling this policy hides lock from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="ad9c7-698">startMenuHidePowerButton</span><span class="sxs-lookup"><span data-stu-id="ad9c7-698">startMenuHidePowerButton</span></span>|<span data-ttu-id="ad9c7-699">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-699">Boolean</span></span>|<span data-ttu-id="ad9c7-700">このポリシーを有効にすると、スタート メニューに電源ボタンが表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-700">Enabling this policy hides the power button from appearing in the start menu.</span></span>|
|<span data-ttu-id="ad9c7-701">startMenuHideRecentJumpLists</span><span class="sxs-lookup"><span data-stu-id="ad9c7-701">startMenuHideRecentJumpLists</span></span>|<span data-ttu-id="ad9c7-702">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-702">Boolean</span></span>|<span data-ttu-id="ad9c7-703">このポリシーを有効にすると、最近開いた項目のジャンプ リストがスタート メニュー/タスクバーに表示されなくなり、設定アプリで対応する切り替えが無効になります。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-703">Enabling this policy hides recent jump lists from appearing on the start menu/taskbar and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="ad9c7-704">startMenuHideRecentlyAddedApps</span><span class="sxs-lookup"><span data-stu-id="ad9c7-704">startMenuHideRecentlyAddedApps</span></span>|<span data-ttu-id="ad9c7-705">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-705">Boolean</span></span>|<span data-ttu-id="ad9c7-706">このポリシーを有効にすると、最近追加したアプリがスタート メニューに表示されなくなり、設定アプリで対応する切り替えが無効になります。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-706">Enabling this policy hides recently added apps from appearing on the start menu and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="ad9c7-707">startMenuHideRestartOptions</span><span class="sxs-lookup"><span data-stu-id="ad9c7-707">startMenuHideRestartOptions</span></span>|<span data-ttu-id="ad9c7-708">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-708">Boolean</span></span>|<span data-ttu-id="ad9c7-709">このポリシーを有効にすると、スタート メニューの電源ボタンに [再起動]/[更新して再起動] が表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-709">Enabling this policy hides “Restart/Update and Restart” from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="ad9c7-710">startMenuHideShutDown</span><span class="sxs-lookup"><span data-stu-id="ad9c7-710">startMenuHideShutDown</span></span>|<span data-ttu-id="ad9c7-711">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-711">Boolean</span></span>|<span data-ttu-id="ad9c7-712">このポリシーを有効にすると、スタート メニューの電源ボタンに [シャットダウン]/[更新してシャットダウン] が表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-712">Enabling this policy hides shut down/update and shut down from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="ad9c7-713">startMenuHideSignOut</span><span class="sxs-lookup"><span data-stu-id="ad9c7-713">startMenuHideSignOut</span></span>|<span data-ttu-id="ad9c7-714">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-714">Boolean</span></span>|<span data-ttu-id="ad9c7-715">このポリシーを有効にすると、スタート メニューのユーザー タイルに [サインアウト] が表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-715">Enabling this policy hides sign out from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="ad9c7-716">startMenuHideSleep</span><span class="sxs-lookup"><span data-stu-id="ad9c7-716">startMenuHideSleep</span></span>|<span data-ttu-id="ad9c7-717">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-717">Boolean</span></span>|<span data-ttu-id="ad9c7-718">このポリシーを有効にすると、スタート メニューの電源ボタンに [スリープ] が表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-718">Enabling this policy hides sleep from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="ad9c7-719">startMenuHideSwitchAccount</span><span class="sxs-lookup"><span data-stu-id="ad9c7-719">startMenuHideSwitchAccount</span></span>|<span data-ttu-id="ad9c7-720">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-720">Boolean</span></span>|<span data-ttu-id="ad9c7-721">このポリシーを有効にすると、スタート メニューのユーザー タイルに [アカウントの切り替え] が表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-721">Enabling this policy hides switch account from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="ad9c7-722">startMenuHideUserTile</span><span class="sxs-lookup"><span data-stu-id="ad9c7-722">startMenuHideUserTile</span></span>|<span data-ttu-id="ad9c7-723">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-723">Boolean</span></span>|<span data-ttu-id="ad9c7-724">このポリシーを有効にすると、スタート メニューにユーザー タイルが表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-724">Enabling this policy hides the user tile from appearing in the start menu.</span></span>|
|<span data-ttu-id="ad9c7-725">startMenuLayoutEdgeAssetsXml</span><span class="sxs-lookup"><span data-stu-id="ad9c7-725">startMenuLayoutEdgeAssetsXml</span></span>|<span data-ttu-id="ad9c7-726">Binary</span><span class="sxs-lookup"><span data-stu-id="ad9c7-726">Binary</span></span>|<span data-ttu-id="ad9c7-727">このポリシー設定では、Edge アセットをインポートして startMenuLayoutXml ポリシーで使用することができます。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-727">This policy setting allows you to import Edge assets to be used with startMenuLayoutXml policy.</span></span> <span data-ttu-id="ad9c7-728">スタートのレイアウトには、Edge アプリからのセカンダリ タイルを含めることができ、このタイルは Edge のローカル アセット ファイルを検索します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-728">Start layout can contain secondary tile from Edge app which looks for Edge local asset file.</span></span> <span data-ttu-id="ad9c7-729">Edge のローカル アセットは存在しないことがあり、その場合は Edge のセカンダリ タイルが空で表示されます。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-729">Edge local asset would not exist and cause Edge secondary tile to appear empty in this case.</span></span> <span data-ttu-id="ad9c7-730">このポリシーは、startMenuLayoutXml ポリシーが変更された場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-730">This policy only gets applied when startMenuLayoutXml policy is modified.</span></span> <span data-ttu-id="ad9c7-731">値は、UTF-8 の Base64 でエンコードされたバイト配列にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-731">The value should be a UTF-8 Base64 encoded byte array.</span></span>|
|<span data-ttu-id="ad9c7-732">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="ad9c7-732">startMenuLayoutXml</span></span>|<span data-ttu-id="ad9c7-733">Binary</span><span class="sxs-lookup"><span data-stu-id="ad9c7-733">Binary</span></span>|<span data-ttu-id="ad9c7-734">管理者がスタート メニューの既定のレイアウトを上書きし、ユーザーがこれを変更できないようにすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-734">Allows admins to override the default Start menu layout and prevents the user from changing it.</span></span> <span data-ttu-id="ad9c7-735">レイアウトを変更するには、レイアウト変更スキーマに基づく XML ファイルを指定します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-735">The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="ad9c7-736">XML は、UTF8 エンコードのバイト配列形式である必要があります。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-736">XML needs to be in a UTF8 encoded byte array format.</span></span>|
|<span data-ttu-id="ad9c7-737">startMenuMode</span><span class="sxs-lookup"><span data-stu-id="ad9c7-737">startMenuMode</span></span>|[<span data-ttu-id="ad9c7-738">windowsStartMenuModeType</span><span class="sxs-lookup"><span data-stu-id="ad9c7-738">windowsStartMenuModeType</span></span>](../resources/intune-deviceconfig-windowsstartmenumodetype.md)|<span data-ttu-id="ad9c7-739">管理者がスタート メニューの表示方法を決めることを許可します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-739">Allows admins to decide how the Start menu is displayed.</span></span> <span data-ttu-id="ad9c7-740">可能な値は、`userDefined`、`fullScreen`、`nonFullScreen` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-740">Possible values are: `userDefined`, `fullScreen`, `nonFullScreen`.</span></span>|
|<span data-ttu-id="ad9c7-741">startMenuPinnedFolderDocuments</span><span class="sxs-lookup"><span data-stu-id="ad9c7-741">startMenuPinnedFolderDocuments</span></span>|[<span data-ttu-id="ad9c7-742">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="ad9c7-742">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="ad9c7-743">スタート メニューへのドキュメント フォルダー ショートカットの表示/非表示を強制します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-743">Enforces the visibility (Show/Hide) of the Documents folder shortcut on the Start menu.</span></span> <span data-ttu-id="ad9c7-744">可能な値は、`notConfigured`、`hide`、`show` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-744">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="ad9c7-745">startMenuPinnedFolderDownloads</span><span class="sxs-lookup"><span data-stu-id="ad9c7-745">startMenuPinnedFolderDownloads</span></span>|[<span data-ttu-id="ad9c7-746">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="ad9c7-746">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="ad9c7-747">スタート メニューへのダウンロード フォルダー ショートカットの表示/非表示を強制します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-747">Enforces the visibility (Show/Hide) of the Downloads folder shortcut on the Start menu.</span></span> <span data-ttu-id="ad9c7-748">可能な値は、`notConfigured`、`hide`、`show` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-748">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="ad9c7-749">startMenuPinnedFolderFileExplorer</span><span class="sxs-lookup"><span data-stu-id="ad9c7-749">startMenuPinnedFolderFileExplorer</span></span>|[<span data-ttu-id="ad9c7-750">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="ad9c7-750">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="ad9c7-751">スタート メニューへのエクスプローラー ショートカットの表示/非表示を強制します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-751">Enforces the visibility (Show/Hide) of the FileExplorer shortcut on the Start menu.</span></span> <span data-ttu-id="ad9c7-752">可能な値は、`notConfigured`、`hide`、`show` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-752">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="ad9c7-753">startMenuPinnedFolderHomeGroup</span><span class="sxs-lookup"><span data-stu-id="ad9c7-753">startMenuPinnedFolderHomeGroup</span></span>|[<span data-ttu-id="ad9c7-754">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="ad9c7-754">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="ad9c7-755">スタート メニューへのホームグループ フォルダー ショートカットの表示/非表示を強制します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-755">Enforces the visibility (Show/Hide) of the HomeGroup folder shortcut on the Start menu.</span></span> <span data-ttu-id="ad9c7-756">可能な値は、`notConfigured`、`hide`、`show` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-756">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="ad9c7-757">startMenuPinnedFolderMusic</span><span class="sxs-lookup"><span data-stu-id="ad9c7-757">startMenuPinnedFolderMusic</span></span>|[<span data-ttu-id="ad9c7-758">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="ad9c7-758">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="ad9c7-759">スタート メニューへのミュージック フォルダー ショートカットの表示/非表示を強制します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-759">Enforces the visibility (Show/Hide) of the Music folder shortcut on the Start menu.</span></span> <span data-ttu-id="ad9c7-760">可能な値は、`notConfigured`、`hide`、`show` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-760">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="ad9c7-761">startMenuPinnedFolderNetwork</span><span class="sxs-lookup"><span data-stu-id="ad9c7-761">startMenuPinnedFolderNetwork</span></span>|[<span data-ttu-id="ad9c7-762">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="ad9c7-762">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="ad9c7-763">スタート メニューへのネットワーク フォルダー ショートカットの表示/非表示を強制します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-763">Enforces the visibility (Show/Hide) of the Network folder shortcut on the Start menu.</span></span> <span data-ttu-id="ad9c7-764">可能な値は、`notConfigured`、`hide`、`show` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-764">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="ad9c7-765">startMenuPinnedFolderPersonalFolder</span><span class="sxs-lookup"><span data-stu-id="ad9c7-765">startMenuPinnedFolderPersonalFolder</span></span>|[<span data-ttu-id="ad9c7-766">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="ad9c7-766">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="ad9c7-767">スタート メニューへの個人用フォルダー ショートカットの表示/非表示を強制します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-767">Enforces the visibility (Show/Hide) of the PersonalFolder shortcut on the Start menu.</span></span> <span data-ttu-id="ad9c7-768">可能な値は、`notConfigured`、`hide`、`show` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-768">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="ad9c7-769">startMenuPinnedFolderPictures</span><span class="sxs-lookup"><span data-stu-id="ad9c7-769">startMenuPinnedFolderPictures</span></span>|[<span data-ttu-id="ad9c7-770">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="ad9c7-770">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="ad9c7-771">スタート メニューへのピクチャ フォルダー ショートカットの表示/非表示を強制します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-771">Enforces the visibility (Show/Hide) of the Pictures folder shortcut on the Start menu.</span></span> <span data-ttu-id="ad9c7-772">可能な値は、`notConfigured`、`hide`、`show` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-772">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="ad9c7-773">startMenuPinnedFolderSettings</span><span class="sxs-lookup"><span data-stu-id="ad9c7-773">startMenuPinnedFolderSettings</span></span>|[<span data-ttu-id="ad9c7-774">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="ad9c7-774">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="ad9c7-775">スタート メニューへの設定フォルダー ショートカットの表示/非表示を強制します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-775">Enforces the visibility (Show/Hide) of the Settings folder shortcut on the Start menu.</span></span> <span data-ttu-id="ad9c7-776">可能な値は、`notConfigured`、`hide`、`show` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-776">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="ad9c7-777">startMenuPinnedFolderVideos</span><span class="sxs-lookup"><span data-stu-id="ad9c7-777">startMenuPinnedFolderVideos</span></span>|[<span data-ttu-id="ad9c7-778">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="ad9c7-778">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="ad9c7-779">スタート メニューへのビデオ フォルダー ショートカットの表示/非表示を強制します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-779">Enforces the visibility (Show/Hide) of the Videos folder shortcut on the Start menu.</span></span> <span data-ttu-id="ad9c7-780">可能な値は、`notConfigured`、`hide`、`show` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-780">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="ad9c7-781">settingsBlockSettingsApp</span><span class="sxs-lookup"><span data-stu-id="ad9c7-781">settingsBlockSettingsApp</span></span>|<span data-ttu-id="ad9c7-782">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-782">Boolean</span></span>|<span data-ttu-id="ad9c7-783">設定アプリへのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-783">Indicates whether or not to block access to Settings app.</span></span>|
|<span data-ttu-id="ad9c7-784">settingsBlockSystemPage</span><span class="sxs-lookup"><span data-stu-id="ad9c7-784">settingsBlockSystemPage</span></span>|<span data-ttu-id="ad9c7-785">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-785">Boolean</span></span>|<span data-ttu-id="ad9c7-786">設定アプリ内の [システム] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-786">Indicates whether or not to block access to System in Settings app.</span></span>|
|<span data-ttu-id="ad9c7-787">settingsBlockDevicesPage</span><span class="sxs-lookup"><span data-stu-id="ad9c7-787">settingsBlockDevicesPage</span></span>|<span data-ttu-id="ad9c7-788">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-788">Boolean</span></span>|<span data-ttu-id="ad9c7-789">設定アプリ内の [デバイス] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-789">Indicates whether or not to block access to Devices in Settings app.</span></span>|
|<span data-ttu-id="ad9c7-790">settingsBlockNetworkInternetPage</span><span class="sxs-lookup"><span data-stu-id="ad9c7-790">settingsBlockNetworkInternetPage</span></span>|<span data-ttu-id="ad9c7-791">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-791">Boolean</span></span>|<span data-ttu-id="ad9c7-792">設定アプリ内の [ネットワークとインターネット] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-792">Indicates whether or not to block access to Network & Internet in Settings app.</span></span>|
|<span data-ttu-id="ad9c7-793">settingsBlockPersonalizationPage</span><span class="sxs-lookup"><span data-stu-id="ad9c7-793">settingsBlockPersonalizationPage</span></span>|<span data-ttu-id="ad9c7-794">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-794">Boolean</span></span>|<span data-ttu-id="ad9c7-795">設定アプリ内の [個人用設定] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-795">Indicates whether or not to block access to Personalization in Settings app.</span></span>|
|<span data-ttu-id="ad9c7-796">settingsBlockAccountsPage</span><span class="sxs-lookup"><span data-stu-id="ad9c7-796">settingsBlockAccountsPage</span></span>|<span data-ttu-id="ad9c7-797">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-797">Boolean</span></span>|<span data-ttu-id="ad9c7-798">設定アプリ内の [アカウント] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-798">Indicates whether or not to block access to Accounts in Settings app.</span></span>|
|<span data-ttu-id="ad9c7-799">settingsBlockTimeLanguagePage</span><span class="sxs-lookup"><span data-stu-id="ad9c7-799">settingsBlockTimeLanguagePage</span></span>|<span data-ttu-id="ad9c7-800">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-800">Boolean</span></span>|<span data-ttu-id="ad9c7-801">設定アプリ内の [時刻と言語] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-801">Indicates whether or not to block access to Time & Language in Settings app.</span></span>|
|<span data-ttu-id="ad9c7-802">settingsBlockEaseOfAccessPage</span><span class="sxs-lookup"><span data-stu-id="ad9c7-802">settingsBlockEaseOfAccessPage</span></span>|<span data-ttu-id="ad9c7-803">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-803">Boolean</span></span>|<span data-ttu-id="ad9c7-804">設定アプリ内の [簡単操作] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-804">Indicates whether or not to block access to Ease of Access in Settings app.</span></span>|
|<span data-ttu-id="ad9c7-805">settingsBlockPrivacyPage</span><span class="sxs-lookup"><span data-stu-id="ad9c7-805">settingsBlockPrivacyPage</span></span>|<span data-ttu-id="ad9c7-806">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-806">Boolean</span></span>|<span data-ttu-id="ad9c7-807">設定アプリ内の [プライバシー] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-807">Indicates whether or not to block access to Privacy in Settings app.</span></span>|
|<span data-ttu-id="ad9c7-808">settingsBlockUpdateSecurityPage</span><span class="sxs-lookup"><span data-stu-id="ad9c7-808">settingsBlockUpdateSecurityPage</span></span>|<span data-ttu-id="ad9c7-809">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-809">Boolean</span></span>|<span data-ttu-id="ad9c7-810">設定アプリ内の [更新とセキュリティ] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-810">Indicates whether or not to block access to Update & Security in Settings app.</span></span>|
|<span data-ttu-id="ad9c7-811">settingsBlockAppsPage</span><span class="sxs-lookup"><span data-stu-id="ad9c7-811">settingsBlockAppsPage</span></span>|<span data-ttu-id="ad9c7-812">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-812">Boolean</span></span>|<span data-ttu-id="ad9c7-813">設定アプリ内の [アプリ] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-813">Indicates whether or not to block access to Apps in Settings app.</span></span>|
|<span data-ttu-id="ad9c7-814">settingsBlockGamingPage</span><span class="sxs-lookup"><span data-stu-id="ad9c7-814">settingsBlockGamingPage</span></span>|<span data-ttu-id="ad9c7-815">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-815">Boolean</span></span>|<span data-ttu-id="ad9c7-816">設定アプリ内の [ゲーム] へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-816">Indicates whether or not to block access to Gaming in Settings app.</span></span>|
|<span data-ttu-id="ad9c7-817">windowsSpotlightBlockConsumerSpecificFeatures</span><span class="sxs-lookup"><span data-stu-id="ad9c7-817">windowsSpotlightBlockConsumerSpecificFeatures</span></span>|<span data-ttu-id="ad9c7-818">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-818">Boolean</span></span>|<span data-ttu-id="ad9c7-819">通常はコンシューマー向けのエクスペリエンスを IT 管理者が禁止できるようにします。たとえば、開始時の提案、メンバーシップ通知、OOBE 後のアプリ インストール、リダイレクト タイルなどです。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-819">Allows IT admins to block experiences that are typically for consumers only, such as Start suggestions, Membership notifications, Post-OOBE app install and redirect tiles.</span></span>|
|<span data-ttu-id="ad9c7-820">windowsSpotlightBlocked</span><span class="sxs-lookup"><span data-stu-id="ad9c7-820">windowsSpotlightBlocked</span></span>|<span data-ttu-id="ad9c7-821">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-821">Boolean</span></span>|<span data-ttu-id="ad9c7-822">IT 管理者が Windows スポットライトのすべての機能をオフにできるようにします</span><span class="sxs-lookup"><span data-stu-id="ad9c7-822">Allows IT admins to turn off all Windows Spotlight features</span></span>|
|<span data-ttu-id="ad9c7-823">windowsSpotlightBlockOnActionCenter</span><span class="sxs-lookup"><span data-stu-id="ad9c7-823">windowsSpotlightBlockOnActionCenter</span></span>|<span data-ttu-id="ad9c7-824">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-824">Boolean</span></span>|<span data-ttu-id="ad9c7-825">各 OS のクリーン インストールやアップグレードの後、またはその後も継続的に、新しい機能や変更された機能を Microsoft からユーザーに紹介することを禁止します</span><span class="sxs-lookup"><span data-stu-id="ad9c7-825">Block suggestions from Microsoft that show after each OS clean install, upgrade or in an on-going basis to introduce users to what is new or changed</span></span>|
|<span data-ttu-id="ad9c7-826">windowsSpotlightBlockTailoredExperiences</span><span class="sxs-lookup"><span data-stu-id="ad9c7-826">windowsSpotlightBlockTailoredExperiences</span></span>|<span data-ttu-id="ad9c7-827">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-827">Boolean</span></span>|<span data-ttu-id="ad9c7-828">ユーザーのデバイスの使用状況に基づいて Windows スポットライトのコンテンツをカスタマイズすることを禁止します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-828">Block personalized content in Windows spotlight based on user’s device usage.</span></span>|
|<span data-ttu-id="ad9c7-829">windowsSpotlightBlockThirdPartyNotifications</span><span class="sxs-lookup"><span data-stu-id="ad9c7-829">windowsSpotlightBlockThirdPartyNotifications</span></span>|<span data-ttu-id="ad9c7-830">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-830">Boolean</span></span>|<span data-ttu-id="ad9c7-831">Windows スポットライト経由でサード パーティのコンテンツを配信することを禁止します</span><span class="sxs-lookup"><span data-stu-id="ad9c7-831">Block third party content delivered via Windows Spotlight</span></span>|
|<span data-ttu-id="ad9c7-832">windowsSpotlightBlockWelcomeExperience</span><span class="sxs-lookup"><span data-stu-id="ad9c7-832">windowsSpotlightBlockWelcomeExperience</span></span>|<span data-ttu-id="ad9c7-833">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-833">Boolean</span></span>|<span data-ttu-id="ad9c7-834">Windows スポットライトからの Windows へようこそのエクスペリエンスを禁止します</span><span class="sxs-lookup"><span data-stu-id="ad9c7-834">Block Windows Spotlight Windows welcome experience</span></span>|
|<span data-ttu-id="ad9c7-835">windowsSpotlightBlockWindowsTips</span><span class="sxs-lookup"><span data-stu-id="ad9c7-835">windowsSpotlightBlockWindowsTips</span></span>|<span data-ttu-id="ad9c7-836">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-836">Boolean</span></span>|<span data-ttu-id="ad9c7-837">Windows のヒントのポップアップを IT 管理者がオフにできるようにします。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-837">Allows IT admins to turn off the popup of Windows Tips.</span></span>|
|<span data-ttu-id="ad9c7-838">windowsSpotlightConfigureOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="ad9c7-838">windowsSpotlightConfigureOnLockScreen</span></span>|[<span data-ttu-id="ad9c7-839">Windowsスポットライト Enablementsettings</span><span class="sxs-lookup"><span data-stu-id="ad9c7-839">windowsSpotlightEnablementSettings</span></span>](../resources/intune-deviceconfig-windowsspotlightenablementsettings.md)|<span data-ttu-id="ad9c7-840">スポットライトの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-840">Specifies the type of Spotlight.</span></span> <span data-ttu-id="ad9c7-841">可能な値は、`notConfigured`、`disabled`、`enabled` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-841">Possible values are: `notConfigured`, `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="ad9c7-842">networkProxyApplySettingsDeviceWide</span><span class="sxs-lookup"><span data-stu-id="ad9c7-842">networkProxyApplySettingsDeviceWide</span></span>|<span data-ttu-id="ad9c7-843">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-843">Boolean</span></span>|<span data-ttu-id="ad9c7-844">オンに設定すると、プロキシの設定がデバイスのすべてのプロセスとアカウントに適用されます。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-844">If set, proxy settings will be applied to all processes and accounts in the device.</span></span> <span data-ttu-id="ad9c7-845">それ以外の場合は、MDM に登録されているユーザー アカウントに適用されます。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-845">Otherwise, it will be applied to the user account that’s enrolled into MDM.</span></span>|
|<span data-ttu-id="ad9c7-846">networkProxyDisableAutoDetect</span><span class="sxs-lookup"><span data-stu-id="ad9c7-846">networkProxyDisableAutoDetect</span></span>|<span data-ttu-id="ad9c7-847">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-847">Boolean</span></span>|<span data-ttu-id="ad9c7-848">設定の自動検出を無効にします。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-848">Disable automatic detection of settings.</span></span> <span data-ttu-id="ad9c7-849">有効にした場合、システムはプロキシ自動構成 (PAC) スクリプトへのパスを検索します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-849">If enabled, the system will try to find the path to a proxy auto-config (PAC) script.</span></span>|
|<span data-ttu-id="ad9c7-850">networkProxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="ad9c7-850">networkProxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="ad9c7-851">String</span><span class="sxs-lookup"><span data-stu-id="ad9c7-851">String</span></span>|<span data-ttu-id="ad9c7-852">使用するプロキシ自動構成 (PAC) スクリプトのアドレス。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-852">Address to the proxy auto-config (PAC) script you want to use.</span></span>|
|<span data-ttu-id="ad9c7-853">networkProxyServer</span><span class="sxs-lookup"><span data-stu-id="ad9c7-853">networkProxyServer</span></span>|[<span data-ttu-id="ad9c7-854">windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="ad9c7-854">windows10NetworkProxyServer</span></span>](../resources/intune-deviceconfig-windows10networkproxyserver.md)|<span data-ttu-id="ad9c7-855">プロキシ サーバーの設定を手動で指定します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-855">Specifies manual proxy server settings.</span></span>|
|<span data-ttu-id="ad9c7-856">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="ad9c7-856">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="ad9c7-857">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-857">Boolean</span></span>|<span data-ttu-id="ad9c7-858">Microsoft アカウントに関連付けられていない電子メール アカウントをユーザーがデバイスに追加できないようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-858">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="ad9c7-859">antiTheftModeBlocked</span><span class="sxs-lookup"><span data-stu-id="ad9c7-859">antiTheftModeBlocked</span></span>|<span data-ttu-id="ad9c7-860">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-860">Boolean</span></span>|<span data-ttu-id="ad9c7-861">ユーザーが盗難防止モードの設定を選択することを禁止するかどうかを示します (Windows 10 Mobile のみ)。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-861">Indicates whether or not to block the user from selecting an AntiTheft mode preference (Windows 10 Mobile only).</span></span>|
|<span data-ttu-id="ad9c7-862">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="ad9c7-862">bluetoothBlocked</span></span>|<span data-ttu-id="ad9c7-863">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-863">Boolean</span></span>|<span data-ttu-id="ad9c7-864">ユーザーが Bluetooth を使用することを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-864">Whether or not to Block the user from using bluetooth.</span></span>|
|<span data-ttu-id="ad9c7-865">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="ad9c7-865">cameraBlocked</span></span>|<span data-ttu-id="ad9c7-866">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-866">Boolean</span></span>|<span data-ttu-id="ad9c7-867">ユーザーがデバイスのカメラにアクセスすることを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-867">Whether or not to Block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="ad9c7-868">connectedDevicesServiceBlocked</span><span class="sxs-lookup"><span data-stu-id="ad9c7-868">connectedDevicesServiceBlocked</span></span>|<span data-ttu-id="ad9c7-869">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-869">Boolean</span></span>|<span data-ttu-id="ad9c7-870">他のデバイスの検出と接続、リモート メッセージング、リモート アプリ セッション、その他のデバイス間エクスペリエンスを可能にする、接続されているデバイスのサービスを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-870">Whether or not to block Connected Devices Service which enables discovery and connection to other devices, remote messaging, remote app sessions and other cross-device experiences.</span></span>|
|<span data-ttu-id="ad9c7-871">certificatesBlockManualRootCertificateInstallation</span><span class="sxs-lookup"><span data-stu-id="ad9c7-871">certificatesBlockManualRootCertificateInstallation</span></span>|<span data-ttu-id="ad9c7-872">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-872">Boolean</span></span>|<span data-ttu-id="ad9c7-873">ユーザーが手動でルート証明書をインストールすることを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-873">Whether or not to Block the user from doing manual root certificate installation.</span></span>|
|<span data-ttu-id="ad9c7-874">copyPasteBlocked</span><span class="sxs-lookup"><span data-stu-id="ad9c7-874">copyPasteBlocked</span></span>|<span data-ttu-id="ad9c7-875">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-875">Boolean</span></span>|<span data-ttu-id="ad9c7-876">ユーザーがコピーと貼り付けを使用することを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-876">Whether or not to Block the user from using copy paste.</span></span>|
|<span data-ttu-id="ad9c7-877">cortanaBlocked</span><span class="sxs-lookup"><span data-stu-id="ad9c7-877">cortanaBlocked</span></span>|<span data-ttu-id="ad9c7-878">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-878">Boolean</span></span>|<span data-ttu-id="ad9c7-879">ユーザーが Cortana を使用することを禁止するかどうか。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-879">Whether or not to Block the user from using Cortana.</span></span>|
|<span data-ttu-id="ad9c7-880">deviceManagementBlockFactoryResetOnMobile</span><span class="sxs-lookup"><span data-stu-id="ad9c7-880">deviceManagementBlockFactoryResetOnMobile</span></span>|<span data-ttu-id="ad9c7-881">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-881">Boolean</span></span>|<span data-ttu-id="ad9c7-882">ユーザーが携帯電話をリセットすることを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-882">Indicates whether or not to Block the user from resetting their phone.</span></span>|
|<span data-ttu-id="ad9c7-883">deviceManagementBlockManualUnenroll</span><span class="sxs-lookup"><span data-stu-id="ad9c7-883">deviceManagementBlockManualUnenroll</span></span>|<span data-ttu-id="ad9c7-884">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-884">Boolean</span></span>|<span data-ttu-id="ad9c7-885">ユーザーがデバイス管理から手動で登録解除を行うことを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-885">Indicates whether or not to Block the user from doing manual un-enrollment from device management.</span></span>|
|<span data-ttu-id="ad9c7-886">safeSearchFilter</span><span class="sxs-lookup"><span data-stu-id="ad9c7-886">safeSearchFilter</span></span>|[<span data-ttu-id="ad9c7-887">safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="ad9c7-887">safeSearchFilterType</span></span>](../resources/intune-deviceconfig-safesearchfiltertype.md)|<span data-ttu-id="ad9c7-888">セーフ サーチに必要なフィルター レベルを指定します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-888">Specifies what filter level of safe search is required.</span></span> <span data-ttu-id="ad9c7-889">可能な値は、`userDefined`、`strict`、`moderate` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-889">Possible values are: `userDefined`, `strict`, `moderate`.</span></span>|
|<span data-ttu-id="ad9c7-890">edgeBlockPopups</span><span class="sxs-lookup"><span data-stu-id="ad9c7-890">edgeBlockPopups</span></span>|<span data-ttu-id="ad9c7-891">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-891">Boolean</span></span>|<span data-ttu-id="ad9c7-892">ポップアップをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-892">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="ad9c7-893">edgeBlockSearchSuggestions</span><span class="sxs-lookup"><span data-stu-id="ad9c7-893">edgeBlockSearchSuggestions</span></span>|<span data-ttu-id="ad9c7-894">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-894">Boolean</span></span>|<span data-ttu-id="ad9c7-895">ユーザーがアドレスバーの検索候補を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-895">Indicates whether or not to block the user from using the search suggestions in the address bar.</span></span>|
|<span data-ttu-id="ad9c7-896">edgeBlockSearchEngineCustomization</span><span class="sxs-lookup"><span data-stu-id="ad9c7-896">edgeBlockSearchEngineCustomization</span></span>|<span data-ttu-id="ad9c7-897">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-897">Boolean</span></span>|<span data-ttu-id="ad9c7-898">ユーザーが新しい検索エンジンを追加したり、既定の検索エンジンを変更したりすることを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-898">Indicates whether or not to block the user from adding new search engine or changing the default search engine.</span></span>|
|<span data-ttu-id="ad9c7-899">edgeBlockSendingIntranetTrafficToInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="ad9c7-899">edgeBlockSendingIntranetTrafficToInternetExplorer</span></span>|<span data-ttu-id="ad9c7-900">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-900">Boolean</span></span>|<span data-ttu-id="ad9c7-901">イントラネットトラフィックをエッジから Internet Explorer に切り替えるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-901">Indicates whether or not to switch the intranet traffic from Edge to Internet Explorer.</span></span> <span data-ttu-id="ad9c7-902">注: このプロパティの名前は誤解されています。このプロパティは現在使用されていません。代わりに EdgeSendIntranetTrafficToInternetExplorer を使用してください。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-902">Note: the name of this property is misleading; the property is obsolete, use EdgeSendIntranetTrafficToInternetExplorer instead.</span></span>|
|<span data-ttu-id="ad9c7-903">edgeSendIntranetTrafficToInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="ad9c7-903">edgeSendIntranetTrafficToInternetExplorer</span></span>|<span data-ttu-id="ad9c7-904">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-904">Boolean</span></span>|<span data-ttu-id="ad9c7-905">イントラネットトラフィックをエッジから Internet Explorer に切り替えるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-905">Indicates whether or not to switch the intranet traffic from Edge to Internet Explorer.</span></span>|
|<span data-ttu-id="ad9c7-906">edgeRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="ad9c7-906">edgeRequireSmartScreen</span></span>|<span data-ttu-id="ad9c7-907">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-907">Boolean</span></span>|<span data-ttu-id="ad9c7-908">スマート スクリーン フィルターの使用をユーザーに要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-908">Indicates whether or not to Require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="ad9c7-909">edgeEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="ad9c7-909">edgeEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="ad9c7-910">String</span><span class="sxs-lookup"><span data-stu-id="ad9c7-910">String</span></span>|<span data-ttu-id="ad9c7-911">エンタープライズ モードのサイト リストの場所を示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-911">Indicates the enterprise mode site list location.</span></span> <span data-ttu-id="ad9c7-912">ローカル ファイル、ローカル ネットワーク、http の場所が該当します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-912">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="ad9c7-913">edgeFirstRunUrl</span><span class="sxs-lookup"><span data-stu-id="ad9c7-913">edgeFirstRunUrl</span></span>|<span data-ttu-id="ad9c7-914">String</span><span class="sxs-lookup"><span data-stu-id="ad9c7-914">String</span></span>|<span data-ttu-id="ad9c7-915">Edge ブラウザーを初めて開いたときに最初に実行される URL です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-915">The first run URL for when Edge browser is opened for the first time.</span></span>|
|<span data-ttu-id="ad9c7-916">edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="ad9c7-916">edgeSearchEngine</span></span>|[<span data-ttu-id="ad9c7-917">edgeSearchEngineBase</span><span class="sxs-lookup"><span data-stu-id="ad9c7-917">edgeSearchEngineBase</span></span>](../resources/intune-deviceconfig-edgesearchenginebase.md)|<span data-ttu-id="ad9c7-918">IT 管理者が MDM 制御デバイス用の既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-918">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="ad9c7-919">AllowSearchEngineCustomization ポリシーが設定されていない場合、ユーザーは上書きして既定の検索エンジンを変更することができます。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-919">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>|
|<span data-ttu-id="ad9c7-920">edgeHomepageUrls</span><span class="sxs-lookup"><span data-stu-id="ad9c7-920">edgeHomepageUrls</span></span>|<span data-ttu-id="ad9c7-921">String コレクション</span><span class="sxs-lookup"><span data-stu-id="ad9c7-921">String collection</span></span>|<span data-ttu-id="ad9c7-922">MDM に登録されているデバイスの Edge ブラウザーに表示されるホームページの URL の一覧です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-922">The list of URLs for homepages shodwn on MDM-enrolled devices on Edge browser.</span></span>|
|<span data-ttu-id="ad9c7-923">edgeBlockAccessToAboutFlags</span><span class="sxs-lookup"><span data-stu-id="ad9c7-923">edgeBlockAccessToAboutFlags</span></span>|<span data-ttu-id="ad9c7-924">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-924">Boolean</span></span>|<span data-ttu-id="ad9c7-925">Edge ブラウザーの about:flags へのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-925">Indicates whether or not to prevent access to about flags on Edge browser.</span></span>|
|<span data-ttu-id="ad9c7-926">smartScreenBlockPromptOverride</span><span class="sxs-lookup"><span data-stu-id="ad9c7-926">smartScreenBlockPromptOverride</span></span>|<span data-ttu-id="ad9c7-927">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-927">Boolean</span></span>|<span data-ttu-id="ad9c7-928">悪意のある Web サイトの可能性があるサイトに関する SmartScreen フィルターの警告をユーザーが無視できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-928">Indicates whether or not users can override SmartScreen Filter warnings about potentially malicious websites.</span></span>|
|<span data-ttu-id="ad9c7-929">smartScreenBlockPromptOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="ad9c7-929">smartScreenBlockPromptOverrideForFiles</span></span>|<span data-ttu-id="ad9c7-930">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-930">Boolean</span></span>|<span data-ttu-id="ad9c7-931">未検証のファイルのダウンロードに関する SmartScreen フィルターの警告をユーザーが無視できるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ad9c7-931">Indicates whether or not users can override the SmartScreen Filter warnings about downloading unverified files</span></span>|
|<span data-ttu-id="ad9c7-932">webRtcBlockLocalhostIpAddress</span><span class="sxs-lookup"><span data-stu-id="ad9c7-932">webRtcBlockLocalhostIpAddress</span></span>|<span data-ttu-id="ad9c7-933">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-933">Boolean</span></span>|<span data-ttu-id="ad9c7-934">WebRTC を使用して通話を発信しているときにユーザーのローカル ホストの IP アドレスが表示されるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ad9c7-934">Indicates whether or not user's localhost IP address is displayed while making phone calls using the WebRTC</span></span>|
|<span data-ttu-id="ad9c7-935">internetSharingBlocked</span><span class="sxs-lookup"><span data-stu-id="ad9c7-935">internetSharingBlocked</span></span>|<span data-ttu-id="ad9c7-936">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-936">Boolean</span></span>|<span data-ttu-id="ad9c7-937">ユーザーがインターネット共有を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-937">Indicates whether or not to Block the user from using internet sharing.</span></span>|
|<span data-ttu-id="ad9c7-938">settingsBlockAddProvisioningPackage</span><span class="sxs-lookup"><span data-stu-id="ad9c7-938">settingsBlockAddProvisioningPackage</span></span>|<span data-ttu-id="ad9c7-939">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-939">Boolean</span></span>|<span data-ttu-id="ad9c7-940">ユーザーがプロビジョニング パッケージをインストールすることを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-940">Indicates whether or not to block the user from installing provisioning packages.</span></span>|
|<span data-ttu-id="ad9c7-941">settingsBlockRemoveProvisioningPackage</span><span class="sxs-lookup"><span data-stu-id="ad9c7-941">settingsBlockRemoveProvisioningPackage</span></span>|<span data-ttu-id="ad9c7-942">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-942">Boolean</span></span>|<span data-ttu-id="ad9c7-943">ランタイム構成エージェントがプロビジョニング パッケージを削除することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-943">Indicates whether or not to block the runtime configuration agent from removing provisioning packages.</span></span>|
|<span data-ttu-id="ad9c7-944">settingsBlockChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="ad9c7-944">settingsBlockChangeSystemTime</span></span>|<span data-ttu-id="ad9c7-945">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-945">Boolean</span></span>|<span data-ttu-id="ad9c7-946">ユーザーが日付と時刻の設定を変更することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-946">Indicates whether or not to block the user from changing date and time settings.</span></span>|
|<span data-ttu-id="ad9c7-947">settingsBlockEditDeviceName</span><span class="sxs-lookup"><span data-stu-id="ad9c7-947">settingsBlockEditDeviceName</span></span>|<span data-ttu-id="ad9c7-948">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-948">Boolean</span></span>|<span data-ttu-id="ad9c7-949">ユーザーがデバイス名を編集することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-949">Indicates whether or not to block the user from editing the device name.</span></span>|
|<span data-ttu-id="ad9c7-950">settingsBlockChangeRegion</span><span class="sxs-lookup"><span data-stu-id="ad9c7-950">settingsBlockChangeRegion</span></span>|<span data-ttu-id="ad9c7-951">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-951">Boolean</span></span>|<span data-ttu-id="ad9c7-952">ユーザーがリージョン設定を変更することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-952">Indicates whether or not to block the user from changing the region settings.</span></span>|
|<span data-ttu-id="ad9c7-953">settingsBlockChangeLanguage</span><span class="sxs-lookup"><span data-stu-id="ad9c7-953">settingsBlockChangeLanguage</span></span>|<span data-ttu-id="ad9c7-954">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-954">Boolean</span></span>|<span data-ttu-id="ad9c7-955">ユーザーが言語の設定を変更することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-955">Indicates whether or not to block the user from changing the language settings.</span></span>|
|<span data-ttu-id="ad9c7-956">settingsBlockChangePowerSleep</span><span class="sxs-lookup"><span data-stu-id="ad9c7-956">settingsBlockChangePowerSleep</span></span>|<span data-ttu-id="ad9c7-957">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-957">Boolean</span></span>|<span data-ttu-id="ad9c7-958">ユーザーが電源とスリープの設定を変更することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-958">Indicates whether or not to block the user from changing power and sleep settings.</span></span>|
|<span data-ttu-id="ad9c7-959">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="ad9c7-959">locationServicesBlocked</span></span>|<span data-ttu-id="ad9c7-960">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-960">Boolean</span></span>|<span data-ttu-id="ad9c7-961">ユーザーが位置情報サービスを使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-961">Indicates whether or not to Block the user from location services.</span></span>|
|<span data-ttu-id="ad9c7-962">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="ad9c7-962">microsoftAccountBlocked</span></span>|<span data-ttu-id="ad9c7-963">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-963">Boolean</span></span>|<span data-ttu-id="ad9c7-964">Microsoft アカウントを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-964">Indicates whether or not to Block a Microsoft account.</span></span>|
|<span data-ttu-id="ad9c7-965">microsoftAccountBlockSettingsSync</span><span class="sxs-lookup"><span data-stu-id="ad9c7-965">microsoftAccountBlockSettingsSync</span></span>|<span data-ttu-id="ad9c7-966">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-966">Boolean</span></span>|<span data-ttu-id="ad9c7-967">Microsoft アカウントの設定の同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-967">Indicates whether or not to Block Microsoft account settings sync.</span></span>|
|<span data-ttu-id="ad9c7-968">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="ad9c7-968">nfcBlocked</span></span>|<span data-ttu-id="ad9c7-969">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-969">Boolean</span></span>|<span data-ttu-id="ad9c7-970">ユーザーが近距離無線通信を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-970">Indicates whether or not to Block the user from using near field communication.</span></span>|
|<span data-ttu-id="ad9c7-971">resetProtectionModeBlocked</span><span class="sxs-lookup"><span data-stu-id="ad9c7-971">resetProtectionModeBlocked</span></span>|<span data-ttu-id="ad9c7-972">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-972">Boolean</span></span>|<span data-ttu-id="ad9c7-973">ユーザーが保護モードをリセットすることを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-973">Indicates whether or not to Block the user from reset protection mode.</span></span>|
|<span data-ttu-id="ad9c7-974">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="ad9c7-974">screenCaptureBlocked</span></span>|<span data-ttu-id="ad9c7-975">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-975">Boolean</span></span>|<span data-ttu-id="ad9c7-976">ユーザーがスクリーンショットを撮ることを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-976">Indicates whether or not to Block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="ad9c7-977">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="ad9c7-977">storageBlockRemovableStorage</span></span>|<span data-ttu-id="ad9c7-978">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-978">Boolean</span></span>|<span data-ttu-id="ad9c7-979">ユーザーがリムーバブル記憶域を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-979">Indicates whether or not to Block the user from using removable storage.</span></span>|
|<span data-ttu-id="ad9c7-980">storageRequireMobileDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="ad9c7-980">storageRequireMobileDeviceEncryption</span></span>|<span data-ttu-id="ad9c7-981">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-981">Boolean</span></span>|<span data-ttu-id="ad9c7-982">モバイル デバイスでの暗号化が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-982">Indicating whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="ad9c7-983">usbBlocked</span><span class="sxs-lookup"><span data-stu-id="ad9c7-983">usbBlocked</span></span>|<span data-ttu-id="ad9c7-984">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-984">Boolean</span></span>|<span data-ttu-id="ad9c7-985">ユーザーが USB 接続を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-985">Indicates whether or not to Block the user from USB connection.</span></span>|
|<span data-ttu-id="ad9c7-986">voiceRecordingBlocked</span><span class="sxs-lookup"><span data-stu-id="ad9c7-986">voiceRecordingBlocked</span></span>|<span data-ttu-id="ad9c7-987">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-987">Boolean</span></span>|<span data-ttu-id="ad9c7-988">ユーザーが音声録音を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-988">Indicates whether or not to Block the user from voice recording.</span></span>|
|<span data-ttu-id="ad9c7-989">wiFiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="ad9c7-989">wiFiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="ad9c7-990">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-990">Boolean</span></span>|<span data-ttu-id="ad9c7-991">Wi-Fi ホットスポットへの自動接続を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-991">Indicating whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="ad9c7-992">Wi-Fi がブロックされていれば、この値は関係ありません。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-992">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="ad9c7-993">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="ad9c7-993">wiFiBlocked</span></span>|<span data-ttu-id="ad9c7-994">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-994">Boolean</span></span>|<span data-ttu-id="ad9c7-995">ユーザーが Wi-Fi を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-995">Indicates whether or not to Block the user from using Wi-Fi.</span></span>|
|<span data-ttu-id="ad9c7-996">wiFiBlockManualConfiguration</span><span class="sxs-lookup"><span data-stu-id="ad9c7-996">wiFiBlockManualConfiguration</span></span>|<span data-ttu-id="ad9c7-997">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-997">Boolean</span></span>|<span data-ttu-id="ad9c7-998">ユーザーが Wi-Fi の手動構成を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-998">Indicates whether or not to Block the user from using Wi-Fi manual configuration.</span></span>|
|<span data-ttu-id="ad9c7-999">wiFiScanInterval</span><span class="sxs-lookup"><span data-stu-id="ad9c7-999">wiFiScanInterval</span></span>|<span data-ttu-id="ad9c7-1000">Int32</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1000">Int32</span></span>|<span data-ttu-id="ad9c7-1001">Wi-Fi ネットワークに対するデバイス スキャンの頻度を指定します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1001">Specify how often devices scan for Wi-Fi networks.</span></span> <span data-ttu-id="ad9c7-1002">サポートされている値は 1 から 500 まで、既定値は 100、500 は最低頻度です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1002">Supported values are 1-500, where 100 = default, and 500 = low frequency.</span></span> <span data-ttu-id="ad9c7-1003">有効な値は 1 から 500 までです</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1003">Valid values 1 to 500</span></span>|
|<span data-ttu-id="ad9c7-1004">wirelessDisplayBlockProjectionToThisDevice</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1004">wirelessDisplayBlockProjectionToThisDevice</span></span>|<span data-ttu-id="ad9c7-1005">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1005">Boolean</span></span>|<span data-ttu-id="ad9c7-1006">他のデバイスがこの PC をプロジェクター用に検出することを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1006">Indicates whether or not to allow other devices from discovering this PC for projection.</span></span>|
|<span data-ttu-id="ad9c7-1007">wirelessDisplayBlockUserInputFromReceiver</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1007">wirelessDisplayBlockUserInputFromReceiver</span></span>|<span data-ttu-id="ad9c7-1008">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1008">Boolean</span></span>|<span data-ttu-id="ad9c7-1009">ワイヤレス ディスプレイ レシーバーからのユーザー入力を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1009">Indicates whether or not to allow user input from wireless display receiver.</span></span>|
|<span data-ttu-id="ad9c7-1010">wirelessDisplayRequirePinForPairing</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1010">wirelessDisplayRequirePinForPairing</span></span>|<span data-ttu-id="ad9c7-1011">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1011">Boolean</span></span>|<span data-ttu-id="ad9c7-1012">新しいデバイスがペアリングを開始するときに PIN が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1012">Indicates whether or not to require a PIN for new devices to initiate pairing.</span></span>|
|<span data-ttu-id="ad9c7-1013">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1013">windowsStoreBlocked</span></span>|<span data-ttu-id="ad9c7-1014">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1014">Boolean</span></span>|<span data-ttu-id="ad9c7-1015">ユーザーが Windows ストアを使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1015">Indicates whether or not to Block the user from using the Windows store.</span></span>|
|<span data-ttu-id="ad9c7-1016">appsAllowTrustedAppsSideloading</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1016">appsAllowTrustedAppsSideloading</span></span>|[<span data-ttu-id="ad9c7-1017">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1017">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="ad9c7-1018">信頼された証明書で署名した AppX パッケージからアプリをサイドローディングできるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1018">Indicates whether apps from AppX packages signed with a trusted certificate can be side loaded.</span></span> <span data-ttu-id="ad9c7-1019">可能な値は、`notConfigured`、`blocked`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1019">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="ad9c7-1020">windowsStoreBlockAutoUpdate</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1020">windowsStoreBlockAutoUpdate</span></span>|<span data-ttu-id="ad9c7-1021">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1021">Boolean</span></span>|<span data-ttu-id="ad9c7-1022">Windows ストアからのアプリの自動更新を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1022">Indicates whether or not to block automatic update of apps from Windows Store.</span></span>|
|<span data-ttu-id="ad9c7-1023">developerUnlockSetting</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1023">developerUnlockSetting</span></span>|[<span data-ttu-id="ad9c7-1024">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1024">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="ad9c7-1025">開発者によるロック解除を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1025">Indicates whether or not to allow developer unlock.</span></span> <span data-ttu-id="ad9c7-1026">可能な値は、`notConfigured`、`blocked`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1026">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="ad9c7-1027">sharedUserAppDataAllowed</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1027">sharedUserAppDataAllowed</span></span>|<span data-ttu-id="ad9c7-1028">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1028">Boolean</span></span>|<span data-ttu-id="ad9c7-1029">同じアプリの複数のユーザーによるデータ共有を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1029">Indicates whether or not to block multiple users of the same app to share data.</span></span>|
|<span data-ttu-id="ad9c7-1030">appsBlockWindowsStoreOriginatedApps</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1030">appsBlockWindowsStoreOriginatedApps</span></span>|<span data-ttu-id="ad9c7-1031">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1031">Boolean</span></span>|<span data-ttu-id="ad9c7-1032">プレインストールまたはダウンロードによって取得したすべての Windows ストア アプリの起動を無効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1032">Indicates whether or not to disable the launch of all apps from Windows Store that came pre-installed or were downloaded.</span></span>|
|<span data-ttu-id="ad9c7-1033">windowsStoreEnablePrivateStoreOnly</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1033">windowsStoreEnablePrivateStoreOnly</span></span>|<span data-ttu-id="ad9c7-1034">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1034">Boolean</span></span>|<span data-ttu-id="ad9c7-1035">プライベート ストアのみを有効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1035">Indicates whether or not to enable Private Store Only.</span></span>|
|<span data-ttu-id="ad9c7-1036">storageRestrictAppDataToSystemVolume</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1036">storageRestrictAppDataToSystemVolume</span></span>|<span data-ttu-id="ad9c7-1037">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1037">Boolean</span></span>|<span data-ttu-id="ad9c7-1038">アプリケーションのデータがシステム ドライブに制限されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1038">Indicates whether application data is restricted to the system drive.</span></span>|
|<span data-ttu-id="ad9c7-1039">storageRestrictAppInstallToSystemVolume</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1039">storageRestrictAppInstallToSystemVolume</span></span>|<span data-ttu-id="ad9c7-1040">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1040">Boolean</span></span>|<span data-ttu-id="ad9c7-1041">アプリケーションのインストールがシステム ドライブに制限されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1041">Indicates whether the installation of applications is restricted to the system drive.</span></span>|
|<span data-ttu-id="ad9c7-1042">gameDvrBlocked</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1042">gameDvrBlocked</span></span>|<span data-ttu-id="ad9c7-1043">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1043">Boolean</span></span>|<span data-ttu-id="ad9c7-1044">DVR とブロードキャストを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1044">Indicates whether or not to block DVR and broadcasting.</span></span>|
|<span data-ttu-id="ad9c7-1045">experienceBlockDeviceDiscovery</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1045">experienceBlockDeviceDiscovery</span></span>|<span data-ttu-id="ad9c7-1046">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1046">Boolean</span></span>|<span data-ttu-id="ad9c7-1047">デバイス検出 UX を有効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1047">Indicates whether or not to enable device discovery UX.</span></span>|
|<span data-ttu-id="ad9c7-1048">experienceBlockErrorDialogWhenNoSIM</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1048">experienceBlockErrorDialogWhenNoSIM</span></span>|<span data-ttu-id="ad9c7-1049">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1049">Boolean</span></span>|<span data-ttu-id="ad9c7-1050">SIM カードが検出されない場合にエラー ダイアログを表示することを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1050">Indicates whether or not to allow the error dialog from displaying if no SIM card is detected.</span></span>|
|<span data-ttu-id="ad9c7-1051">experienceBlockTaskSwitcher</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1051">experienceBlockTaskSwitcher</span></span>|<span data-ttu-id="ad9c7-1052">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1052">Boolean</span></span>|<span data-ttu-id="ad9c7-1053">デバイスでのタスクの切り替えを有効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1053">Indicates whether or not to enable task switching on the device.</span></span>|
|<span data-ttu-id="ad9c7-1054">logonBlockFastUserSwitching</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1054">logonBlockFastUserSwitching</span></span>|<span data-ttu-id="ad9c7-1055">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1055">Boolean</span></span>|<span data-ttu-id="ad9c7-1056">同時にログオンしているユーザー間での切り替えをログオフなしで迅速に行う機能を無効にします。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1056">Disables the ability to quickly switch between users that are logged on simultaneously without logging off.</span></span>|
|<span data-ttu-id="ad9c7-1057">tenantLockdownRequireNetworkDuringOutOfBoxExperience</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1057">tenantLockdownRequireNetworkDuringOutOfBoxExperience</span></span>|<span data-ttu-id="ad9c7-1058">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1058">Boolean</span></span>|<span data-ttu-id="ad9c7-1059">ネットワークへの接続にデバイスが必要かどうか。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1059">Whether the device is required to connect to the network.</span></span>|
|<span data-ttu-id="ad9c7-1060">appManagementMSIAllowUserControlOverInstall</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1060">appManagementMSIAllowUserControlOverInstall</span></span>|<span data-ttu-id="ad9c7-1061">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1061">Boolean</span></span>|<span data-ttu-id="ad9c7-1062">このポリシー設定では、通常、システム管理者のみが使用できるインストールオプションをユーザーが変更することができます。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1062">This policy setting permits users to change installation options that typically are available only to system administrators.</span></span>|
|<span data-ttu-id="ad9c7-1063">appManagementMSIAlwaysInstallWithElevatedPrivileges</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1063">appManagementMSIAlwaysInstallWithElevatedPrivileges</span></span>|<span data-ttu-id="ad9c7-1064">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1064">Boolean</span></span>|<span data-ttu-id="ad9c7-1065">このポリシー設定は、システムにプログラムをインストールするときに、管理者特権でのアクセス許可を使用するように Windows インストーラーに指示します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1065">This policy setting directs Windows Installer to use elevated permissions when it installs any program on the system.</span></span>|
|<span data-ttu-id="ad9c7-1066">dataProtectionBlockDirectMemoryAccess</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1066">dataProtectionBlockDirectMemoryAccess</span></span>|<span data-ttu-id="ad9c7-1067">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1067">Boolean</span></span>|<span data-ttu-id="ad9c7-1068">このポリシー設定を使用すると、ユーザーが Windows にログインしない限り、ホットプラグ可能な PCI 下流ポートすべてのダイレクトメモリアクセス (DMA) をブロックすることができます。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1068">This policy setting allows you to block direct memory access (DMA) for all hot pluggable PCI downstream ports until a user logs into Windows.</span></span>|
|<span data-ttu-id="ad9c7-1069">appManagementPackageFamilyNamesToLaunchAfterLogOn</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1069">appManagementPackageFamilyNamesToLaunchAfterLogOn</span></span>|<span data-ttu-id="ad9c7-1070">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1070">String collection</span></span>|<span data-ttu-id="ad9c7-1071">Windows アプリの、セミコロンで区切られたパッケージファミリー名のリスト。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1071">List of semi-colon delimited Package Family Names of Windows apps.</span></span> <span data-ttu-id="ad9c7-1072">表示された Windows アプリは、ログオン後に起動されます。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1072">Listed Windows apps are to be launched after logon.</span></span>|



## <a name="response"></a><span data-ttu-id="ad9c7-1073">応答</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1073">Response</span></span>
<span data-ttu-id="ad9c7-1074">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1074">If successful, this method returns a `200 OK` response code and an updated [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad9c7-1075">例</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1075">Example</span></span>

### <a name="request"></a><span data-ttu-id="ad9c7-1076">要求</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1076">Request</span></span>
<span data-ttu-id="ad9c7-1077">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1077">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 14387

{
  "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
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
  "taskManagerBlockEndTask": true,
  "windows10AppsForceUpdateSchedule": {
    "@odata.type": "microsoft.graph.windows10AppsForceUpdateSchedule",
    "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
    "recurrence": "daily",
    "runImmediatelyIfAfterStartDateTime": true
  },
  "enableAutomaticRedeployment": true,
  "microsoftAccountSignInAssistantSettings": "disabled",
  "authenticationAllowSecondaryDevice": true,
  "authenticationWebSignIn": "enabled",
  "authenticationPreferredAzureADTenantDomainName": "Authentication Preferred Azure ADTenant Domain Name value",
  "cryptographyAllowFipsAlgorithmPolicy": true,
  "displayAppListWithGdiDPIScalingTurnedOn": [
    "Display App List With Gdi DPIScaling Turned On value"
  ],
  "displayAppListWithGdiDPIScalingTurnedOff": [
    "Display App List With Gdi DPIScaling Turned Off value"
  ],
  "enterpriseCloudPrintDiscoveryEndPoint": "Enterprise Cloud Print Discovery End Point value",
  "enterpriseCloudPrintOAuthAuthority": "Enterprise Cloud Print OAuth Authority value",
  "enterpriseCloudPrintOAuthClientIdentifier": "Enterprise Cloud Print OAuth Client Identifier value",
  "enterpriseCloudPrintResourceIdentifier": "Enterprise Cloud Print Resource Identifier value",
  "enterpriseCloudPrintDiscoveryMaxLimit": 5,
  "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "Enterprise Cloud Print Mopria Discovery Resource Identifier value",
  "experienceDoNotSyncBrowserSettings": "blockedWithUserOverride",
  "messagingBlockSync": true,
  "messagingBlockMMS": true,
  "messagingBlockRichCommunicationServices": true,
  "printerNames": [
    "Printer Names value"
  ],
  "printerDefaultName": "Printer Default Name value",
  "printerBlockAddition": true,
  "searchBlockDiacritics": true,
  "searchDisableAutoLanguageDetection": true,
  "searchDisableIndexingEncryptedItems": true,
  "searchEnableRemoteQueries": true,
  "searchDisableUseLocation": true,
  "searchDisableLocation": true,
  "searchDisableIndexerBackoff": true,
  "searchDisableIndexingRemovableDrive": true,
  "searchEnableAutomaticIndexSizeManangement": true,
  "searchBlockWebResults": true,
  "securityBlockAzureADJoinedDevicesAutoEncryption": true,
  "diagnosticsDataSubmissionMode": "none",
  "oneDriveDisableFileSync": true,
  "systemTelemetryProxyServer": "System Telemetry Proxy Server value",
  "edgeTelemetryForMicrosoft365Analytics": "intranet",
  "inkWorkspaceAccess": "enabled",
  "inkWorkspaceAccessState": "blocked",
  "inkWorkspaceBlockSuggestedApps": true,
  "smartScreenEnableAppInstallControl": true,
  "smartScreenAppInstallControl": "anywhere",
  "personalizationDesktopImageUrl": "https://example.com/personalizationDesktopImageUrl/",
  "personalizationLockScreenImageUrl": "https://example.com/personalizationLockScreenImageUrl/",
  "bluetoothAllowedServices": [
    "Bluetooth Allowed Services value"
  ],
  "bluetoothBlockAdvertising": true,
  "bluetoothBlockPromptedProximalConnections": true,
  "bluetoothBlockDiscoverableMode": true,
  "bluetoothBlockPrePairing": true,
  "edgeBlockAutofill": true,
  "edgeBlocked": true,
  "edgeCookiePolicy": "allow",
  "edgeBlockDeveloperTools": true,
  "edgeBlockSendingDoNotTrackHeader": true,
  "edgeBlockExtensions": true,
  "edgeBlockInPrivateBrowsing": true,
  "edgeBlockJavaScript": true,
  "edgeBlockPasswordManager": true,
  "edgeBlockAddressBarDropdown": true,
  "edgeBlockCompatibilityList": true,
  "edgeClearBrowsingDataOnExit": true,
  "edgeAllowStartPagesModification": true,
  "edgeDisableFirstRunPage": true,
  "edgeBlockLiveTileDataCollection": true,
  "edgeSyncFavoritesWithInternetExplorer": true,
  "edgeFavoritesListLocation": "Edge Favorites List Location value",
  "edgeBlockEditFavorites": true,
  "edgeNewTabPageURL": "Edge New Tab Page URL value",
  "edgeHomeButtonConfiguration": {
    "@odata.type": "microsoft.graph.edgeHomeButtonConfiguration"
  },
  "edgeHomeButtonConfigurationEnabled": true,
  "edgeOpensWith": "startPage",
  "edgeBlockSideloadingExtensions": true,
  "edgeRequiredExtensionPackageFamilyNames": [
    "Edge Required Extension Package Family Names value"
  ],
  "edgeBlockPrinting": true,
  "edgeFavoritesBarVisibility": "hide",
  "edgeBlockSavingHistory": true,
  "edgeBlockFullScreenMode": true,
  "edgeBlockWebContentOnNewTabPage": true,
  "edgeBlockTabPreloading": true,
  "edgeBlockPrelaunch": true,
  "edgeShowMessageWhenOpeningInternetExplorerSites": "disabled",
  "edgePreventCertificateErrorOverride": true,
  "edgeKioskModeRestriction": "digitalSignage",
  "edgeKioskResetAfterIdleTimeInMinutes": 4,
  "cellularBlockDataWhenRoaming": true,
  "cellularBlockVpn": true,
  "cellularBlockVpnWhenRoaming": true,
  "cellularData": "required",
  "defenderBlockEndUserAccess": true,
  "defenderDaysBeforeDeletingQuarantinedMalware": 12,
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "clean",
    "moderateSeverity": "clean",
    "highSeverity": "clean",
    "severeSeverity": "clean"
  },
  "defenderSystemScanSchedule": "everyday",
  "defenderFilesAndFoldersToExclude": [
    "Defender Files And Folders To Exclude value"
  ],
  "defenderFileExtensionsToExclude": [
    "Defender File Extensions To Exclude value"
  ],
  "defenderScanMaxCpu": 2,
  "defenderMonitorFileActivity": "disable",
  "defenderPotentiallyUnwantedAppAction": "block",
  "defenderPotentiallyUnwantedAppActionSetting": "enable",
  "defenderProcessesToExclude": [
    "Defender Processes To Exclude value"
  ],
  "defenderPromptForSampleSubmission": "alwaysPrompt",
  "defenderRequireBehaviorMonitoring": true,
  "defenderRequireCloudProtection": true,
  "defenderRequireNetworkInspectionSystem": true,
  "defenderRequireRealTimeMonitoring": true,
  "defenderScanArchiveFiles": true,
  "defenderScanDownloads": true,
  "defenderScheduleScanEnableLowCpuPriority": true,
  "defenderDisableCatchupQuickScan": true,
  "defenderDisableCatchupFullScan": true,
  "defenderScanNetworkFiles": true,
  "defenderScanIncomingMail": true,
  "defenderScanMappedNetworkDrivesDuringFullScan": true,
  "defenderScanRemovableDrivesDuringFullScan": true,
  "defenderScanScriptsLoadedInInternetExplorer": true,
  "defenderSignatureUpdateIntervalInHours": 6,
  "defenderScanType": "disabled",
  "defenderScheduledScanTime": "11:59:10.9990000",
  "defenderScheduledQuickScanTime": "11:58:49.3840000",
  "defenderCloudBlockLevel": "high",
  "defenderCloudExtendedTimeout": 12,
  "defenderCloudExtendedTimeoutInSeconds": 5,
  "defenderBlockOnAccessProtection": true,
  "defenderSubmitSamplesConsentType": "alwaysPrompt",
  "lockScreenAllowTimeoutConfiguration": true,
  "lockScreenBlockActionCenterNotifications": true,
  "lockScreenBlockCortana": true,
  "lockScreenBlockToastNotifications": true,
  "lockScreenTimeoutInSeconds": 10,
  "lockScreenActivateAppsWithVoice": "enabled",
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "passwordRequireWhenResumeFromIdleState": true,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordMinimumAgeInDays": 8,
  "privacyAdvertisingId": "blocked",
  "privacyAutoAcceptPairingAndConsentPrompts": true,
  "privacyDisableLaunchExperience": true,
  "privacyBlockInputPersonalization": true,
  "privacyBlockPublishUserActivities": true,
  "privacyBlockActivityFeed": true,
  "startBlockUnpinningAppsFromTaskbar": true,
  "startMenuAppListVisibility": "collapse",
  "startMenuHideChangeAccountSettings": true,
  "startMenuHideFrequentlyUsedApps": true,
  "startMenuHideHibernate": true,
  "startMenuHideLock": true,
  "startMenuHidePowerButton": true,
  "startMenuHideRecentJumpLists": true,
  "startMenuHideRecentlyAddedApps": true,
  "startMenuHideRestartOptions": true,
  "startMenuHideShutDown": true,
  "startMenuHideSignOut": true,
  "startMenuHideSleep": true,
  "startMenuHideSwitchAccount": true,
  "startMenuHideUserTile": true,
  "startMenuLayoutEdgeAssetsXml": "c3RhcnRNZW51TGF5b3V0RWRnZUFzc2V0c1htbA==",
  "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s",
  "startMenuMode": "fullScreen",
  "startMenuPinnedFolderDocuments": "hide",
  "startMenuPinnedFolderDownloads": "hide",
  "startMenuPinnedFolderFileExplorer": "hide",
  "startMenuPinnedFolderHomeGroup": "hide",
  "startMenuPinnedFolderMusic": "hide",
  "startMenuPinnedFolderNetwork": "hide",
  "startMenuPinnedFolderPersonalFolder": "hide",
  "startMenuPinnedFolderPictures": "hide",
  "startMenuPinnedFolderSettings": "hide",
  "startMenuPinnedFolderVideos": "hide",
  "settingsBlockSettingsApp": true,
  "settingsBlockSystemPage": true,
  "settingsBlockDevicesPage": true,
  "settingsBlockNetworkInternetPage": true,
  "settingsBlockPersonalizationPage": true,
  "settingsBlockAccountsPage": true,
  "settingsBlockTimeLanguagePage": true,
  "settingsBlockEaseOfAccessPage": true,
  "settingsBlockPrivacyPage": true,
  "settingsBlockUpdateSecurityPage": true,
  "settingsBlockAppsPage": true,
  "settingsBlockGamingPage": true,
  "windowsSpotlightBlockConsumerSpecificFeatures": true,
  "windowsSpotlightBlocked": true,
  "windowsSpotlightBlockOnActionCenter": true,
  "windowsSpotlightBlockTailoredExperiences": true,
  "windowsSpotlightBlockThirdPartyNotifications": true,
  "windowsSpotlightBlockWelcomeExperience": true,
  "windowsSpotlightBlockWindowsTips": true,
  "windowsSpotlightConfigureOnLockScreen": "disabled",
  "networkProxyApplySettingsDeviceWide": true,
  "networkProxyDisableAutoDetect": true,
  "networkProxyAutomaticConfigurationUrl": "https://example.com/networkProxyAutomaticConfigurationUrl/",
  "networkProxyServer": {
    "@odata.type": "microsoft.graph.windows10NetworkProxyServer",
    "address": "Address value",
    "exceptions": [
      "Exceptions value"
    ],
    "useForLocalAddresses": true
  },
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "antiTheftModeBlocked": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "connectedDevicesServiceBlocked": true,
  "certificatesBlockManualRootCertificateInstallation": true,
  "copyPasteBlocked": true,
  "cortanaBlocked": true,
  "deviceManagementBlockFactoryResetOnMobile": true,
  "deviceManagementBlockManualUnenroll": true,
  "safeSearchFilter": "strict",
  "edgeBlockPopups": true,
  "edgeBlockSearchSuggestions": true,
  "edgeBlockSearchEngineCustomization": true,
  "edgeBlockSendingIntranetTrafficToInternetExplorer": true,
  "edgeSendIntranetTrafficToInternetExplorer": true,
  "edgeRequireSmartScreen": true,
  "edgeEnterpriseModeSiteListLocation": "Edge Enterprise Mode Site List Location value",
  "edgeFirstRunUrl": "https://example.com/edgeFirstRunUrl/",
  "edgeSearchEngine": {
    "@odata.type": "microsoft.graph.edgeSearchEngineBase"
  },
  "edgeHomepageUrls": [
    "Edge Homepage Urls value"
  ],
  "edgeBlockAccessToAboutFlags": true,
  "smartScreenBlockPromptOverride": true,
  "smartScreenBlockPromptOverrideForFiles": true,
  "webRtcBlockLocalhostIpAddress": true,
  "internetSharingBlocked": true,
  "settingsBlockAddProvisioningPackage": true,
  "settingsBlockRemoveProvisioningPackage": true,
  "settingsBlockChangeSystemTime": true,
  "settingsBlockEditDeviceName": true,
  "settingsBlockChangeRegion": true,
  "settingsBlockChangeLanguage": true,
  "settingsBlockChangePowerSleep": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "microsoftAccountBlockSettingsSync": true,
  "nfcBlocked": true,
  "resetProtectionModeBlocked": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireMobileDeviceEncryption": true,
  "usbBlocked": true,
  "voiceRecordingBlocked": true,
  "wiFiBlockAutomaticConnectHotspots": true,
  "wiFiBlocked": true,
  "wiFiBlockManualConfiguration": true,
  "wiFiScanInterval": 0,
  "wirelessDisplayBlockProjectionToThisDevice": true,
  "wirelessDisplayBlockUserInputFromReceiver": true,
  "wirelessDisplayRequirePinForPairing": true,
  "windowsStoreBlocked": true,
  "appsAllowTrustedAppsSideloading": "blocked",
  "windowsStoreBlockAutoUpdate": true,
  "developerUnlockSetting": "blocked",
  "sharedUserAppDataAllowed": true,
  "appsBlockWindowsStoreOriginatedApps": true,
  "windowsStoreEnablePrivateStoreOnly": true,
  "storageRestrictAppDataToSystemVolume": true,
  "storageRestrictAppInstallToSystemVolume": true,
  "gameDvrBlocked": true,
  "experienceBlockDeviceDiscovery": true,
  "experienceBlockErrorDialogWhenNoSIM": true,
  "experienceBlockTaskSwitcher": true,
  "logonBlockFastUserSwitching": true,
  "tenantLockdownRequireNetworkDuringOutOfBoxExperience": true,
  "appManagementMSIAllowUserControlOverInstall": true,
  "appManagementMSIAlwaysInstallWithElevatedPrivileges": true,
  "dataProtectionBlockDirectMemoryAccess": true,
  "appManagementPackageFamilyNamesToLaunchAfterLogOn": [
    "App Management Package Family Names To Launch After Log On value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="ad9c7-1078">応答</span><span class="sxs-lookup"><span data-stu-id="ad9c7-1078">Response</span></span>
<span data-ttu-id="ad9c7-p186">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ad9c7-p186">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 14559

{
  "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
  "id": "a4235d71-5d71-a423-715d-23a4715d23a4",
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
  "taskManagerBlockEndTask": true,
  "windows10AppsForceUpdateSchedule": {
    "@odata.type": "microsoft.graph.windows10AppsForceUpdateSchedule",
    "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
    "recurrence": "daily",
    "runImmediatelyIfAfterStartDateTime": true
  },
  "enableAutomaticRedeployment": true,
  "microsoftAccountSignInAssistantSettings": "disabled",
  "authenticationAllowSecondaryDevice": true,
  "authenticationWebSignIn": "enabled",
  "authenticationPreferredAzureADTenantDomainName": "Authentication Preferred Azure ADTenant Domain Name value",
  "cryptographyAllowFipsAlgorithmPolicy": true,
  "displayAppListWithGdiDPIScalingTurnedOn": [
    "Display App List With Gdi DPIScaling Turned On value"
  ],
  "displayAppListWithGdiDPIScalingTurnedOff": [
    "Display App List With Gdi DPIScaling Turned Off value"
  ],
  "enterpriseCloudPrintDiscoveryEndPoint": "Enterprise Cloud Print Discovery End Point value",
  "enterpriseCloudPrintOAuthAuthority": "Enterprise Cloud Print OAuth Authority value",
  "enterpriseCloudPrintOAuthClientIdentifier": "Enterprise Cloud Print OAuth Client Identifier value",
  "enterpriseCloudPrintResourceIdentifier": "Enterprise Cloud Print Resource Identifier value",
  "enterpriseCloudPrintDiscoveryMaxLimit": 5,
  "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "Enterprise Cloud Print Mopria Discovery Resource Identifier value",
  "experienceDoNotSyncBrowserSettings": "blockedWithUserOverride",
  "messagingBlockSync": true,
  "messagingBlockMMS": true,
  "messagingBlockRichCommunicationServices": true,
  "printerNames": [
    "Printer Names value"
  ],
  "printerDefaultName": "Printer Default Name value",
  "printerBlockAddition": true,
  "searchBlockDiacritics": true,
  "searchDisableAutoLanguageDetection": true,
  "searchDisableIndexingEncryptedItems": true,
  "searchEnableRemoteQueries": true,
  "searchDisableUseLocation": true,
  "searchDisableLocation": true,
  "searchDisableIndexerBackoff": true,
  "searchDisableIndexingRemovableDrive": true,
  "searchEnableAutomaticIndexSizeManangement": true,
  "searchBlockWebResults": true,
  "securityBlockAzureADJoinedDevicesAutoEncryption": true,
  "diagnosticsDataSubmissionMode": "none",
  "oneDriveDisableFileSync": true,
  "systemTelemetryProxyServer": "System Telemetry Proxy Server value",
  "edgeTelemetryForMicrosoft365Analytics": "intranet",
  "inkWorkspaceAccess": "enabled",
  "inkWorkspaceAccessState": "blocked",
  "inkWorkspaceBlockSuggestedApps": true,
  "smartScreenEnableAppInstallControl": true,
  "smartScreenAppInstallControl": "anywhere",
  "personalizationDesktopImageUrl": "https://example.com/personalizationDesktopImageUrl/",
  "personalizationLockScreenImageUrl": "https://example.com/personalizationLockScreenImageUrl/",
  "bluetoothAllowedServices": [
    "Bluetooth Allowed Services value"
  ],
  "bluetoothBlockAdvertising": true,
  "bluetoothBlockPromptedProximalConnections": true,
  "bluetoothBlockDiscoverableMode": true,
  "bluetoothBlockPrePairing": true,
  "edgeBlockAutofill": true,
  "edgeBlocked": true,
  "edgeCookiePolicy": "allow",
  "edgeBlockDeveloperTools": true,
  "edgeBlockSendingDoNotTrackHeader": true,
  "edgeBlockExtensions": true,
  "edgeBlockInPrivateBrowsing": true,
  "edgeBlockJavaScript": true,
  "edgeBlockPasswordManager": true,
  "edgeBlockAddressBarDropdown": true,
  "edgeBlockCompatibilityList": true,
  "edgeClearBrowsingDataOnExit": true,
  "edgeAllowStartPagesModification": true,
  "edgeDisableFirstRunPage": true,
  "edgeBlockLiveTileDataCollection": true,
  "edgeSyncFavoritesWithInternetExplorer": true,
  "edgeFavoritesListLocation": "Edge Favorites List Location value",
  "edgeBlockEditFavorites": true,
  "edgeNewTabPageURL": "Edge New Tab Page URL value",
  "edgeHomeButtonConfiguration": {
    "@odata.type": "microsoft.graph.edgeHomeButtonConfiguration"
  },
  "edgeHomeButtonConfigurationEnabled": true,
  "edgeOpensWith": "startPage",
  "edgeBlockSideloadingExtensions": true,
  "edgeRequiredExtensionPackageFamilyNames": [
    "Edge Required Extension Package Family Names value"
  ],
  "edgeBlockPrinting": true,
  "edgeFavoritesBarVisibility": "hide",
  "edgeBlockSavingHistory": true,
  "edgeBlockFullScreenMode": true,
  "edgeBlockWebContentOnNewTabPage": true,
  "edgeBlockTabPreloading": true,
  "edgeBlockPrelaunch": true,
  "edgeShowMessageWhenOpeningInternetExplorerSites": "disabled",
  "edgePreventCertificateErrorOverride": true,
  "edgeKioskModeRestriction": "digitalSignage",
  "edgeKioskResetAfterIdleTimeInMinutes": 4,
  "cellularBlockDataWhenRoaming": true,
  "cellularBlockVpn": true,
  "cellularBlockVpnWhenRoaming": true,
  "cellularData": "required",
  "defenderBlockEndUserAccess": true,
  "defenderDaysBeforeDeletingQuarantinedMalware": 12,
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "clean",
    "moderateSeverity": "clean",
    "highSeverity": "clean",
    "severeSeverity": "clean"
  },
  "defenderSystemScanSchedule": "everyday",
  "defenderFilesAndFoldersToExclude": [
    "Defender Files And Folders To Exclude value"
  ],
  "defenderFileExtensionsToExclude": [
    "Defender File Extensions To Exclude value"
  ],
  "defenderScanMaxCpu": 2,
  "defenderMonitorFileActivity": "disable",
  "defenderPotentiallyUnwantedAppAction": "block",
  "defenderPotentiallyUnwantedAppActionSetting": "enable",
  "defenderProcessesToExclude": [
    "Defender Processes To Exclude value"
  ],
  "defenderPromptForSampleSubmission": "alwaysPrompt",
  "defenderRequireBehaviorMonitoring": true,
  "defenderRequireCloudProtection": true,
  "defenderRequireNetworkInspectionSystem": true,
  "defenderRequireRealTimeMonitoring": true,
  "defenderScanArchiveFiles": true,
  "defenderScanDownloads": true,
  "defenderScheduleScanEnableLowCpuPriority": true,
  "defenderDisableCatchupQuickScan": true,
  "defenderDisableCatchupFullScan": true,
  "defenderScanNetworkFiles": true,
  "defenderScanIncomingMail": true,
  "defenderScanMappedNetworkDrivesDuringFullScan": true,
  "defenderScanRemovableDrivesDuringFullScan": true,
  "defenderScanScriptsLoadedInInternetExplorer": true,
  "defenderSignatureUpdateIntervalInHours": 6,
  "defenderScanType": "disabled",
  "defenderScheduledScanTime": "11:59:10.9990000",
  "defenderScheduledQuickScanTime": "11:58:49.3840000",
  "defenderCloudBlockLevel": "high",
  "defenderCloudExtendedTimeout": 12,
  "defenderCloudExtendedTimeoutInSeconds": 5,
  "defenderBlockOnAccessProtection": true,
  "defenderSubmitSamplesConsentType": "alwaysPrompt",
  "lockScreenAllowTimeoutConfiguration": true,
  "lockScreenBlockActionCenterNotifications": true,
  "lockScreenBlockCortana": true,
  "lockScreenBlockToastNotifications": true,
  "lockScreenTimeoutInSeconds": 10,
  "lockScreenActivateAppsWithVoice": "enabled",
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "passwordRequireWhenResumeFromIdleState": true,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordMinimumAgeInDays": 8,
  "privacyAdvertisingId": "blocked",
  "privacyAutoAcceptPairingAndConsentPrompts": true,
  "privacyDisableLaunchExperience": true,
  "privacyBlockInputPersonalization": true,
  "privacyBlockPublishUserActivities": true,
  "privacyBlockActivityFeed": true,
  "startBlockUnpinningAppsFromTaskbar": true,
  "startMenuAppListVisibility": "collapse",
  "startMenuHideChangeAccountSettings": true,
  "startMenuHideFrequentlyUsedApps": true,
  "startMenuHideHibernate": true,
  "startMenuHideLock": true,
  "startMenuHidePowerButton": true,
  "startMenuHideRecentJumpLists": true,
  "startMenuHideRecentlyAddedApps": true,
  "startMenuHideRestartOptions": true,
  "startMenuHideShutDown": true,
  "startMenuHideSignOut": true,
  "startMenuHideSleep": true,
  "startMenuHideSwitchAccount": true,
  "startMenuHideUserTile": true,
  "startMenuLayoutEdgeAssetsXml": "c3RhcnRNZW51TGF5b3V0RWRnZUFzc2V0c1htbA==",
  "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s",
  "startMenuMode": "fullScreen",
  "startMenuPinnedFolderDocuments": "hide",
  "startMenuPinnedFolderDownloads": "hide",
  "startMenuPinnedFolderFileExplorer": "hide",
  "startMenuPinnedFolderHomeGroup": "hide",
  "startMenuPinnedFolderMusic": "hide",
  "startMenuPinnedFolderNetwork": "hide",
  "startMenuPinnedFolderPersonalFolder": "hide",
  "startMenuPinnedFolderPictures": "hide",
  "startMenuPinnedFolderSettings": "hide",
  "startMenuPinnedFolderVideos": "hide",
  "settingsBlockSettingsApp": true,
  "settingsBlockSystemPage": true,
  "settingsBlockDevicesPage": true,
  "settingsBlockNetworkInternetPage": true,
  "settingsBlockPersonalizationPage": true,
  "settingsBlockAccountsPage": true,
  "settingsBlockTimeLanguagePage": true,
  "settingsBlockEaseOfAccessPage": true,
  "settingsBlockPrivacyPage": true,
  "settingsBlockUpdateSecurityPage": true,
  "settingsBlockAppsPage": true,
  "settingsBlockGamingPage": true,
  "windowsSpotlightBlockConsumerSpecificFeatures": true,
  "windowsSpotlightBlocked": true,
  "windowsSpotlightBlockOnActionCenter": true,
  "windowsSpotlightBlockTailoredExperiences": true,
  "windowsSpotlightBlockThirdPartyNotifications": true,
  "windowsSpotlightBlockWelcomeExperience": true,
  "windowsSpotlightBlockWindowsTips": true,
  "windowsSpotlightConfigureOnLockScreen": "disabled",
  "networkProxyApplySettingsDeviceWide": true,
  "networkProxyDisableAutoDetect": true,
  "networkProxyAutomaticConfigurationUrl": "https://example.com/networkProxyAutomaticConfigurationUrl/",
  "networkProxyServer": {
    "@odata.type": "microsoft.graph.windows10NetworkProxyServer",
    "address": "Address value",
    "exceptions": [
      "Exceptions value"
    ],
    "useForLocalAddresses": true
  },
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "antiTheftModeBlocked": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "connectedDevicesServiceBlocked": true,
  "certificatesBlockManualRootCertificateInstallation": true,
  "copyPasteBlocked": true,
  "cortanaBlocked": true,
  "deviceManagementBlockFactoryResetOnMobile": true,
  "deviceManagementBlockManualUnenroll": true,
  "safeSearchFilter": "strict",
  "edgeBlockPopups": true,
  "edgeBlockSearchSuggestions": true,
  "edgeBlockSearchEngineCustomization": true,
  "edgeBlockSendingIntranetTrafficToInternetExplorer": true,
  "edgeSendIntranetTrafficToInternetExplorer": true,
  "edgeRequireSmartScreen": true,
  "edgeEnterpriseModeSiteListLocation": "Edge Enterprise Mode Site List Location value",
  "edgeFirstRunUrl": "https://example.com/edgeFirstRunUrl/",
  "edgeSearchEngine": {
    "@odata.type": "microsoft.graph.edgeSearchEngineBase"
  },
  "edgeHomepageUrls": [
    "Edge Homepage Urls value"
  ],
  "edgeBlockAccessToAboutFlags": true,
  "smartScreenBlockPromptOverride": true,
  "smartScreenBlockPromptOverrideForFiles": true,
  "webRtcBlockLocalhostIpAddress": true,
  "internetSharingBlocked": true,
  "settingsBlockAddProvisioningPackage": true,
  "settingsBlockRemoveProvisioningPackage": true,
  "settingsBlockChangeSystemTime": true,
  "settingsBlockEditDeviceName": true,
  "settingsBlockChangeRegion": true,
  "settingsBlockChangeLanguage": true,
  "settingsBlockChangePowerSleep": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "microsoftAccountBlockSettingsSync": true,
  "nfcBlocked": true,
  "resetProtectionModeBlocked": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireMobileDeviceEncryption": true,
  "usbBlocked": true,
  "voiceRecordingBlocked": true,
  "wiFiBlockAutomaticConnectHotspots": true,
  "wiFiBlocked": true,
  "wiFiBlockManualConfiguration": true,
  "wiFiScanInterval": 0,
  "wirelessDisplayBlockProjectionToThisDevice": true,
  "wirelessDisplayBlockUserInputFromReceiver": true,
  "wirelessDisplayRequirePinForPairing": true,
  "windowsStoreBlocked": true,
  "appsAllowTrustedAppsSideloading": "blocked",
  "windowsStoreBlockAutoUpdate": true,
  "developerUnlockSetting": "blocked",
  "sharedUserAppDataAllowed": true,
  "appsBlockWindowsStoreOriginatedApps": true,
  "windowsStoreEnablePrivateStoreOnly": true,
  "storageRestrictAppDataToSystemVolume": true,
  "storageRestrictAppInstallToSystemVolume": true,
  "gameDvrBlocked": true,
  "experienceBlockDeviceDiscovery": true,
  "experienceBlockErrorDialogWhenNoSIM": true,
  "experienceBlockTaskSwitcher": true,
  "logonBlockFastUserSwitching": true,
  "tenantLockdownRequireNetworkDuringOutOfBoxExperience": true,
  "appManagementMSIAllowUserControlOverInstall": true,
  "appManagementMSIAlwaysInstallWithElevatedPrivileges": true,
  "dataProtectionBlockDirectMemoryAccess": true,
  "appManagementPackageFamilyNamesToLaunchAfterLogOn": [
    "App Management Package Family Names To Launch After Log On value"
  ]
}
```





