---
title: Windows10EasEmailProfileConfiguration を作成する
description: 新しい windows10EasEmailProfileConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 020ae339b167ab04cf2495f7ff599409d0cf3322
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36345289"
---
# <a name="create-windows10easemailprofileconfiguration"></a><span data-ttu-id="9ecc6-103">Windows10EasEmailProfileConfiguration を作成する</span><span class="sxs-lookup"><span data-stu-id="9ecc6-103">Create windows10EasEmailProfileConfiguration</span></span>

> <span data-ttu-id="9ecc6-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ecc6-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ecc6-106">新しい[windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-106">Create a new [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ecc6-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="9ecc6-107">Prerequisites</span></span>
<span data-ttu-id="9ecc6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ecc6-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9ecc6-110">Permission type</span></span>|<span data-ttu-id="9ecc6-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9ecc6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ecc6-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9ecc6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9ecc6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ecc6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9ecc6-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9ecc6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ecc6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-115">Not supported.</span></span>|
|<span data-ttu-id="9ecc6-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9ecc6-116">Application</span></span>|<span data-ttu-id="9ecc6-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ecc6-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ecc6-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9ecc6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9ecc6-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9ecc6-119">Request headers</span></span>
|<span data-ttu-id="9ecc6-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9ecc6-120">Header</span></span>|<span data-ttu-id="9ecc6-121">値</span><span class="sxs-lookup"><span data-stu-id="9ecc6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ecc6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ecc6-122">Authorization</span></span>|<span data-ttu-id="9ecc6-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ecc6-124">承諾</span><span class="sxs-lookup"><span data-stu-id="9ecc6-124">Accept</span></span>|<span data-ttu-id="9ecc6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9ecc6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ecc6-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="9ecc6-126">Request body</span></span>
<span data-ttu-id="9ecc6-127">要求本文で、windows10EasEmailProfileConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-127">In the request body, supply a JSON representation for the windows10EasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="9ecc6-128">次の表に、windows10EasEmailProfileConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-128">The following table shows the properties that are required when you create the windows10EasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="9ecc6-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9ecc6-129">Property</span></span>|<span data-ttu-id="9ecc6-130">型</span><span class="sxs-lookup"><span data-stu-id="9ecc6-130">Type</span></span>|<span data-ttu-id="9ecc6-131">説明</span><span class="sxs-lookup"><span data-stu-id="9ecc6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ecc6-132">id</span><span class="sxs-lookup"><span data-stu-id="9ecc6-132">id</span></span>|<span data-ttu-id="9ecc6-133">文字列</span><span class="sxs-lookup"><span data-stu-id="9ecc6-133">String</span></span>|<span data-ttu-id="9ecc6-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-134">Key of the entity.</span></span> <span data-ttu-id="9ecc6-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9ecc6-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ecc6-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ecc6-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9ecc6-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ecc6-137">DateTimeOffset</span></span>|<span data-ttu-id="9ecc6-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-138">DateTime the object was last modified.</span></span> <span data-ttu-id="9ecc6-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9ecc6-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ecc6-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9ecc6-140">roleScopeTagIds</span></span>|<span data-ttu-id="9ecc6-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="9ecc6-141">String collection</span></span>|<span data-ttu-id="9ecc6-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9ecc6-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9ecc6-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ecc6-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9ecc6-144">supportsScopeTags</span></span>|<span data-ttu-id="9ecc6-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ecc6-145">Boolean</span></span>|<span data-ttu-id="9ecc6-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9ecc6-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9ecc6-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9ecc6-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-149">This property is read-only.</span></span> <span data-ttu-id="9ecc6-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9ecc6-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ecc6-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9ecc6-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="9ecc6-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9ecc6-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="9ecc6-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="9ecc6-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9ecc6-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ecc6-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9ecc6-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="9ecc6-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9ecc6-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="9ecc6-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="9ecc6-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9ecc6-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ecc6-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="9ecc6-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="9ecc6-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="9ecc6-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="9ecc6-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="9ecc6-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9ecc6-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ecc6-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9ecc6-163">createdDateTime</span></span>|<span data-ttu-id="9ecc6-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ecc6-164">DateTimeOffset</span></span>|<span data-ttu-id="9ecc6-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-165">DateTime the object was created.</span></span> <span data-ttu-id="9ecc6-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9ecc6-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ecc6-167">description</span><span class="sxs-lookup"><span data-stu-id="9ecc6-167">description</span></span>|<span data-ttu-id="9ecc6-168">String</span><span class="sxs-lookup"><span data-stu-id="9ecc6-168">String</span></span>|<span data-ttu-id="9ecc6-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9ecc6-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9ecc6-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ecc6-171">displayName</span><span class="sxs-lookup"><span data-stu-id="9ecc6-171">displayName</span></span>|<span data-ttu-id="9ecc6-172">String</span><span class="sxs-lookup"><span data-stu-id="9ecc6-172">String</span></span>|<span data-ttu-id="9ecc6-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9ecc6-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9ecc6-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ecc6-175">version</span><span class="sxs-lookup"><span data-stu-id="9ecc6-175">version</span></span>|<span data-ttu-id="9ecc6-176">Int32</span><span class="sxs-lookup"><span data-stu-id="9ecc6-176">Int32</span></span>|<span data-ttu-id="9ecc6-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-177">Version of the device configuration.</span></span> <span data-ttu-id="9ecc6-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9ecc6-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ecc6-179">usernameSource</span><span class="sxs-lookup"><span data-stu-id="9ecc6-179">usernameSource</span></span>|[<span data-ttu-id="9ecc6-180">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="9ecc6-180">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="9ecc6-181">ユーザー名属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-181">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="9ecc6-182">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-182">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="9ecc6-183">可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-183">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="9ecc6-184">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="9ecc6-184">usernameAADSource</span></span>|[<span data-ttu-id="9ecc6-185">usernameSource</span><span class="sxs-lookup"><span data-stu-id="9ecc6-185">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="9ecc6-186">メールプロファイルのユーザー名を取得するために使用される AAD フィールドの名前。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-186">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="9ecc6-187">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-187">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="9ecc6-188">可能な値は、`userPrincipalName`、`primarySmtpAddress`、`samAccountName` です。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-188">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="9ecc6-189">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="9ecc6-189">userDomainNameSource</span></span>|[<span data-ttu-id="9ecc6-190">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="9ecc6-190">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="9ecc6-191">UserDomainname 属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-191">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="9ecc6-192">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-192">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="9ecc6-193">可能な値は、`fullDomainName`、`netBiosDomainName` です。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-193">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="9ecc6-194">customDomainName</span><span class="sxs-lookup"><span data-stu-id="9ecc6-194">customDomainName</span></span>|<span data-ttu-id="9ecc6-195">String</span><span class="sxs-lookup"><span data-stu-id="9ecc6-195">String</span></span>|<span data-ttu-id="9ecc6-196">デバイスにインストールする前に電子メールプロファイルを生成するときに使用するカスタムドメイン名の値。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-196">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="9ecc6-197">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-197">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="9ecc6-198">accountName</span><span class="sxs-lookup"><span data-stu-id="9ecc6-198">accountName</span></span>|<span data-ttu-id="9ecc6-199">String</span><span class="sxs-lookup"><span data-stu-id="9ecc6-199">String</span></span>|<span data-ttu-id="9ecc6-200">アカウント名。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-200">Account name.</span></span>|
|<span data-ttu-id="9ecc6-201">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="9ecc6-201">syncCalendar</span></span>|<span data-ttu-id="9ecc6-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ecc6-202">Boolean</span></span>|<span data-ttu-id="9ecc6-203">予定表を同期するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-203">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="9ecc6-204">syncContacts</span><span class="sxs-lookup"><span data-stu-id="9ecc6-204">syncContacts</span></span>|<span data-ttu-id="9ecc6-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ecc6-205">Boolean</span></span>|<span data-ttu-id="9ecc6-206">連絡先を同期するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-206">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="9ecc6-207">syncTasks</span><span class="sxs-lookup"><span data-stu-id="9ecc6-207">syncTasks</span></span>|<span data-ttu-id="9ecc6-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ecc6-208">Boolean</span></span>|<span data-ttu-id="9ecc6-209">タスクを同期するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-209">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="9ecc6-210">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="9ecc6-210">durationOfEmailToSync</span></span>|[<span data-ttu-id="9ecc6-211">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="9ecc6-211">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="9ecc6-212">同期する電子メールの期間。可能な値は`userDefined`、 `oneDay`、 `threeDays` `oneWeek` `twoWeeks` `oneMonth`、、、、 `unlimited`、です。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-212">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="9ecc6-213">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="9ecc6-213">emailAddressSource</span></span>|[<span data-ttu-id="9ecc6-214">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="9ecc6-214">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="9ecc6-215">AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入される電子メール属性。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-215">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="9ecc6-216">可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-216">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="9ecc6-217">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="9ecc6-217">emailSyncSchedule</span></span>|[<span data-ttu-id="9ecc6-218">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="9ecc6-218">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="9ecc6-219">電子メール同期スケジュール。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-219">Email sync schedule.</span></span> <span data-ttu-id="9ecc6-220">可能な値は、`userDefined`、`asMessagesArrive`、`manual`、`fifteenMinutes`、`thirtyMinutes`、`sixtyMinutes`、`basedOnMyUsage` です。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-220">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="9ecc6-221">hostName</span><span class="sxs-lookup"><span data-stu-id="9ecc6-221">hostName</span></span>|<span data-ttu-id="9ecc6-222">String</span><span class="sxs-lookup"><span data-stu-id="9ecc6-222">String</span></span>|<span data-ttu-id="9ecc6-223">ネイティブメールアプリが接続する Exchange の場所 (URL)。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-223">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="9ecc6-224">requireSsl</span><span class="sxs-lookup"><span data-stu-id="9ecc6-224">requireSsl</span></span>|<span data-ttu-id="9ecc6-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ecc6-225">Boolean</span></span>|<span data-ttu-id="9ecc6-226">SSL を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-226">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="9ecc6-227">応答</span><span class="sxs-lookup"><span data-stu-id="9ecc6-227">Response</span></span>
<span data-ttu-id="9ecc6-228">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-228">If successful, this method returns a `201 Created` response code and a [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ecc6-229">例</span><span class="sxs-lookup"><span data-stu-id="9ecc6-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ecc6-230">要求</span><span class="sxs-lookup"><span data-stu-id="9ecc6-230">Request</span></span>
<span data-ttu-id="9ecc6-231">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-231">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1526

{
  "@odata.type": "#microsoft.graph.windows10EasEmailProfileConfiguration",
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

### <a name="response"></a><span data-ttu-id="9ecc6-232">応答</span><span class="sxs-lookup"><span data-stu-id="9ecc6-232">Response</span></span>
<span data-ttu-id="9ecc6-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9ecc6-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1698

{
  "@odata.type": "#microsoft.graph.windows10EasEmailProfileConfiguration",
  "id": "9dc6f073-f073-9dc6-73f0-c69d73f0c69d",
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






