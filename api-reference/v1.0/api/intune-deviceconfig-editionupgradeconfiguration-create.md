---
title: editionUpgradeConfiguration の作成
description: 新しい editionUpgradeConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c32873ffe50a4a35f94324d782e055508389e7e4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937923"
---
# <a name="create-editionupgradeconfiguration"></a><span data-ttu-id="51947-103">editionUpgradeConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="51947-103">Create editionUpgradeConfiguration</span></span>

> <span data-ttu-id="51947-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="51947-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51947-105">新しい [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="51947-105">Create a new [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="51947-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="51947-106">Prerequisites</span></span>
<span data-ttu-id="51947-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="51947-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51947-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="51947-109">Permission type</span></span>|<span data-ttu-id="51947-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="51947-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51947-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="51947-111">Delegated (work or school account)</span></span>|<span data-ttu-id="51947-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51947-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="51947-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="51947-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51947-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51947-114">Not supported.</span></span>|
|<span data-ttu-id="51947-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="51947-115">Application</span></span>|<span data-ttu-id="51947-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51947-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51947-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="51947-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="51947-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="51947-118">Request headers</span></span>
|<span data-ttu-id="51947-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="51947-119">Header</span></span>|<span data-ttu-id="51947-120">値</span><span class="sxs-lookup"><span data-stu-id="51947-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51947-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="51947-121">Authorization</span></span>|<span data-ttu-id="51947-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="51947-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51947-123">Accept</span><span class="sxs-lookup"><span data-stu-id="51947-123">Accept</span></span>|<span data-ttu-id="51947-124">application/json</span><span class="sxs-lookup"><span data-stu-id="51947-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51947-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="51947-125">Request body</span></span>
<span data-ttu-id="51947-126">要求本文では、editionUpgradeConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="51947-126">In the request body, supply a JSON representation for the editionUpgradeConfiguration object.</span></span>

<span data-ttu-id="51947-127">次の表に、editionUpgradeConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="51947-127">The following table shows the properties that are required when you create the editionUpgradeConfiguration.</span></span>

|<span data-ttu-id="51947-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="51947-128">Property</span></span>|<span data-ttu-id="51947-129">型</span><span class="sxs-lookup"><span data-stu-id="51947-129">Type</span></span>|<span data-ttu-id="51947-130">説明</span><span class="sxs-lookup"><span data-stu-id="51947-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51947-131">ID</span><span class="sxs-lookup"><span data-stu-id="51947-131">id</span></span>|<span data-ttu-id="51947-132">String</span><span class="sxs-lookup"><span data-stu-id="51947-132">String</span></span>|<span data-ttu-id="51947-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="51947-133">Key of the entity.</span></span> <span data-ttu-id="51947-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51947-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51947-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="51947-135">lastModifiedDateTime</span></span>|<span data-ttu-id="51947-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51947-136">DateTimeOffset</span></span>|<span data-ttu-id="51947-137">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="51947-137">DateTime the object was last modified.</span></span> <span data-ttu-id="51947-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51947-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51947-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="51947-139">createdDateTime</span></span>|<span data-ttu-id="51947-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51947-140">DateTimeOffset</span></span>|<span data-ttu-id="51947-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="51947-141">DateTime the object was created.</span></span> <span data-ttu-id="51947-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51947-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51947-143">説明</span><span class="sxs-lookup"><span data-stu-id="51947-143">description</span></span>|<span data-ttu-id="51947-144">String</span><span class="sxs-lookup"><span data-stu-id="51947-144">String</span></span>|<span data-ttu-id="51947-145">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="51947-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="51947-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51947-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51947-147">displayName</span><span class="sxs-lookup"><span data-stu-id="51947-147">displayName</span></span>|<span data-ttu-id="51947-148">String</span><span class="sxs-lookup"><span data-stu-id="51947-148">String</span></span>|<span data-ttu-id="51947-149">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="51947-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="51947-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51947-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51947-151">version</span><span class="sxs-lookup"><span data-stu-id="51947-151">version</span></span>|<span data-ttu-id="51947-152">Int32</span><span class="sxs-lookup"><span data-stu-id="51947-152">Int32</span></span>|<span data-ttu-id="51947-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="51947-153">Version of the device configuration.</span></span> <span data-ttu-id="51947-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51947-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51947-155">licenseType</span><span class="sxs-lookup"><span data-stu-id="51947-155">licenseType</span></span>|[<span data-ttu-id="51947-156">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="51947-156">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="51947-157">エディション アップグレード ライセンスの種類。</span><span class="sxs-lookup"><span data-stu-id="51947-157">Edition Upgrade License Type.</span></span> <span data-ttu-id="51947-158">可能な値は、`productKey`、`licenseFile` です。</span><span class="sxs-lookup"><span data-stu-id="51947-158">Possible values are: `productKey`, `licenseFile`.</span></span>|
|<span data-ttu-id="51947-159">targetEdition</span><span class="sxs-lookup"><span data-stu-id="51947-159">targetEdition</span></span>|[<span data-ttu-id="51947-160">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="51947-160">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="51947-161">エディション アップグレードの対象エディション。</span><span class="sxs-lookup"><span data-stu-id="51947-161">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="51947-162">可能な値は、`windows10Enterprise`、`windows10EnterpriseN`、`windows10Education`、`windows10EducationN`、`windows10MobileEnterprise`、`windows10HolographicEnterprise`、`windows10Professional`、`windows10ProfessionalN`、`windows10ProfessionalEducation`、`windows10ProfessionalEducationN`、`windows10ProfessionalWorkstation`、`windows10ProfessionalWorkstationN` です。</span><span class="sxs-lookup"><span data-stu-id="51947-162">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span></span>|
|<span data-ttu-id="51947-163">license</span><span class="sxs-lookup"><span data-stu-id="51947-163">license</span></span>|<span data-ttu-id="51947-164">String</span><span class="sxs-lookup"><span data-stu-id="51947-164">String</span></span>|<span data-ttu-id="51947-165">エディション アップグレード ライセンスのファイル コンテンツ。</span><span class="sxs-lookup"><span data-stu-id="51947-165">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="51947-166">productKey</span><span class="sxs-lookup"><span data-stu-id="51947-166">productKey</span></span>|<span data-ttu-id="51947-167">String</span><span class="sxs-lookup"><span data-stu-id="51947-167">String</span></span>|<span data-ttu-id="51947-168">エディション アップグレードのプロダクト キー。</span><span class="sxs-lookup"><span data-stu-id="51947-168">Edition Upgrade Product Key.</span></span>|



## <a name="response"></a><span data-ttu-id="51947-169">応答</span><span class="sxs-lookup"><span data-stu-id="51947-169">Response</span></span>
<span data-ttu-id="51947-170">このメソッドが成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="51947-170">If successful, this method returns a `201 Created` response code and a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51947-171">例</span><span class="sxs-lookup"><span data-stu-id="51947-171">Example</span></span>
### <a name="request"></a><span data-ttu-id="51947-172">要求</span><span class="sxs-lookup"><span data-stu-id="51947-172">Request</span></span>
<span data-ttu-id="51947-173">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="51947-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="51947-174">応答</span><span class="sxs-lookup"><span data-stu-id="51947-174">Response</span></span>
<span data-ttu-id="51947-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="51947-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



