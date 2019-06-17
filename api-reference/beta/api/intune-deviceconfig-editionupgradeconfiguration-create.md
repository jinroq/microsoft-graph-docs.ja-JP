---
title: editionUpgradeConfiguration の作成
description: 新しい editionUpgradeConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 02557152a32acbb3c44a7efa08e2332985295f6d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34967413"
---
# <a name="create-editionupgradeconfiguration"></a><span data-ttu-id="b916e-103">editionUpgradeConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="b916e-103">Create editionUpgradeConfiguration</span></span>

> <span data-ttu-id="b916e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b916e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b916e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b916e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b916e-106">新しい [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b916e-106">Create a new [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b916e-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="b916e-107">Prerequisites</span></span>
<span data-ttu-id="b916e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b916e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b916e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b916e-110">Permission type</span></span>|<span data-ttu-id="b916e-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b916e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b916e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b916e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b916e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b916e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b916e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b916e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b916e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b916e-115">Not supported.</span></span>|
|<span data-ttu-id="b916e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b916e-116">Application</span></span>|<span data-ttu-id="b916e-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b916e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b916e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b916e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b916e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b916e-119">Request headers</span></span>
|<span data-ttu-id="b916e-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b916e-120">Header</span></span>|<span data-ttu-id="b916e-121">値</span><span class="sxs-lookup"><span data-stu-id="b916e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b916e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b916e-122">Authorization</span></span>|<span data-ttu-id="b916e-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="b916e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b916e-124">承諾</span><span class="sxs-lookup"><span data-stu-id="b916e-124">Accept</span></span>|<span data-ttu-id="b916e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b916e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b916e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="b916e-126">Request body</span></span>
<span data-ttu-id="b916e-127">要求本文では、editionUpgradeConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b916e-127">In the request body, supply a JSON representation for the editionUpgradeConfiguration object.</span></span>

<span data-ttu-id="b916e-128">次の表に、editionUpgradeConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b916e-128">The following table shows the properties that are required when you create the editionUpgradeConfiguration.</span></span>

|<span data-ttu-id="b916e-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b916e-129">Property</span></span>|<span data-ttu-id="b916e-130">型</span><span class="sxs-lookup"><span data-stu-id="b916e-130">Type</span></span>|<span data-ttu-id="b916e-131">説明</span><span class="sxs-lookup"><span data-stu-id="b916e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b916e-132">id</span><span class="sxs-lookup"><span data-stu-id="b916e-132">id</span></span>|<span data-ttu-id="b916e-133">文字列</span><span class="sxs-lookup"><span data-stu-id="b916e-133">String</span></span>|<span data-ttu-id="b916e-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b916e-134">Key of the entity.</span></span> <span data-ttu-id="b916e-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b916e-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b916e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b916e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b916e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b916e-137">DateTimeOffset</span></span>|<span data-ttu-id="b916e-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="b916e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b916e-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b916e-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b916e-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b916e-140">roleScopeTagIds</span></span>|<span data-ttu-id="b916e-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="b916e-141">String collection</span></span>|<span data-ttu-id="b916e-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="b916e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b916e-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b916e-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b916e-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b916e-144">supportsScopeTags</span></span>|<span data-ttu-id="b916e-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="b916e-145">Boolean</span></span>|<span data-ttu-id="b916e-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b916e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b916e-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="b916e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b916e-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="b916e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b916e-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="b916e-149">This property is read-only.</span></span> <span data-ttu-id="b916e-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b916e-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b916e-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b916e-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b916e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b916e-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b916e-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="b916e-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b916e-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b916e-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b916e-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b916e-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b916e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b916e-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b916e-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="b916e-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b916e-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b916e-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b916e-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="b916e-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b916e-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="b916e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b916e-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="b916e-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b916e-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b916e-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b916e-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b916e-163">createdDateTime</span></span>|<span data-ttu-id="b916e-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b916e-164">DateTimeOffset</span></span>|<span data-ttu-id="b916e-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="b916e-165">DateTime the object was created.</span></span> <span data-ttu-id="b916e-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b916e-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b916e-167">description</span><span class="sxs-lookup"><span data-stu-id="b916e-167">description</span></span>|<span data-ttu-id="b916e-168">String</span><span class="sxs-lookup"><span data-stu-id="b916e-168">String</span></span>|<span data-ttu-id="b916e-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="b916e-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b916e-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b916e-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b916e-171">displayName</span><span class="sxs-lookup"><span data-stu-id="b916e-171">displayName</span></span>|<span data-ttu-id="b916e-172">String</span><span class="sxs-lookup"><span data-stu-id="b916e-172">String</span></span>|<span data-ttu-id="b916e-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="b916e-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b916e-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b916e-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b916e-175">version</span><span class="sxs-lookup"><span data-stu-id="b916e-175">version</span></span>|<span data-ttu-id="b916e-176">Int32</span><span class="sxs-lookup"><span data-stu-id="b916e-176">Int32</span></span>|<span data-ttu-id="b916e-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="b916e-177">Version of the device configuration.</span></span> <span data-ttu-id="b916e-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b916e-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b916e-179">licenseType</span><span class="sxs-lookup"><span data-stu-id="b916e-179">licenseType</span></span>|[<span data-ttu-id="b916e-180">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="b916e-180">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="b916e-181">エディション アップグレード ライセンスの種類。</span><span class="sxs-lookup"><span data-stu-id="b916e-181">Edition Upgrade License Type.</span></span> <span data-ttu-id="b916e-182">可能な値は、`productKey`、`licenseFile`、`notConfigured` です。</span><span class="sxs-lookup"><span data-stu-id="b916e-182">Possible values are: `productKey`, `licenseFile`, `notConfigured`.</span></span>|
|<span data-ttu-id="b916e-183">targetEdition</span><span class="sxs-lookup"><span data-stu-id="b916e-183">targetEdition</span></span>|[<span data-ttu-id="b916e-184">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="b916e-184">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="b916e-185">エディション アップグレードの対象エディション。</span><span class="sxs-lookup"><span data-stu-id="b916e-185">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="b916e-186">可能な値: `windows10Enterprise`、 `windows10EnterpriseN` `windows10Education` `windows10EducationN` `windows10MobileEnterprise` `windows10HolographicEnterprise` `windows10Professional` `windows10ProfessionalN` `windows10ProfessionalEducation` `windows10ProfessionalEducationN` `windows10ProfessionalWorkstation` `windows10ProfessionalWorkstationN`、、、、、、、、、、、、 `notConfigured` `windows10Home` `windows10HomeChina` `windows10HomeN` `windows10HomeSingleLanguage` `windows10Mobile` `windows10IoTCore`, `windows10IoTCoreCommercial`.</span><span class="sxs-lookup"><span data-stu-id="b916e-186">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`, `windows10Home`, `windows10HomeChina`, `windows10HomeN`, `windows10HomeSingleLanguage`, `windows10Mobile`, `windows10IoTCore`, `windows10IoTCoreCommercial`.</span></span>|
|<span data-ttu-id="b916e-187">license</span><span class="sxs-lookup"><span data-stu-id="b916e-187">license</span></span>|<span data-ttu-id="b916e-188">String</span><span class="sxs-lookup"><span data-stu-id="b916e-188">String</span></span>|<span data-ttu-id="b916e-189">エディション アップグレード ライセンスのファイル コンテンツ。</span><span class="sxs-lookup"><span data-stu-id="b916e-189">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="b916e-190">productKey</span><span class="sxs-lookup"><span data-stu-id="b916e-190">productKey</span></span>|<span data-ttu-id="b916e-191">String</span><span class="sxs-lookup"><span data-stu-id="b916e-191">String</span></span>|<span data-ttu-id="b916e-192">エディション アップグレードのプロダクト キー。</span><span class="sxs-lookup"><span data-stu-id="b916e-192">Edition Upgrade Product Key.</span></span>|
|<span data-ttu-id="b916e-193">windowsSMode</span><span class="sxs-lookup"><span data-stu-id="b916e-193">windowsSMode</span></span>|[<span data-ttu-id="b916e-194">windowsSModeConfiguration</span><span class="sxs-lookup"><span data-stu-id="b916e-194">windowsSModeConfiguration</span></span>](../resources/intune-deviceconfig-windowssmodeconfiguration.md)|<span data-ttu-id="b916e-195">S モード構成。</span><span class="sxs-lookup"><span data-stu-id="b916e-195">S mode configuration.</span></span> <span data-ttu-id="b916e-196">可能な値は、`noRestriction`、`block`、`unlock` です。</span><span class="sxs-lookup"><span data-stu-id="b916e-196">Possible values are: `noRestriction`, `block`, `unlock`.</span></span>|



## <a name="response"></a><span data-ttu-id="b916e-197">応答</span><span class="sxs-lookup"><span data-stu-id="b916e-197">Response</span></span>
<span data-ttu-id="b916e-198">このメソッドが成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b916e-198">If successful, this method returns a `201 Created` response code and a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b916e-199">例</span><span class="sxs-lookup"><span data-stu-id="b916e-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="b916e-200">要求</span><span class="sxs-lookup"><span data-stu-id="b916e-200">Request</span></span>
<span data-ttu-id="b916e-201">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b916e-201">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1204

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
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
  "licenseType": "licenseFile",
  "targetEdition": "windows10EnterpriseN",
  "license": "License value",
  "productKey": "Product Key value",
  "windowsSMode": "block"
}
```

### <a name="response"></a><span data-ttu-id="b916e-202">応答</span><span class="sxs-lookup"><span data-stu-id="b916e-202">Response</span></span>
<span data-ttu-id="b916e-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b916e-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1376

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "id": "f39fc471-c471-f39f-71c4-9ff371c49ff3",
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
  "licenseType": "licenseFile",
  "targetEdition": "windows10EnterpriseN",
  "license": "License value",
  "productKey": "Product Key value",
  "windowsSMode": "block"
}
```





