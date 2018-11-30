---
title: editionUpgradeConfiguration の更新
description: editionUpgradeConfiguration オブジェクトのプロパティを更新します。
ms.openlocfilehash: 81564ae9430566212efcc100de779dc83e9ed664
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023188"
---
# <a name="update-editionupgradeconfiguration"></a><span data-ttu-id="0f58a-103">editionUpgradeConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="0f58a-103">Update editionUpgradeConfiguration</span></span>

> <span data-ttu-id="0f58a-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0f58a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0f58a-105">[editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0f58a-105">Update the properties of a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0f58a-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="0f58a-106">Prerequisites</span></span>
<span data-ttu-id="0f58a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0f58a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f58a-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0f58a-109">Permission type</span></span>|<span data-ttu-id="0f58a-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0f58a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f58a-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0f58a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0f58a-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f58a-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0f58a-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0f58a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f58a-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0f58a-114">Not supported.</span></span>|
|<span data-ttu-id="0f58a-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0f58a-115">Application</span></span>|<span data-ttu-id="0f58a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0f58a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f58a-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0f58a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0f58a-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0f58a-118">Request headers</span></span>
|<span data-ttu-id="0f58a-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0f58a-119">Header</span></span>|<span data-ttu-id="0f58a-120">値</span><span class="sxs-lookup"><span data-stu-id="0f58a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f58a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f58a-121">Authorization</span></span>|<span data-ttu-id="0f58a-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="0f58a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f58a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="0f58a-123">Accept</span></span>|<span data-ttu-id="0f58a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0f58a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f58a-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="0f58a-125">Request body</span></span>
<span data-ttu-id="0f58a-126">要求本文では、[editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0f58a-126">In the request body, supply a JSON representation for the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

<span data-ttu-id="0f58a-127">次の表に、[editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0f58a-127">The following table shows the properties that are required when you create the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span></span>

|<span data-ttu-id="0f58a-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0f58a-128">Property</span></span>|<span data-ttu-id="0f58a-129">型</span><span class="sxs-lookup"><span data-stu-id="0f58a-129">Type</span></span>|<span data-ttu-id="0f58a-130">説明</span><span class="sxs-lookup"><span data-stu-id="0f58a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f58a-131">id</span><span class="sxs-lookup"><span data-stu-id="0f58a-131">id</span></span>|<span data-ttu-id="0f58a-132">String</span><span class="sxs-lookup"><span data-stu-id="0f58a-132">String</span></span>|<span data-ttu-id="0f58a-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0f58a-133">Key of the entity.</span></span> <span data-ttu-id="0f58a-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0f58a-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f58a-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0f58a-135">lastModifiedDateTime</span></span>|<span data-ttu-id="0f58a-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f58a-136">DateTimeOffset</span></span>|<span data-ttu-id="0f58a-137">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="0f58a-137">DateTime the object was last modified.</span></span> <span data-ttu-id="0f58a-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0f58a-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f58a-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0f58a-139">createdDateTime</span></span>|<span data-ttu-id="0f58a-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f58a-140">DateTimeOffset</span></span>|<span data-ttu-id="0f58a-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="0f58a-141">DateTime the object was created.</span></span> <span data-ttu-id="0f58a-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0f58a-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f58a-143">説明</span><span class="sxs-lookup"><span data-stu-id="0f58a-143">description</span></span>|<span data-ttu-id="0f58a-144">String</span><span class="sxs-lookup"><span data-stu-id="0f58a-144">String</span></span>|<span data-ttu-id="0f58a-145">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="0f58a-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0f58a-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0f58a-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f58a-147">displayName</span><span class="sxs-lookup"><span data-stu-id="0f58a-147">displayName</span></span>|<span data-ttu-id="0f58a-148">String</span><span class="sxs-lookup"><span data-stu-id="0f58a-148">String</span></span>|<span data-ttu-id="0f58a-149">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="0f58a-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0f58a-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0f58a-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f58a-151">version</span><span class="sxs-lookup"><span data-stu-id="0f58a-151">version</span></span>|<span data-ttu-id="0f58a-152">Int32</span><span class="sxs-lookup"><span data-stu-id="0f58a-152">Int32</span></span>|<span data-ttu-id="0f58a-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="0f58a-153">Version of the device configuration.</span></span> <span data-ttu-id="0f58a-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0f58a-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f58a-155">licenseType</span><span class="sxs-lookup"><span data-stu-id="0f58a-155">licenseType</span></span>|[<span data-ttu-id="0f58a-156">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="0f58a-156">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="0f58a-157">エディション アップグレード ライセンスの種類。</span><span class="sxs-lookup"><span data-stu-id="0f58a-157">Edition Upgrade License Type.</span></span> <span data-ttu-id="0f58a-158">可能な値は、`productKey`、`licenseFile` です。</span><span class="sxs-lookup"><span data-stu-id="0f58a-158">Possible values are: `productKey`, `licenseFile`.</span></span>|
|<span data-ttu-id="0f58a-159">targetEdition</span><span class="sxs-lookup"><span data-stu-id="0f58a-159">targetEdition</span></span>|[<span data-ttu-id="0f58a-160">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="0f58a-160">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="0f58a-161">エディション アップグレードの対象エディション。</span><span class="sxs-lookup"><span data-stu-id="0f58a-161">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="0f58a-162">可能な値は、`windows10Enterprise`、`windows10EnterpriseN`、`windows10Education`、`windows10EducationN`、`windows10MobileEnterprise`、`windows10HolographicEnterprise`、`windows10Professional`、`windows10ProfessionalN`、`windows10ProfessionalEducation`、`windows10ProfessionalEducationN`、`windows10ProfessionalWorkstation`、`windows10ProfessionalWorkstationN` です。</span><span class="sxs-lookup"><span data-stu-id="0f58a-162">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span></span>|
|<span data-ttu-id="0f58a-163">license</span><span class="sxs-lookup"><span data-stu-id="0f58a-163">license</span></span>|<span data-ttu-id="0f58a-164">String</span><span class="sxs-lookup"><span data-stu-id="0f58a-164">String</span></span>|<span data-ttu-id="0f58a-165">エディション アップグレード ライセンスのファイル コンテンツ。</span><span class="sxs-lookup"><span data-stu-id="0f58a-165">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="0f58a-166">productKey</span><span class="sxs-lookup"><span data-stu-id="0f58a-166">productKey</span></span>|<span data-ttu-id="0f58a-167">String</span><span class="sxs-lookup"><span data-stu-id="0f58a-167">String</span></span>|<span data-ttu-id="0f58a-168">エディション アップグレードのプロダクト キー。</span><span class="sxs-lookup"><span data-stu-id="0f58a-168">Edition Upgrade Product Key.</span></span>|



## <a name="response"></a><span data-ttu-id="0f58a-169">応答</span><span class="sxs-lookup"><span data-stu-id="0f58a-169">Response</span></span>
<span data-ttu-id="0f58a-170">このメソッドが成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0f58a-170">If successful, this method returns a `200 OK` response code and an updated [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f58a-171">例</span><span class="sxs-lookup"><span data-stu-id="0f58a-171">Example</span></span>
### <a name="request"></a><span data-ttu-id="0f58a-172">要求</span><span class="sxs-lookup"><span data-stu-id="0f58a-172">Request</span></span>
<span data-ttu-id="0f58a-173">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0f58a-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 311

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "licenseType": "licenseFile",
  "targetEdition": "windows10EnterpriseN",
  "license": "License value",
  "productKey": "Product Key value"
}
```

### <a name="response"></a><span data-ttu-id="0f58a-174">応答</span><span class="sxs-lookup"><span data-stu-id="0f58a-174">Response</span></span>
<span data-ttu-id="0f58a-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0f58a-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 483

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "id": "f39fc471-c471-f39f-71c4-9ff371c49ff3",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "licenseType": "licenseFile",
  "targetEdition": "windows10EnterpriseN",
  "license": "License value",
  "productKey": "Product Key value"
}
```



