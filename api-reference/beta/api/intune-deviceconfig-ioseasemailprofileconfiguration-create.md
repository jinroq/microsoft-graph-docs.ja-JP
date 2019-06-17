---
title: IosEasEmailProfileConfiguration 作成
description: 新しい iosEasEmailProfileConfiguration このオブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 526403ce3974b16b9bce90d39664ccc98959e256
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34967014"
---
# <a name="create-ioseasemailprofileconfiguration"></a><span data-ttu-id="ea3a3-103">IosEasEmailProfileConfiguration 作成</span><span class="sxs-lookup"><span data-stu-id="ea3a3-103">Create iosEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="ea3a3-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea3a3-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea3a3-106">新しい[Ioseasemailprofileconfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)このオブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-106">Create a new [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ea3a3-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="ea3a3-107">Prerequisites</span></span>
<span data-ttu-id="ea3a3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea3a3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ea3a3-110">Permission type</span></span>|<span data-ttu-id="ea3a3-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ea3a3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea3a3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ea3a3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ea3a3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea3a3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ea3a3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ea3a3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea3a3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-115">Not supported.</span></span>|
|<span data-ttu-id="ea3a3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ea3a3-116">Application</span></span>|<span data-ttu-id="ea3a3-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea3a3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ea3a3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ea3a3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ea3a3-119">Request headers</span></span>
|<span data-ttu-id="ea3a3-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ea3a3-120">Header</span></span>|<span data-ttu-id="ea3a3-121">値</span><span class="sxs-lookup"><span data-stu-id="ea3a3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea3a3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea3a3-122">Authorization</span></span>|<span data-ttu-id="ea3a3-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea3a3-124">承諾</span><span class="sxs-lookup"><span data-stu-id="ea3a3-124">Accept</span></span>|<span data-ttu-id="ea3a3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ea3a3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea3a3-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ea3a3-126">Request body</span></span>
<span data-ttu-id="ea3a3-127">要求本文で、iosEasEmailProfileConfiguration このオブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-127">In the request body, supply a JSON representation for the iosEasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="ea3a3-128">次の表に、iosEasEmailProfileConfiguration 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-128">The following table shows the properties that are required when you create the iosEasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="ea3a3-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ea3a3-129">Property</span></span>|<span data-ttu-id="ea3a3-130">型</span><span class="sxs-lookup"><span data-stu-id="ea3a3-130">Type</span></span>|<span data-ttu-id="ea3a3-131">説明</span><span class="sxs-lookup"><span data-stu-id="ea3a3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea3a3-132">id</span><span class="sxs-lookup"><span data-stu-id="ea3a3-132">id</span></span>|<span data-ttu-id="ea3a3-133">文字列</span><span class="sxs-lookup"><span data-stu-id="ea3a3-133">String</span></span>|<span data-ttu-id="ea3a3-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-134">Key of the entity.</span></span> <span data-ttu-id="ea3a3-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ea3a3-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea3a3-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ea3a3-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ea3a3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea3a3-137">DateTimeOffset</span></span>|<span data-ttu-id="ea3a3-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ea3a3-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ea3a3-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea3a3-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ea3a3-140">roleScopeTagIds</span></span>|<span data-ttu-id="ea3a3-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="ea3a3-141">String collection</span></span>|<span data-ttu-id="ea3a3-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ea3a3-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ea3a3-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea3a3-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ea3a3-144">supportsScopeTags</span></span>|<span data-ttu-id="ea3a3-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea3a3-145">Boolean</span></span>|<span data-ttu-id="ea3a3-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ea3a3-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ea3a3-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ea3a3-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-149">This property is read-only.</span></span> <span data-ttu-id="ea3a3-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ea3a3-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea3a3-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ea3a3-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ea3a3-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ea3a3-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ea3a3-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ea3a3-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ea3a3-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea3a3-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ea3a3-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ea3a3-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ea3a3-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ea3a3-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ea3a3-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ea3a3-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea3a3-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="ea3a3-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ea3a3-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="ea3a3-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ea3a3-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ea3a3-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ea3a3-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea3a3-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ea3a3-163">createdDateTime</span></span>|<span data-ttu-id="ea3a3-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea3a3-164">DateTimeOffset</span></span>|<span data-ttu-id="ea3a3-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-165">DateTime the object was created.</span></span> <span data-ttu-id="ea3a3-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ea3a3-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea3a3-167">description</span><span class="sxs-lookup"><span data-stu-id="ea3a3-167">description</span></span>|<span data-ttu-id="ea3a3-168">String</span><span class="sxs-lookup"><span data-stu-id="ea3a3-168">String</span></span>|<span data-ttu-id="ea3a3-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ea3a3-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ea3a3-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea3a3-171">displayName</span><span class="sxs-lookup"><span data-stu-id="ea3a3-171">displayName</span></span>|<span data-ttu-id="ea3a3-172">String</span><span class="sxs-lookup"><span data-stu-id="ea3a3-172">String</span></span>|<span data-ttu-id="ea3a3-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ea3a3-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ea3a3-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea3a3-175">version</span><span class="sxs-lookup"><span data-stu-id="ea3a3-175">version</span></span>|<span data-ttu-id="ea3a3-176">Int32</span><span class="sxs-lookup"><span data-stu-id="ea3a3-176">Int32</span></span>|<span data-ttu-id="ea3a3-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-177">Version of the device configuration.</span></span> <span data-ttu-id="ea3a3-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ea3a3-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea3a3-179">usernameSource</span><span class="sxs-lookup"><span data-stu-id="ea3a3-179">usernameSource</span></span>|[<span data-ttu-id="ea3a3-180">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="ea3a3-180">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="ea3a3-181">ユーザー名属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-181">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="ea3a3-182">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-182">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="ea3a3-183">可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-183">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="ea3a3-184">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="ea3a3-184">usernameAADSource</span></span>|[<span data-ttu-id="ea3a3-185">usernameSource</span><span class="sxs-lookup"><span data-stu-id="ea3a3-185">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="ea3a3-186">メールプロファイルのユーザー名を取得するために使用される AAD フィールドの名前。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-186">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="ea3a3-187">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-187">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="ea3a3-188">可能な値は、`userPrincipalName`、`primarySmtpAddress`、`samAccountName` です。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-188">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="ea3a3-189">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="ea3a3-189">userDomainNameSource</span></span>|[<span data-ttu-id="ea3a3-190">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="ea3a3-190">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="ea3a3-191">UserDomainname 属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-191">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="ea3a3-192">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-192">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="ea3a3-193">可能な値は、`fullDomainName`、`netBiosDomainName` です。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-193">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="ea3a3-194">customDomainName</span><span class="sxs-lookup"><span data-stu-id="ea3a3-194">customDomainName</span></span>|<span data-ttu-id="ea3a3-195">String</span><span class="sxs-lookup"><span data-stu-id="ea3a3-195">String</span></span>|<span data-ttu-id="ea3a3-196">デバイスにインストールする前に電子メールプロファイルを生成するときに使用するカスタムドメイン名の値。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-196">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="ea3a3-197">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-197">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="ea3a3-198">accountName</span><span class="sxs-lookup"><span data-stu-id="ea3a3-198">accountName</span></span>|<span data-ttu-id="ea3a3-199">String</span><span class="sxs-lookup"><span data-stu-id="ea3a3-199">String</span></span>|<span data-ttu-id="ea3a3-200">アカウント名。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-200">Account name.</span></span>|
|<span data-ttu-id="ea3a3-201">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ea3a3-201">authenticationMethod</span></span>|[<span data-ttu-id="ea3a3-202">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ea3a3-202">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="ea3a3-203">この電子メールプロファイルの認証方法。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-203">Authentication method for this Email profile.</span></span> <span data-ttu-id="ea3a3-204">可能な値は、`usernameAndPassword`、`certificate`、`derivedCredential` です。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-204">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="ea3a3-205">Blockmovingmessagestooruncommand/電子メールアカウント</span><span class="sxs-lookup"><span data-stu-id="ea3a3-205">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="ea3a3-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea3a3-206">Boolean</span></span>|<span data-ttu-id="ea3a3-207">他の電子メールアカウントへのメッセージの移動をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-207">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="ea3a3-208">blockSendingEmailFromThirdPartyApps</span><span class="sxs-lookup"><span data-stu-id="ea3a3-208">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="ea3a3-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea3a3-209">Boolean</span></span>|<span data-ttu-id="ea3a3-210">サードパーティ製アプリからの電子メールの送信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-210">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="ea3a3-211">blockSyncingRecentlyUsedEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="ea3a3-211">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="ea3a3-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea3a3-212">Boolean</span></span>|<span data-ttu-id="ea3a3-213">最近使用した電子メールアドレスの同期をブロックするかどうかを示します (たとえば、新しい電子メールを作成する場合)。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-213">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="ea3a3-214">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="ea3a3-214">durationOfEmailToSync</span></span>|[<span data-ttu-id="ea3a3-215">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="ea3a3-215">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="ea3a3-216">電子メールを同期する時間。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-216">Duration of time email should be synced back to.</span></span> <span data-ttu-id="ea3a3-217">.</span><span class="sxs-lookup"><span data-stu-id="ea3a3-217"></span></span> <span data-ttu-id="ea3a3-218">可能な値は、`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited` です。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-218">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="ea3a3-219">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="ea3a3-219">emailAddressSource</span></span>|[<span data-ttu-id="ea3a3-220">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="ea3a3-220">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="ea3a3-221">AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入される電子メール属性。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-221">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="ea3a3-222">可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-222">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="ea3a3-223">hostName</span><span class="sxs-lookup"><span data-stu-id="ea3a3-223">hostName</span></span>|<span data-ttu-id="ea3a3-224">String</span><span class="sxs-lookup"><span data-stu-id="ea3a3-224">String</span></span>|<span data-ttu-id="ea3a3-225">ネイティブメールアプリが接続する Exchange の場所 (URL)。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-225">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="ea3a3-226">requireSmime</span><span class="sxs-lookup"><span data-stu-id="ea3a3-226">requireSmime</span></span>|<span data-ttu-id="ea3a3-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea3a3-227">Boolean</span></span>|<span data-ttu-id="ea3a3-228">S/MIME 証明書を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-228">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="ea3a3-229">smimeEnablePerMessageSwitch</span><span class="sxs-lookup"><span data-stu-id="ea3a3-229">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="ea3a3-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea3a3-230">Boolean</span></span>|<span data-ttu-id="ea3a3-231">暗号化されていない電子メールを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-231">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="ea3a3-232">smimeEncryptByDefaultEnabled</span><span class="sxs-lookup"><span data-stu-id="ea3a3-232">smimeEncryptByDefaultEnabled</span></span>|<span data-ttu-id="ea3a3-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea3a3-233">Boolean</span></span>|<span data-ttu-id="ea3a3-234">True S/MIME 暗号化に設定すると、既定で有効になります。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-234">If set to true S/MIME encryption is enabled by default.</span></span>|
|<span data-ttu-id="ea3a3-235">smimeSigningEnabled</span><span class="sxs-lookup"><span data-stu-id="ea3a3-235">smimeSigningEnabled</span></span>|<span data-ttu-id="ea3a3-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea3a3-236">Boolean</span></span>|<span data-ttu-id="ea3a3-237">このアカウントに対して true S/MIME 署名を有効に設定した場合</span><span class="sxs-lookup"><span data-stu-id="ea3a3-237">If set to true S/MIME signing is enabled for this account</span></span>|
|<span data-ttu-id="ea3a3-238">smimeSigningUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="ea3a3-238">smimeSigningUserOverrideEnabled</span></span>|<span data-ttu-id="ea3a3-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea3a3-239">Boolean</span></span>|<span data-ttu-id="ea3a3-240">True に設定されている場合、ユーザーは S/MIME の署名のオンとオフを切り替えることができます。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-240">If set to true, the user can toggle S/MIME signing on or off.</span></span>|
|<span data-ttu-id="ea3a3-241">smimeEncryptByDefaultUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="ea3a3-241">smimeEncryptByDefaultUserOverrideEnabled</span></span>|<span data-ttu-id="ea3a3-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea3a3-242">Boolean</span></span>|<span data-ttu-id="ea3a3-243">True に設定されている場合、ユーザーは既定の設定で暗号化を切り替えることができます。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-243">If set to true, the user can toggle the encryption by default setting.</span></span>|
|<span data-ttu-id="ea3a3-244">smimeSigningCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="ea3a3-244">smimeSigningCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="ea3a3-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea3a3-245">Boolean</span></span>|<span data-ttu-id="ea3a3-246">True に設定されている場合、ユーザーは署名 id を選択できます。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-246">If set to true, the user can select the signing identity.</span></span>|
|<span data-ttu-id="ea3a3-247">smimeEncryptionCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="ea3a3-247">smimeEncryptionCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="ea3a3-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea3a3-248">Boolean</span></span>|<span data-ttu-id="ea3a3-249">True に設定されている場合、ユーザーは S/MIME 暗号化 id を選択できます。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-249">If set to true the user can select the S/MIME encryption identity.</span></span> |
|<span data-ttu-id="ea3a3-250">requireSsl</span><span class="sxs-lookup"><span data-stu-id="ea3a3-250">requireSsl</span></span>|<span data-ttu-id="ea3a3-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea3a3-251">Boolean</span></span>|<span data-ttu-id="ea3a3-252">SSL を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-252">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="ea3a3-253">useOAuth</span><span class="sxs-lookup"><span data-stu-id="ea3a3-253">useOAuth</span></span>|<span data-ttu-id="ea3a3-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea3a3-254">Boolean</span></span>|<span data-ttu-id="ea3a3-255">接続で認証に OAuth を使用するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-255">Specifies whether the connection should use OAuth for authentication.</span></span>|
|<span data-ttu-id="ea3a3-256">signingCertificateType</span><span class="sxs-lookup"><span data-stu-id="ea3a3-256">signingCertificateType</span></span>|[<span data-ttu-id="ea3a3-257">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="ea3a3-257">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="ea3a3-258">この電子メールプロファイルの署名証明書の種類。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-258">Signing Certificate type for this Email profile.</span></span> <span data-ttu-id="ea3a3-259">可能な値は、`none`、`certificate`、`derivedCredential` です。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-259">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="ea3a3-260">encryptionCertificateType</span><span class="sxs-lookup"><span data-stu-id="ea3a3-260">encryptionCertificateType</span></span>|[<span data-ttu-id="ea3a3-261">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="ea3a3-261">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="ea3a3-262">この電子メールプロファイルの暗号化証明書の種類。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-262">Encryption Certificate type for this Email profile.</span></span> <span data-ttu-id="ea3a3-263">可能な値は、`none`、`certificate`、`derivedCredential` です。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-263">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|



## <a name="response"></a><span data-ttu-id="ea3a3-264">応答</span><span class="sxs-lookup"><span data-stu-id="ea3a3-264">Response</span></span>
<span data-ttu-id="ea3a3-265">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[Ioseasemailprofileconfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) "オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-265">If successful, this method returns a `201 Created` response code and a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea3a3-266">例</span><span class="sxs-lookup"><span data-stu-id="ea3a3-266">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea3a3-267">要求</span><span class="sxs-lookup"><span data-stu-id="ea3a3-267">Request</span></span>
<span data-ttu-id="ea3a3-268">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-268">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2057

{
  "@odata.type": "#microsoft.graph.iosEasEmailProfileConfiguration",
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
  "authenticationMethod": "certificate",
  "blockMovingMessagesToOtherEmailAccounts": true,
  "blockSendingEmailFromThirdPartyApps": true,
  "blockSyncingRecentlyUsedEmailAddresses": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "hostName": "Host Name value",
  "requireSmime": true,
  "smimeEnablePerMessageSwitch": true,
  "smimeEncryptByDefaultEnabled": true,
  "smimeSigningEnabled": true,
  "smimeSigningUserOverrideEnabled": true,
  "smimeEncryptByDefaultUserOverrideEnabled": true,
  "smimeSigningCertificateUserOverrideEnabled": true,
  "smimeEncryptionCertificateUserOverrideEnabled": true,
  "requireSsl": true,
  "useOAuth": true,
  "signingCertificateType": "certificate",
  "encryptionCertificateType": "certificate"
}
```

### <a name="response"></a><span data-ttu-id="ea3a3-269">応答</span><span class="sxs-lookup"><span data-stu-id="ea3a3-269">Response</span></span>
<span data-ttu-id="ea3a3-p122">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ea3a3-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2229

{
  "@odata.type": "#microsoft.graph.iosEasEmailProfileConfiguration",
  "id": "e03086da-86da-e030-da86-30e0da8630e0",
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
  "authenticationMethod": "certificate",
  "blockMovingMessagesToOtherEmailAccounts": true,
  "blockSendingEmailFromThirdPartyApps": true,
  "blockSyncingRecentlyUsedEmailAddresses": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "hostName": "Host Name value",
  "requireSmime": true,
  "smimeEnablePerMessageSwitch": true,
  "smimeEncryptByDefaultEnabled": true,
  "smimeSigningEnabled": true,
  "smimeSigningUserOverrideEnabled": true,
  "smimeEncryptByDefaultUserOverrideEnabled": true,
  "smimeSigningCertificateUserOverrideEnabled": true,
  "smimeEncryptionCertificateUserOverrideEnabled": true,
  "requireSsl": true,
  "useOAuth": true,
  "signingCertificateType": "certificate",
  "encryptionCertificateType": "certificate"
}
```





