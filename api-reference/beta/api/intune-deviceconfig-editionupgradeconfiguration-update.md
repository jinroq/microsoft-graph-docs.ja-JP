---
title: editionUpgradeConfiguration の更新
description: editionUpgradeConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 2ece07f1d0efbcf67f4c28a8fcc3dd2a0b349287
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302115"
---
# <a name="update-editionupgradeconfiguration"></a><span data-ttu-id="6ae17-103">editionUpgradeConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="6ae17-103">Update editionUpgradeConfiguration</span></span>

> <span data-ttu-id="6ae17-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6ae17-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6ae17-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6ae17-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6ae17-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6ae17-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6ae17-107">[editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6ae17-107">Update the properties of a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6ae17-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="6ae17-108">Prerequisites</span></span>
<span data-ttu-id="6ae17-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6ae17-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ae17-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6ae17-111">Permission type</span></span>|<span data-ttu-id="6ae17-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6ae17-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ae17-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6ae17-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6ae17-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ae17-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6ae17-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6ae17-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ae17-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6ae17-116">Not supported.</span></span>|
|<span data-ttu-id="6ae17-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6ae17-117">Application</span></span>|<span data-ttu-id="6ae17-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6ae17-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ae17-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6ae17-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6ae17-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6ae17-120">Request headers</span></span>
|<span data-ttu-id="6ae17-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6ae17-121">Header</span></span>|<span data-ttu-id="6ae17-122">値</span><span class="sxs-lookup"><span data-stu-id="6ae17-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ae17-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ae17-123">Authorization</span></span>|<span data-ttu-id="6ae17-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="6ae17-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ae17-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6ae17-125">Accept</span></span>|<span data-ttu-id="6ae17-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6ae17-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ae17-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="6ae17-127">Request body</span></span>
<span data-ttu-id="6ae17-128">要求本文では、[editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6ae17-128">In the request body, supply a JSON representation for the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

<span data-ttu-id="6ae17-129">次の表に、[editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6ae17-129">The following table shows the properties that are required when you create the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span></span>

|<span data-ttu-id="6ae17-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ae17-130">Property</span></span>|<span data-ttu-id="6ae17-131">種類</span><span class="sxs-lookup"><span data-stu-id="6ae17-131">Type</span></span>|<span data-ttu-id="6ae17-132">説明</span><span class="sxs-lookup"><span data-stu-id="6ae17-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ae17-133">ID</span><span class="sxs-lookup"><span data-stu-id="6ae17-133">id</span></span>|<span data-ttu-id="6ae17-134">String</span><span class="sxs-lookup"><span data-stu-id="6ae17-134">String</span></span>|<span data-ttu-id="6ae17-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6ae17-135">Key of the entity.</span></span> <span data-ttu-id="6ae17-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6ae17-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ae17-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6ae17-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6ae17-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ae17-138">DateTimeOffset</span></span>|<span data-ttu-id="6ae17-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="6ae17-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6ae17-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6ae17-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ae17-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6ae17-141">roleScopeTagIds</span></span>|<span data-ttu-id="6ae17-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="6ae17-142">String collection</span></span>|<span data-ttu-id="6ae17-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="6ae17-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6ae17-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6ae17-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ae17-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6ae17-145">supportsScopeTags</span></span>|<span data-ttu-id="6ae17-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="6ae17-146">Boolean</span></span>|<span data-ttu-id="6ae17-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ae17-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6ae17-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="6ae17-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6ae17-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="6ae17-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6ae17-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="6ae17-150">This property is read-only.</span></span> <span data-ttu-id="6ae17-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6ae17-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ae17-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6ae17-152">createdDateTime</span></span>|<span data-ttu-id="6ae17-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ae17-153">DateTimeOffset</span></span>|<span data-ttu-id="6ae17-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="6ae17-154">DateTime the object was created.</span></span> <span data-ttu-id="6ae17-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6ae17-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ae17-156">説明</span><span class="sxs-lookup"><span data-stu-id="6ae17-156">description</span></span>|<span data-ttu-id="6ae17-157">String</span><span class="sxs-lookup"><span data-stu-id="6ae17-157">String</span></span>|<span data-ttu-id="6ae17-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="6ae17-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6ae17-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6ae17-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ae17-160">displayName</span><span class="sxs-lookup"><span data-stu-id="6ae17-160">displayName</span></span>|<span data-ttu-id="6ae17-161">String</span><span class="sxs-lookup"><span data-stu-id="6ae17-161">String</span></span>|<span data-ttu-id="6ae17-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="6ae17-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6ae17-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6ae17-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ae17-164">version</span><span class="sxs-lookup"><span data-stu-id="6ae17-164">version</span></span>|<span data-ttu-id="6ae17-165">Int32</span><span class="sxs-lookup"><span data-stu-id="6ae17-165">Int32</span></span>|<span data-ttu-id="6ae17-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="6ae17-166">Version of the device configuration.</span></span> <span data-ttu-id="6ae17-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6ae17-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ae17-168">licenseType</span><span class="sxs-lookup"><span data-stu-id="6ae17-168">licenseType</span></span>|[<span data-ttu-id="6ae17-169">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="6ae17-169">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="6ae17-170">エディション アップグレード ライセンスの種類。</span><span class="sxs-lookup"><span data-stu-id="6ae17-170">Edition Upgrade License Type.</span></span> <span data-ttu-id="6ae17-171">可能な値は、`productKey`、`licenseFile`、`notConfigured` です。</span><span class="sxs-lookup"><span data-stu-id="6ae17-171">Possible values are: `productKey`, `licenseFile`, `notConfigured`.</span></span>|
|<span data-ttu-id="6ae17-172">targetEdition</span><span class="sxs-lookup"><span data-stu-id="6ae17-172">targetEdition</span></span>|[<span data-ttu-id="6ae17-173">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="6ae17-173">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="6ae17-174">エディション アップグレードの対象エディション。</span><span class="sxs-lookup"><span data-stu-id="6ae17-174">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="6ae17-175">使用可能な値: `windows10Enterprise`、 `windows10EnterpriseN`、 `windows10Education`、 `windows10EducationN`、 `windows10MobileEnterprise`、 `windows10HolographicEnterprise`、 `windows10Professional`、 `windows10ProfessionalN`、 `windows10ProfessionalEducation`、 `windows10ProfessionalEducationN`、 `windows10ProfessionalWorkstation`、 `windows10ProfessionalWorkstationN`、 `notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="6ae17-175">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`.</span></span>|
|<span data-ttu-id="6ae17-176">license</span><span class="sxs-lookup"><span data-stu-id="6ae17-176">license</span></span>|<span data-ttu-id="6ae17-177">String</span><span class="sxs-lookup"><span data-stu-id="6ae17-177">String</span></span>|<span data-ttu-id="6ae17-178">エディション アップグレード ライセンスのファイル コンテンツ。</span><span class="sxs-lookup"><span data-stu-id="6ae17-178">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="6ae17-179">productKey</span><span class="sxs-lookup"><span data-stu-id="6ae17-179">productKey</span></span>|<span data-ttu-id="6ae17-180">String</span><span class="sxs-lookup"><span data-stu-id="6ae17-180">String</span></span>|<span data-ttu-id="6ae17-181">エディション アップグレードのプロダクト キー。</span><span class="sxs-lookup"><span data-stu-id="6ae17-181">Edition Upgrade Product Key.</span></span>|
|<span data-ttu-id="6ae17-182">windowsSMode</span><span class="sxs-lookup"><span data-stu-id="6ae17-182">windowsSMode</span></span>|[<span data-ttu-id="6ae17-183">windowsSModeConfiguration</span><span class="sxs-lookup"><span data-stu-id="6ae17-183">windowsSModeConfiguration</span></span>](../resources/intune-deviceconfig-windowssmodeconfiguration.md)|<span data-ttu-id="6ae17-184">S モードの設定です。</span><span class="sxs-lookup"><span data-stu-id="6ae17-184">S mode configuration.</span></span> <span data-ttu-id="6ae17-185">可能な値は、`noRestriction`、`block`、`unlock` です。</span><span class="sxs-lookup"><span data-stu-id="6ae17-185">Possible values are: `noRestriction`, `block`, `unlock`.</span></span>|



## <a name="response"></a><span data-ttu-id="6ae17-186">応答</span><span class="sxs-lookup"><span data-stu-id="6ae17-186">Response</span></span>
<span data-ttu-id="6ae17-187">このメソッドが成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6ae17-187">If successful, this method returns a `200 OK` response code and an updated [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ae17-188">例</span><span class="sxs-lookup"><span data-stu-id="6ae17-188">Example</span></span>
### <a name="request"></a><span data-ttu-id="6ae17-189">要求</span><span class="sxs-lookup"><span data-stu-id="6ae17-189">Request</span></span>
<span data-ttu-id="6ae17-190">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6ae17-190">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 429

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="6ae17-191">応答</span><span class="sxs-lookup"><span data-stu-id="6ae17-191">Response</span></span>
<span data-ttu-id="6ae17-p114">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6ae17-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




