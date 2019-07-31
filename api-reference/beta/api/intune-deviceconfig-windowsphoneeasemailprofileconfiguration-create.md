---
title: WindowsPhoneEASEmailProfileConfiguration の作成
description: 新しい windowsPhoneEASEmailProfileConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c85ea38a4d0d52bbb4d3a56c8ab4fa097b9d24cb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35986436"
---
# <a name="create-windowsphoneeasemailprofileconfiguration"></a><span data-ttu-id="4adf1-103">WindowsPhoneEASEmailProfileConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="4adf1-103">Create windowsPhoneEASEmailProfileConfiguration</span></span>

> <span data-ttu-id="4adf1-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4adf1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4adf1-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4adf1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4adf1-106">新しい[Windowsphoneeasemailprofileconfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="4adf1-106">Create a new [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4adf1-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="4adf1-107">Prerequisites</span></span>
<span data-ttu-id="4adf1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4adf1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4adf1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4adf1-110">Permission type</span></span>|<span data-ttu-id="4adf1-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4adf1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4adf1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4adf1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4adf1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4adf1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4adf1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4adf1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4adf1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4adf1-115">Not supported.</span></span>|
|<span data-ttu-id="4adf1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4adf1-116">Application</span></span>|<span data-ttu-id="4adf1-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4adf1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4adf1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4adf1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4adf1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4adf1-119">Request headers</span></span>
|<span data-ttu-id="4adf1-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4adf1-120">Header</span></span>|<span data-ttu-id="4adf1-121">値</span><span class="sxs-lookup"><span data-stu-id="4adf1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4adf1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4adf1-122">Authorization</span></span>|<span data-ttu-id="4adf1-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="4adf1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4adf1-124">承諾</span><span class="sxs-lookup"><span data-stu-id="4adf1-124">Accept</span></span>|<span data-ttu-id="4adf1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4adf1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4adf1-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="4adf1-126">Request body</span></span>
<span data-ttu-id="4adf1-127">要求本文で、windowsPhoneEASEmailProfileConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4adf1-127">In the request body, supply a JSON representation for the windowsPhoneEASEmailProfileConfiguration object.</span></span>

<span data-ttu-id="4adf1-128">次の表に、windowsPhoneEASEmailProfileConfiguration 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4adf1-128">The following table shows the properties that are required when you create the windowsPhoneEASEmailProfileConfiguration.</span></span>

|<span data-ttu-id="4adf1-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4adf1-129">Property</span></span>|<span data-ttu-id="4adf1-130">型</span><span class="sxs-lookup"><span data-stu-id="4adf1-130">Type</span></span>|<span data-ttu-id="4adf1-131">説明</span><span class="sxs-lookup"><span data-stu-id="4adf1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4adf1-132">id</span><span class="sxs-lookup"><span data-stu-id="4adf1-132">id</span></span>|<span data-ttu-id="4adf1-133">文字列</span><span class="sxs-lookup"><span data-stu-id="4adf1-133">String</span></span>|<span data-ttu-id="4adf1-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="4adf1-134">Key of the entity.</span></span> <span data-ttu-id="4adf1-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4adf1-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4adf1-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4adf1-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4adf1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4adf1-137">DateTimeOffset</span></span>|<span data-ttu-id="4adf1-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="4adf1-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4adf1-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4adf1-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4adf1-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4adf1-140">roleScopeTagIds</span></span>|<span data-ttu-id="4adf1-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="4adf1-141">String collection</span></span>|<span data-ttu-id="4adf1-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="4adf1-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4adf1-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4adf1-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4adf1-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4adf1-144">supportsScopeTags</span></span>|<span data-ttu-id="4adf1-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="4adf1-145">Boolean</span></span>|<span data-ttu-id="4adf1-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4adf1-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4adf1-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="4adf1-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4adf1-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="4adf1-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4adf1-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="4adf1-149">This property is read-only.</span></span> <span data-ttu-id="4adf1-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4adf1-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4adf1-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4adf1-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4adf1-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4adf1-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4adf1-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="4adf1-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4adf1-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4adf1-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4adf1-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4adf1-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4adf1-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4adf1-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4adf1-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="4adf1-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4adf1-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4adf1-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4adf1-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="4adf1-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4adf1-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="4adf1-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4adf1-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="4adf1-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4adf1-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4adf1-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4adf1-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4adf1-163">createdDateTime</span></span>|<span data-ttu-id="4adf1-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4adf1-164">DateTimeOffset</span></span>|<span data-ttu-id="4adf1-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="4adf1-165">DateTime the object was created.</span></span> <span data-ttu-id="4adf1-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4adf1-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4adf1-167">description</span><span class="sxs-lookup"><span data-stu-id="4adf1-167">description</span></span>|<span data-ttu-id="4adf1-168">String</span><span class="sxs-lookup"><span data-stu-id="4adf1-168">String</span></span>|<span data-ttu-id="4adf1-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="4adf1-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4adf1-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4adf1-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4adf1-171">displayName</span><span class="sxs-lookup"><span data-stu-id="4adf1-171">displayName</span></span>|<span data-ttu-id="4adf1-172">String</span><span class="sxs-lookup"><span data-stu-id="4adf1-172">String</span></span>|<span data-ttu-id="4adf1-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="4adf1-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4adf1-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4adf1-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4adf1-175">version</span><span class="sxs-lookup"><span data-stu-id="4adf1-175">version</span></span>|<span data-ttu-id="4adf1-176">Int32</span><span class="sxs-lookup"><span data-stu-id="4adf1-176">Int32</span></span>|<span data-ttu-id="4adf1-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="4adf1-177">Version of the device configuration.</span></span> <span data-ttu-id="4adf1-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4adf1-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4adf1-179">usernameSource</span><span class="sxs-lookup"><span data-stu-id="4adf1-179">usernameSource</span></span>|[<span data-ttu-id="4adf1-180">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="4adf1-180">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="4adf1-181">ユーザー名属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。</span><span class="sxs-lookup"><span data-stu-id="4adf1-181">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="4adf1-182">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="4adf1-182">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="4adf1-183">可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="4adf1-183">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="4adf1-184">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="4adf1-184">usernameAADSource</span></span>|[<span data-ttu-id="4adf1-185">usernameSource</span><span class="sxs-lookup"><span data-stu-id="4adf1-185">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="4adf1-186">メールプロファイルのユーザー名を取得するために使用される AAD フィールドの名前。</span><span class="sxs-lookup"><span data-stu-id="4adf1-186">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="4adf1-187">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="4adf1-187">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="4adf1-188">可能な値は、`userPrincipalName`、`primarySmtpAddress`、`samAccountName` です。</span><span class="sxs-lookup"><span data-stu-id="4adf1-188">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="4adf1-189">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="4adf1-189">userDomainNameSource</span></span>|[<span data-ttu-id="4adf1-190">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="4adf1-190">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="4adf1-191">UserDomainname 属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。</span><span class="sxs-lookup"><span data-stu-id="4adf1-191">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="4adf1-192">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="4adf1-192">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="4adf1-193">可能な値は、`fullDomainName`、`netBiosDomainName` です。</span><span class="sxs-lookup"><span data-stu-id="4adf1-193">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="4adf1-194">customDomainName</span><span class="sxs-lookup"><span data-stu-id="4adf1-194">customDomainName</span></span>|<span data-ttu-id="4adf1-195">String</span><span class="sxs-lookup"><span data-stu-id="4adf1-195">String</span></span>|<span data-ttu-id="4adf1-196">デバイスにインストールする前に電子メールプロファイルを生成するときに使用するカスタムドメイン名の値。</span><span class="sxs-lookup"><span data-stu-id="4adf1-196">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="4adf1-197">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="4adf1-197">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="4adf1-198">accountName</span><span class="sxs-lookup"><span data-stu-id="4adf1-198">accountName</span></span>|<span data-ttu-id="4adf1-199">String</span><span class="sxs-lookup"><span data-stu-id="4adf1-199">String</span></span>|<span data-ttu-id="4adf1-200">アカウント名。</span><span class="sxs-lookup"><span data-stu-id="4adf1-200">Account name.</span></span>|
|<span data-ttu-id="4adf1-201">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="4adf1-201">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="4adf1-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="4adf1-202">Boolean</span></span>|<span data-ttu-id="4adf1-203">このポリシーを Windows 8.1 にのみ適用するかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="4adf1-203">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="4adf1-204">このプロパティは読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4adf1-204">This property is read-only.</span></span>|
|<span data-ttu-id="4adf1-205">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="4adf1-205">syncCalendar</span></span>|<span data-ttu-id="4adf1-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="4adf1-206">Boolean</span></span>|<span data-ttu-id="4adf1-207">予定表を同期するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="4adf1-207">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="4adf1-208">syncContacts</span><span class="sxs-lookup"><span data-stu-id="4adf1-208">syncContacts</span></span>|<span data-ttu-id="4adf1-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="4adf1-209">Boolean</span></span>|<span data-ttu-id="4adf1-210">連絡先を同期するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="4adf1-210">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="4adf1-211">syncTasks</span><span class="sxs-lookup"><span data-stu-id="4adf1-211">syncTasks</span></span>|<span data-ttu-id="4adf1-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="4adf1-212">Boolean</span></span>|<span data-ttu-id="4adf1-213">タスクを同期するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="4adf1-213">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="4adf1-214">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="4adf1-214">durationOfEmailToSync</span></span>|[<span data-ttu-id="4adf1-215">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="4adf1-215">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="4adf1-216">同期する電子メールの期間。可能な値は`userDefined`、 `oneDay`、 `threeDays` `oneWeek` `twoWeeks` `oneMonth`、、、、 `unlimited`、です。</span><span class="sxs-lookup"><span data-stu-id="4adf1-216">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="4adf1-217">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="4adf1-217">emailAddressSource</span></span>|[<span data-ttu-id="4adf1-218">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="4adf1-218">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="4adf1-219">AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入される電子メール属性。</span><span class="sxs-lookup"><span data-stu-id="4adf1-219">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="4adf1-220">可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="4adf1-220">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="4adf1-221">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="4adf1-221">emailSyncSchedule</span></span>|[<span data-ttu-id="4adf1-222">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="4adf1-222">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="4adf1-223">電子メール同期スケジュール。</span><span class="sxs-lookup"><span data-stu-id="4adf1-223">Email sync schedule.</span></span> <span data-ttu-id="4adf1-224">可能な値は、`userDefined`、`asMessagesArrive`、`manual`、`fifteenMinutes`、`thirtyMinutes`、`sixtyMinutes`、`basedOnMyUsage` です。</span><span class="sxs-lookup"><span data-stu-id="4adf1-224">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="4adf1-225">hostName</span><span class="sxs-lookup"><span data-stu-id="4adf1-225">hostName</span></span>|<span data-ttu-id="4adf1-226">String</span><span class="sxs-lookup"><span data-stu-id="4adf1-226">String</span></span>|<span data-ttu-id="4adf1-227">ネイティブメールアプリが接続する Exchange の場所 (URL)。</span><span class="sxs-lookup"><span data-stu-id="4adf1-227">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="4adf1-228">requireSsl</span><span class="sxs-lookup"><span data-stu-id="4adf1-228">requireSsl</span></span>|<span data-ttu-id="4adf1-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="4adf1-229">Boolean</span></span>|<span data-ttu-id="4adf1-230">SSL を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4adf1-230">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="4adf1-231">応答</span><span class="sxs-lookup"><span data-stu-id="4adf1-231">Response</span></span>
<span data-ttu-id="4adf1-232">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[Windowsphoneeasemailprofileconfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4adf1-232">If successful, this method returns a `201 Created` response code and a [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4adf1-233">例</span><span class="sxs-lookup"><span data-stu-id="4adf1-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="4adf1-234">要求</span><span class="sxs-lookup"><span data-stu-id="4adf1-234">Request</span></span>
<span data-ttu-id="4adf1-235">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4adf1-235">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="4adf1-236">応答</span><span class="sxs-lookup"><span data-stu-id="4adf1-236">Response</span></span>
<span data-ttu-id="4adf1-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4adf1-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





