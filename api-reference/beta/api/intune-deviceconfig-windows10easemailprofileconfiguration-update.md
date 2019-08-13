---
title: Windows10EasEmailProfileConfiguration の更新
description: Windows10EasEmailProfileConfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 20a3487ad728345e86057a06420122936c6d5c92
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36345310"
---
# <a name="update-windows10easemailprofileconfiguration"></a><span data-ttu-id="d2da1-103">Windows10EasEmailProfileConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="d2da1-103">Update windows10EasEmailProfileConfiguration</span></span>

> <span data-ttu-id="d2da1-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2da1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2da1-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d2da1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2da1-106">[Windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d2da1-106">Update the properties of a [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d2da1-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="d2da1-107">Prerequisites</span></span>
<span data-ttu-id="d2da1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d2da1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2da1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d2da1-110">Permission type</span></span>|<span data-ttu-id="d2da1-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d2da1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2da1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d2da1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d2da1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2da1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d2da1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d2da1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2da1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2da1-115">Not supported.</span></span>|
|<span data-ttu-id="d2da1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d2da1-116">Application</span></span>|<span data-ttu-id="d2da1-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2da1-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2da1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d2da1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d2da1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d2da1-119">Request headers</span></span>
|<span data-ttu-id="d2da1-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d2da1-120">Header</span></span>|<span data-ttu-id="d2da1-121">値</span><span class="sxs-lookup"><span data-stu-id="d2da1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2da1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2da1-122">Authorization</span></span>|<span data-ttu-id="d2da1-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d2da1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2da1-124">承諾</span><span class="sxs-lookup"><span data-stu-id="d2da1-124">Accept</span></span>|<span data-ttu-id="d2da1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d2da1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2da1-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d2da1-126">Request body</span></span>
<span data-ttu-id="d2da1-127">要求本文で、 [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d2da1-127">In the request body, supply a JSON representation for the [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="d2da1-128">次の表に、 [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d2da1-128">The following table shows the properties that are required when you create the [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="d2da1-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d2da1-129">Property</span></span>|<span data-ttu-id="d2da1-130">型</span><span class="sxs-lookup"><span data-stu-id="d2da1-130">Type</span></span>|<span data-ttu-id="d2da1-131">説明</span><span class="sxs-lookup"><span data-stu-id="d2da1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2da1-132">id</span><span class="sxs-lookup"><span data-stu-id="d2da1-132">id</span></span>|<span data-ttu-id="d2da1-133">文字列</span><span class="sxs-lookup"><span data-stu-id="d2da1-133">String</span></span>|<span data-ttu-id="d2da1-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d2da1-134">Key of the entity.</span></span> <span data-ttu-id="d2da1-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d2da1-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2da1-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d2da1-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d2da1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2da1-137">DateTimeOffset</span></span>|<span data-ttu-id="d2da1-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="d2da1-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d2da1-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d2da1-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2da1-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d2da1-140">roleScopeTagIds</span></span>|<span data-ttu-id="d2da1-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="d2da1-141">String collection</span></span>|<span data-ttu-id="d2da1-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="d2da1-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d2da1-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d2da1-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2da1-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d2da1-144">supportsScopeTags</span></span>|<span data-ttu-id="d2da1-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2da1-145">Boolean</span></span>|<span data-ttu-id="d2da1-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d2da1-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d2da1-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="d2da1-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d2da1-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="d2da1-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d2da1-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="d2da1-149">This property is read-only.</span></span> <span data-ttu-id="d2da1-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d2da1-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2da1-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d2da1-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d2da1-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d2da1-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d2da1-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="d2da1-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d2da1-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d2da1-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2da1-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d2da1-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d2da1-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d2da1-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d2da1-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="d2da1-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d2da1-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d2da1-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2da1-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="d2da1-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d2da1-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="d2da1-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d2da1-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="d2da1-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d2da1-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d2da1-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2da1-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d2da1-163">createdDateTime</span></span>|<span data-ttu-id="d2da1-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2da1-164">DateTimeOffset</span></span>|<span data-ttu-id="d2da1-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="d2da1-165">DateTime the object was created.</span></span> <span data-ttu-id="d2da1-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d2da1-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2da1-167">description</span><span class="sxs-lookup"><span data-stu-id="d2da1-167">description</span></span>|<span data-ttu-id="d2da1-168">String</span><span class="sxs-lookup"><span data-stu-id="d2da1-168">String</span></span>|<span data-ttu-id="d2da1-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="d2da1-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d2da1-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d2da1-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2da1-171">displayName</span><span class="sxs-lookup"><span data-stu-id="d2da1-171">displayName</span></span>|<span data-ttu-id="d2da1-172">String</span><span class="sxs-lookup"><span data-stu-id="d2da1-172">String</span></span>|<span data-ttu-id="d2da1-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="d2da1-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d2da1-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d2da1-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2da1-175">version</span><span class="sxs-lookup"><span data-stu-id="d2da1-175">version</span></span>|<span data-ttu-id="d2da1-176">Int32</span><span class="sxs-lookup"><span data-stu-id="d2da1-176">Int32</span></span>|<span data-ttu-id="d2da1-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="d2da1-177">Version of the device configuration.</span></span> <span data-ttu-id="d2da1-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d2da1-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2da1-179">usernameSource</span><span class="sxs-lookup"><span data-stu-id="d2da1-179">usernameSource</span></span>|[<span data-ttu-id="d2da1-180">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="d2da1-180">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="d2da1-181">ユーザー名属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。</span><span class="sxs-lookup"><span data-stu-id="d2da1-181">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="d2da1-182">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="d2da1-182">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="d2da1-183">可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="d2da1-183">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="d2da1-184">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="d2da1-184">usernameAADSource</span></span>|[<span data-ttu-id="d2da1-185">usernameSource</span><span class="sxs-lookup"><span data-stu-id="d2da1-185">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="d2da1-186">メールプロファイルのユーザー名を取得するために使用される AAD フィールドの名前。</span><span class="sxs-lookup"><span data-stu-id="d2da1-186">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="d2da1-187">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="d2da1-187">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="d2da1-188">可能な値は、`userPrincipalName`、`primarySmtpAddress`、`samAccountName` です。</span><span class="sxs-lookup"><span data-stu-id="d2da1-188">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="d2da1-189">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="d2da1-189">userDomainNameSource</span></span>|[<span data-ttu-id="d2da1-190">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="d2da1-190">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="d2da1-191">UserDomainname 属性。 AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入されます。</span><span class="sxs-lookup"><span data-stu-id="d2da1-191">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="d2da1-192">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="d2da1-192">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="d2da1-193">可能な値は、`fullDomainName`、`netBiosDomainName` です。</span><span class="sxs-lookup"><span data-stu-id="d2da1-193">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="d2da1-194">customDomainName</span><span class="sxs-lookup"><span data-stu-id="d2da1-194">customDomainName</span></span>|<span data-ttu-id="d2da1-195">String</span><span class="sxs-lookup"><span data-stu-id="d2da1-195">String</span></span>|<span data-ttu-id="d2da1-196">デバイスにインストールする前に電子メールプロファイルを生成するときに使用するカスタムドメイン名の値。</span><span class="sxs-lookup"><span data-stu-id="d2da1-196">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="d2da1-197">[EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="d2da1-197">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="d2da1-198">accountName</span><span class="sxs-lookup"><span data-stu-id="d2da1-198">accountName</span></span>|<span data-ttu-id="d2da1-199">String</span><span class="sxs-lookup"><span data-stu-id="d2da1-199">String</span></span>|<span data-ttu-id="d2da1-200">アカウント名。</span><span class="sxs-lookup"><span data-stu-id="d2da1-200">Account name.</span></span>|
|<span data-ttu-id="d2da1-201">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="d2da1-201">syncCalendar</span></span>|<span data-ttu-id="d2da1-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2da1-202">Boolean</span></span>|<span data-ttu-id="d2da1-203">予定表を同期するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="d2da1-203">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="d2da1-204">syncContacts</span><span class="sxs-lookup"><span data-stu-id="d2da1-204">syncContacts</span></span>|<span data-ttu-id="d2da1-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2da1-205">Boolean</span></span>|<span data-ttu-id="d2da1-206">連絡先を同期するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="d2da1-206">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="d2da1-207">syncTasks</span><span class="sxs-lookup"><span data-stu-id="d2da1-207">syncTasks</span></span>|<span data-ttu-id="d2da1-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2da1-208">Boolean</span></span>|<span data-ttu-id="d2da1-209">タスクを同期するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="d2da1-209">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="d2da1-210">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="d2da1-210">durationOfEmailToSync</span></span>|[<span data-ttu-id="d2da1-211">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="d2da1-211">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="d2da1-212">同期する電子メールの期間。可能な値は`userDefined`、 `oneDay`、 `threeDays` `oneWeek` `twoWeeks` `oneMonth`、、、、 `unlimited`、です。</span><span class="sxs-lookup"><span data-stu-id="d2da1-212">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="d2da1-213">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="d2da1-213">emailAddressSource</span></span>|[<span data-ttu-id="d2da1-214">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="d2da1-214">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="d2da1-215">AAD から選択され、デバイスにインストールする前にこのプロファイルに挿入される電子メール属性。</span><span class="sxs-lookup"><span data-stu-id="d2da1-215">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="d2da1-216">可能な値は、`userPrincipalName`、`primarySmtpAddress` です。</span><span class="sxs-lookup"><span data-stu-id="d2da1-216">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="d2da1-217">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="d2da1-217">emailSyncSchedule</span></span>|[<span data-ttu-id="d2da1-218">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="d2da1-218">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="d2da1-219">電子メール同期スケジュール。</span><span class="sxs-lookup"><span data-stu-id="d2da1-219">Email sync schedule.</span></span> <span data-ttu-id="d2da1-220">可能な値は、`userDefined`、`asMessagesArrive`、`manual`、`fifteenMinutes`、`thirtyMinutes`、`sixtyMinutes`、`basedOnMyUsage` です。</span><span class="sxs-lookup"><span data-stu-id="d2da1-220">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="d2da1-221">hostName</span><span class="sxs-lookup"><span data-stu-id="d2da1-221">hostName</span></span>|<span data-ttu-id="d2da1-222">String</span><span class="sxs-lookup"><span data-stu-id="d2da1-222">String</span></span>|<span data-ttu-id="d2da1-223">ネイティブメールアプリが接続する Exchange の場所 (URL)。</span><span class="sxs-lookup"><span data-stu-id="d2da1-223">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="d2da1-224">requireSsl</span><span class="sxs-lookup"><span data-stu-id="d2da1-224">requireSsl</span></span>|<span data-ttu-id="d2da1-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2da1-225">Boolean</span></span>|<span data-ttu-id="d2da1-226">SSL を使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d2da1-226">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="d2da1-227">応答</span><span class="sxs-lookup"><span data-stu-id="d2da1-227">Response</span></span>
<span data-ttu-id="d2da1-228">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d2da1-228">If successful, this method returns a `200 OK` response code and an updated [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2da1-229">例</span><span class="sxs-lookup"><span data-stu-id="d2da1-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2da1-230">要求</span><span class="sxs-lookup"><span data-stu-id="d2da1-230">Request</span></span>
<span data-ttu-id="d2da1-231">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d2da1-231">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="d2da1-232">応答</span><span class="sxs-lookup"><span data-stu-id="d2da1-232">Response</span></span>
<span data-ttu-id="d2da1-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d2da1-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






