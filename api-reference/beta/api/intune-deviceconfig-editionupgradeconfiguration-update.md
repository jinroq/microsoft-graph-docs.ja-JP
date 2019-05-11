---
title: editionUpgradeConfiguration の更新
description: editionUpgradeConfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 132d8614026dbd582f3e5d7b5090b46748c62b30
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33926779"
---
# <a name="update-editionupgradeconfiguration"></a><span data-ttu-id="d5ff5-103">editionUpgradeConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="d5ff5-103">Update editionUpgradeConfiguration</span></span>

> <span data-ttu-id="d5ff5-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5ff5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5ff5-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d5ff5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5ff5-106">[editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d5ff5-106">Update the properties of a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d5ff5-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="d5ff5-107">Prerequisites</span></span>
<span data-ttu-id="d5ff5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d5ff5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5ff5-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d5ff5-110">Permission type</span></span>|<span data-ttu-id="d5ff5-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d5ff5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5ff5-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d5ff5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d5ff5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5ff5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d5ff5-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d5ff5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5ff5-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5ff5-115">Not supported.</span></span>|
|<span data-ttu-id="d5ff5-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d5ff5-116">Application</span></span>|<span data-ttu-id="d5ff5-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5ff5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5ff5-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d5ff5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d5ff5-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d5ff5-119">Request headers</span></span>
|<span data-ttu-id="d5ff5-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d5ff5-120">Header</span></span>|<span data-ttu-id="d5ff5-121">値</span><span class="sxs-lookup"><span data-stu-id="d5ff5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5ff5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5ff5-122">Authorization</span></span>|<span data-ttu-id="d5ff5-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d5ff5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5ff5-124">承諾</span><span class="sxs-lookup"><span data-stu-id="d5ff5-124">Accept</span></span>|<span data-ttu-id="d5ff5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d5ff5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5ff5-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d5ff5-126">Request body</span></span>
<span data-ttu-id="d5ff5-127">要求本文では、[editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d5ff5-127">In the request body, supply a JSON representation for the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

<span data-ttu-id="d5ff5-128">次の表に、[editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d5ff5-128">The following table shows the properties that are required when you create the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span></span>

|<span data-ttu-id="d5ff5-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d5ff5-129">Property</span></span>|<span data-ttu-id="d5ff5-130">型</span><span class="sxs-lookup"><span data-stu-id="d5ff5-130">Type</span></span>|<span data-ttu-id="d5ff5-131">説明</span><span class="sxs-lookup"><span data-stu-id="d5ff5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5ff5-132">id</span><span class="sxs-lookup"><span data-stu-id="d5ff5-132">id</span></span>|<span data-ttu-id="d5ff5-133">文字列</span><span class="sxs-lookup"><span data-stu-id="d5ff5-133">String</span></span>|<span data-ttu-id="d5ff5-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d5ff5-134">Key of the entity.</span></span> <span data-ttu-id="d5ff5-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5ff5-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5ff5-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d5ff5-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d5ff5-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5ff5-137">DateTimeOffset</span></span>|<span data-ttu-id="d5ff5-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="d5ff5-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d5ff5-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5ff5-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5ff5-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d5ff5-140">roleScopeTagIds</span></span>|<span data-ttu-id="d5ff5-141">String collection</span><span class="sxs-lookup"><span data-stu-id="d5ff5-141">String collection</span></span>|<span data-ttu-id="d5ff5-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="d5ff5-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d5ff5-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5ff5-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5ff5-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d5ff5-144">supportsScopeTags</span></span>|<span data-ttu-id="d5ff5-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5ff5-145">Boolean</span></span>|<span data-ttu-id="d5ff5-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d5ff5-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d5ff5-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="d5ff5-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d5ff5-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="d5ff5-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d5ff5-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="d5ff5-149">This property is read-only.</span></span> <span data-ttu-id="d5ff5-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5ff5-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5ff5-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d5ff5-151">createdDateTime</span></span>|<span data-ttu-id="d5ff5-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5ff5-152">DateTimeOffset</span></span>|<span data-ttu-id="d5ff5-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="d5ff5-153">DateTime the object was created.</span></span> <span data-ttu-id="d5ff5-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5ff5-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5ff5-155">description</span><span class="sxs-lookup"><span data-stu-id="d5ff5-155">description</span></span>|<span data-ttu-id="d5ff5-156">String</span><span class="sxs-lookup"><span data-stu-id="d5ff5-156">String</span></span>|<span data-ttu-id="d5ff5-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="d5ff5-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d5ff5-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5ff5-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5ff5-159">displayName</span><span class="sxs-lookup"><span data-stu-id="d5ff5-159">displayName</span></span>|<span data-ttu-id="d5ff5-160">String</span><span class="sxs-lookup"><span data-stu-id="d5ff5-160">String</span></span>|<span data-ttu-id="d5ff5-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="d5ff5-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d5ff5-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5ff5-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5ff5-163">version</span><span class="sxs-lookup"><span data-stu-id="d5ff5-163">version</span></span>|<span data-ttu-id="d5ff5-164">Int32</span><span class="sxs-lookup"><span data-stu-id="d5ff5-164">Int32</span></span>|<span data-ttu-id="d5ff5-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="d5ff5-165">Version of the device configuration.</span></span> <span data-ttu-id="d5ff5-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d5ff5-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5ff5-167">licenseType</span><span class="sxs-lookup"><span data-stu-id="d5ff5-167">licenseType</span></span>|[<span data-ttu-id="d5ff5-168">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="d5ff5-168">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="d5ff5-169">エディション アップグレード ライセンスの種類。</span><span class="sxs-lookup"><span data-stu-id="d5ff5-169">Edition Upgrade License Type.</span></span> <span data-ttu-id="d5ff5-170">可能な値は、`productKey`、`licenseFile`、`notConfigured` です。</span><span class="sxs-lookup"><span data-stu-id="d5ff5-170">Possible values are: `productKey`, `licenseFile`, `notConfigured`.</span></span>|
|<span data-ttu-id="d5ff5-171">targetEdition</span><span class="sxs-lookup"><span data-stu-id="d5ff5-171">targetEdition</span></span>|[<span data-ttu-id="d5ff5-172">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="d5ff5-172">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="d5ff5-173">エディション アップグレードの対象エディション。</span><span class="sxs-lookup"><span data-stu-id="d5ff5-173">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="d5ff5-174">可能な値は、`windows10Enterprise`、`windows10EnterpriseN`、`windows10Education`、`windows10EducationN`、`windows10MobileEnterprise`、`windows10HolographicEnterprise`、`windows10Professional`、`windows10ProfessionalN`、`windows10ProfessionalEducation`、`windows10ProfessionalEducationN`、`windows10ProfessionalWorkstation`、`windows10ProfessionalWorkstationN`、`notConfigured` です。</span><span class="sxs-lookup"><span data-stu-id="d5ff5-174">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`.</span></span>|
|<span data-ttu-id="d5ff5-175">license</span><span class="sxs-lookup"><span data-stu-id="d5ff5-175">license</span></span>|<span data-ttu-id="d5ff5-176">String</span><span class="sxs-lookup"><span data-stu-id="d5ff5-176">String</span></span>|<span data-ttu-id="d5ff5-177">エディション アップグレード ライセンスのファイル コンテンツ。</span><span class="sxs-lookup"><span data-stu-id="d5ff5-177">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="d5ff5-178">productKey</span><span class="sxs-lookup"><span data-stu-id="d5ff5-178">productKey</span></span>|<span data-ttu-id="d5ff5-179">String</span><span class="sxs-lookup"><span data-stu-id="d5ff5-179">String</span></span>|<span data-ttu-id="d5ff5-180">エディション アップグレードのプロダクト キー。</span><span class="sxs-lookup"><span data-stu-id="d5ff5-180">Edition Upgrade Product Key.</span></span>|
|<span data-ttu-id="d5ff5-181">windowsSMode</span><span class="sxs-lookup"><span data-stu-id="d5ff5-181">windowsSMode</span></span>|[<span data-ttu-id="d5ff5-182">windowsSModeConfiguration</span><span class="sxs-lookup"><span data-stu-id="d5ff5-182">windowsSModeConfiguration</span></span>](../resources/intune-deviceconfig-windowssmodeconfiguration.md)|<span data-ttu-id="d5ff5-183">S モード構成。</span><span class="sxs-lookup"><span data-stu-id="d5ff5-183">S mode configuration.</span></span> <span data-ttu-id="d5ff5-184">可能な値は、`noRestriction`、`block`、`unlock` です。</span><span class="sxs-lookup"><span data-stu-id="d5ff5-184">Possible values are: `noRestriction`, `block`, `unlock`.</span></span>|



## <a name="response"></a><span data-ttu-id="d5ff5-185">応答</span><span class="sxs-lookup"><span data-stu-id="d5ff5-185">Response</span></span>
<span data-ttu-id="d5ff5-186">このメソッドが成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d5ff5-186">If successful, this method returns a `200 OK` response code and an updated [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5ff5-187">例</span><span class="sxs-lookup"><span data-stu-id="d5ff5-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5ff5-188">要求</span><span class="sxs-lookup"><span data-stu-id="d5ff5-188">Request</span></span>
<span data-ttu-id="d5ff5-189">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d5ff5-189">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 431

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="d5ff5-190">応答</span><span class="sxs-lookup"><span data-stu-id="d5ff5-190">Response</span></span>
<span data-ttu-id="d5ff5-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d5ff5-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 603

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "id": "f39fc471-c471-f39f-71c4-9ff371c49ff3",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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




