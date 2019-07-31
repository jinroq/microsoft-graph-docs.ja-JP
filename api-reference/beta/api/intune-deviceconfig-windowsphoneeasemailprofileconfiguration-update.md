---
title: WindowsPhoneEASEmailProfileConfiguration の更新
description: WindowsPhoneEASEmailProfileConfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 54ad7ac159a47e4f3eb112e1184dda3d02cc8b79
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35982068"
---
# <a name="update-windowsphoneeasemailprofileconfiguration"></a><span data-ttu-id="3cbe6-103">WindowsPhoneEASEmailProfileConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="3cbe6-103">Update windowsPhoneEASEmailProfileConfiguration</span></span>

> <span data-ttu-id="3cbe6-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3cbe6-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3cbe6-106">[Windowsphoneeasemailprofileconfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-106">Update the properties of a [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3cbe6-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="3cbe6-107">Prerequisites</span></span>
<span data-ttu-id="3cbe6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cbe6-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3cbe6-110">Permission type</span></span>|<span data-ttu-id="3cbe6-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3cbe6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3cbe6-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3cbe6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3cbe6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cbe6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3cbe6-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3cbe6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3cbe6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-115">Not supported.</span></span>|
|<span data-ttu-id="3cbe6-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3cbe6-116">Application</span></span>|<span data-ttu-id="3cbe6-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3cbe6-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3cbe6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3cbe6-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3cbe6-119">Request headers</span></span>
|<span data-ttu-id="3cbe6-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3cbe6-120">Header</span></span>|<span data-ttu-id="3cbe6-121">値</span><span class="sxs-lookup"><span data-stu-id="3cbe6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3cbe6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3cbe6-122">Authorization</span></span>|<span data-ttu-id="3cbe6-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3cbe6-124">承諾</span><span class="sxs-lookup"><span data-stu-id="3cbe6-124">Accept</span></span>|<span data-ttu-id="3cbe6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3cbe6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3cbe6-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="3cbe6-126">Request body</span></span>
<span data-ttu-id="3cbe6-127">要求本文で、 [Windowsphoneeasemailprofileconfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-127">In the request body, supply a JSON representation for the [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="3cbe6-128">次の表に、 [Windowsphoneeasemailprofileconfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-128">The following table shows the properties that are required when you create the [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="3cbe6-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3cbe6-129">Property</span></span>|<span data-ttu-id="3cbe6-130">型</span><span class="sxs-lookup"><span data-stu-id="3cbe6-130">Type</span></span>|<span data-ttu-id="3cbe6-131">説明</span><span class="sxs-lookup"><span data-stu-id="3cbe6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cbe6-132">id</span><span class="sxs-lookup"><span data-stu-id="3cbe6-132">id</span></span>|<span data-ttu-id="3cbe6-133">文字列</span><span class="sxs-lookup"><span data-stu-id="3cbe6-133">String</span></span>|<span data-ttu-id="3cbe6-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-134">Key of the entity.</span></span> <span data-ttu-id="3cbe6-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3cbe6-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3cbe6-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3cbe6-136">lastModifiedDateTime</span></span>|<span data-ttu-id="3cbe6-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3cbe6-137">DateTimeOffset</span></span>|<span data-ttu-id="3cbe6-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-138">DateTime the object was last modified.</span></span> <span data-ttu-id="3cbe6-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3cbe6-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3cbe6-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3cbe6-140">roleScopeTagIds</span></span>|<span data-ttu-id="3cbe6-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="3cbe6-141">String collection</span></span>|<span data-ttu-id="3cbe6-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3cbe6-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3cbe6-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3cbe6-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3cbe6-144">supportsScopeTags</span></span>|<span data-ttu-id="3cbe6-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cbe6-145">Boolean</span></span>|<span data-ttu-id="3cbe6-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3cbe6-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3cbe6-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3cbe6-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-149">This property is read-only.</span></span> <span data-ttu-id="3cbe6-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3cbe6-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3cbe6-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3cbe6-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="3cbe6-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3cbe6-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="3cbe6-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="3cbe6-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3cbe6-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3cbe6-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3cbe6-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="3cbe6-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3cbe6-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="3cbe6-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="3cbe6-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3cbe6-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3cbe6-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="3cbe6-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="3cbe6-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="3cbe6-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="3cbe6-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="3cbe6-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3cbe6-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3cbe6-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3cbe6-163">createdDateTime</span></span>|<span data-ttu-id="3cbe6-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3cbe6-164">DateTimeOffset</span></span>|<span data-ttu-id="3cbe6-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-165">DateTime the object was created.</span></span> <span data-ttu-id="3cbe6-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3cbe6-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3cbe6-167">description</span><span class="sxs-lookup"><span data-stu-id="3cbe6-167">description</span></span>|<span data-ttu-id="3cbe6-168">String</span><span class="sxs-lookup"><span data-stu-id="3cbe6-168">String</span></span>|<span data-ttu-id="3cbe6-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3cbe6-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3cbe6-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3cbe6-171">displayName</span><span class="sxs-lookup"><span data-stu-id="3cbe6-171">displayName</span></span>|<span data-ttu-id="3cbe6-172">String</span><span class="sxs-lookup"><span data-stu-id="3cbe6-172">String</span></span>|<span data-ttu-id="3cbe6-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3cbe6-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3cbe6-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3cbe6-175">version</span><span class="sxs-lookup"><span data-stu-id="3cbe6-175">version</span></span>|<span data-ttu-id="3cbe6-176">Int32</span><span class="sxs-lookup"><span data-stu-id="3cbe6-176">Int32</span></span>|<span data-ttu-id="3cbe6-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-177">Version of the device configuration.</span></span> <span data-ttu-id="3cbe6-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3cbe6-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3cbe6-179">usernameSource</span><span class="sxs-lookup"><span data-stu-id="3cbe6-179">usernameSource</span></span>|[<span data-ttu-id="3cbe6-180">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="3cbe6-180">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="3cbe6-181">ユーザー名属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-181">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="3cbe6-182">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-182">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="3cbe6-183">可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-183">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="3cbe6-184">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="3cbe6-184">usernameAADSource</span></span>|[<span data-ttu-id="3cbe6-185">usernameSource</span><span class="sxs-lookup"><span data-stu-id="3cbe6-185">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="3cbe6-186">メールプロファイルのユーザー名を取得するために使用される AAD フィールドの名前。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-186">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="3cbe6-187">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-187">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="3cbe6-188">可能な値は、`userPrincipalName`、`primarySmtpAddress`、`samAccountName` です。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-188">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="3cbe6-189">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="3cbe6-189">userDomainNameSource</span></span>|[<span data-ttu-id="3cbe6-190">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="3cbe6-190">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="3cbe6-191">UserDomainname 属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-191">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="3cbe6-192">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-192">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="3cbe6-193">可能な値は、`fullDomainName`、`netBiosDomainName` です。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-193">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="3cbe6-194">customDomainName</span><span class="sxs-lookup"><span data-stu-id="3cbe6-194">customDomainName</span></span>|<span data-ttu-id="3cbe6-195">String</span><span class="sxs-lookup"><span data-stu-id="3cbe6-195">String</span></span>|<span data-ttu-id="3cbe6-196">デバイスにインストールする前に電子メールプロファイルを生成するときに使用するカスタムドメイン名の値。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-196">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="3cbe6-197">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-197">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="3cbe6-198">accountName</span><span class="sxs-lookup"><span data-stu-id="3cbe6-198">accountName</span></span>|<span data-ttu-id="3cbe6-199">String</span><span class="sxs-lookup"><span data-stu-id="3cbe6-199">String</span></span>|<span data-ttu-id="3cbe6-200">アカウント名。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-200">Account name.</span></span>|
|<span data-ttu-id="3cbe6-201">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="3cbe6-201">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="3cbe6-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cbe6-202">Boolean</span></span>|<span data-ttu-id="3cbe6-203">このポリシーを Windows 8.1 にのみ適用するかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-203">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="3cbe6-204">このプロパティは読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-204">This property is read-only.</span></span>|
|<span data-ttu-id="3cbe6-205">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="3cbe6-205">syncCalendar</span></span>|<span data-ttu-id="3cbe6-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cbe6-206">Boolean</span></span>|<span data-ttu-id="3cbe6-207">予定表を同期するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-207">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="3cbe6-208">syncContacts</span><span class="sxs-lookup"><span data-stu-id="3cbe6-208">syncContacts</span></span>|<span data-ttu-id="3cbe6-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cbe6-209">Boolean</span></span>|<span data-ttu-id="3cbe6-210">連絡先を同期するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-210">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="3cbe6-211">syncTasks</span><span class="sxs-lookup"><span data-stu-id="3cbe6-211">syncTasks</span></span>|<span data-ttu-id="3cbe6-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cbe6-212">Boolean</span></span>|<span data-ttu-id="3cbe6-213">タスクを同期するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-213">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="3cbe6-214">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="3cbe6-214">durationOfEmailToSync</span></span>|[<span data-ttu-id="3cbe6-215">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="3cbe6-215">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="3cbe6-216">同期する電子メールの期間。可能な値は`userDefined`、 `oneDay`、 `threeDays` `oneWeek` `twoWeeks` `oneMonth`、、、、 `unlimited`、です。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-216">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="3cbe6-217">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="3cbe6-217">emailAddressSource</span></span>|[<span data-ttu-id="3cbe6-218">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="3cbe6-218">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="3cbe6-219">AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入される電子メール属性。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-219">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="3cbe6-220">可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-220">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="3cbe6-221">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="3cbe6-221">emailSyncSchedule</span></span>|[<span data-ttu-id="3cbe6-222">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="3cbe6-222">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="3cbe6-223">電子メール同期スケジュール。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-223">Email sync schedule.</span></span> <span data-ttu-id="3cbe6-224">可能な値は、`userDefined`、`asMessagesArrive`、`manual`、`fifteenMinutes`、`thirtyMinutes`、`sixtyMinutes`、`basedOnMyUsage` です。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-224">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="3cbe6-225">hostName</span><span class="sxs-lookup"><span data-stu-id="3cbe6-225">hostName</span></span>|<span data-ttu-id="3cbe6-226">String</span><span class="sxs-lookup"><span data-stu-id="3cbe6-226">String</span></span>|<span data-ttu-id="3cbe6-227">ネイティブメールアプリが接続する Exchange の場所 (URL)。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-227">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="3cbe6-228">requireSsl</span><span class="sxs-lookup"><span data-stu-id="3cbe6-228">requireSsl</span></span>|<span data-ttu-id="3cbe6-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cbe6-229">Boolean</span></span>|<span data-ttu-id="3cbe6-230">SSL を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-230">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="3cbe6-231">応答</span><span class="sxs-lookup"><span data-stu-id="3cbe6-231">Response</span></span>
<span data-ttu-id="3cbe6-232">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[Windowsphoneeasemailprofileconfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-232">If successful, this method returns a `200 OK` response code and an updated [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3cbe6-233">例</span><span class="sxs-lookup"><span data-stu-id="3cbe6-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="3cbe6-234">要求</span><span class="sxs-lookup"><span data-stu-id="3cbe6-234">Request</span></span>
<span data-ttu-id="3cbe6-235">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-235">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1567

{
  "@odata.type": "#microsoft.graph.windowsPhoneEASEmailProfileConfiguration",
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
  "usernameSource": "primarySmtpAddress",
  "usernameAADSource": "primarySmtpAddress",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value",
  "accountName": "Account Name value",
  "applyOnlyToWindowsPhone81": true,
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "emailSyncSchedule": "asMessagesArrive",
  "hostName": "Host Name value",
  "requireSsl": true
}
```

### <a name="response"></a><span data-ttu-id="3cbe6-236">応答</span><span class="sxs-lookup"><span data-stu-id="3cbe6-236">Response</span></span>
<span data-ttu-id="3cbe6-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3cbe6-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1739

{
  "@odata.type": "#microsoft.graph.windowsPhoneEASEmailProfileConfiguration",
  "id": "554f402a-402a-554f-2a40-4f552a404f55",
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
  "usernameSource": "primarySmtpAddress",
  "usernameAADSource": "primarySmtpAddress",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value",
  "accountName": "Account Name value",
  "applyOnlyToWindowsPhone81": true,
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "emailSyncSchedule": "asMessagesArrive",
  "hostName": "Host Name value",
  "requireSsl": true
}
```





