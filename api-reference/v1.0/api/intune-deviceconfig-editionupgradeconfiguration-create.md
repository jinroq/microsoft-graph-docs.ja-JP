---
title: editionUpgradeConfiguration の作成
description: 新しい editionUpgradeConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 18349354e899b85cfb34975e899333c679c15c08
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32578898"
---
# <a name="create-editionupgradeconfiguration"></a><span data-ttu-id="a65fd-103">editionUpgradeConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="a65fd-103">Create editionUpgradeConfiguration</span></span>

> <span data-ttu-id="a65fd-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a65fd-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a65fd-105">新しい [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a65fd-105">Create a new [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a65fd-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="a65fd-106">Prerequisites</span></span>
<span data-ttu-id="a65fd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a65fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a65fd-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a65fd-109">Permission type</span></span>|<span data-ttu-id="a65fd-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a65fd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a65fd-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a65fd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a65fd-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a65fd-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a65fd-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a65fd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a65fd-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a65fd-114">Not supported.</span></span>|
|<span data-ttu-id="a65fd-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a65fd-115">Application</span></span>|<span data-ttu-id="a65fd-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a65fd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a65fd-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a65fd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a65fd-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a65fd-118">Request headers</span></span>
|<span data-ttu-id="a65fd-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a65fd-119">Header</span></span>|<span data-ttu-id="a65fd-120">値</span><span class="sxs-lookup"><span data-stu-id="a65fd-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a65fd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a65fd-121">Authorization</span></span>|<span data-ttu-id="a65fd-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a65fd-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a65fd-123">承諾</span><span class="sxs-lookup"><span data-stu-id="a65fd-123">Accept</span></span>|<span data-ttu-id="a65fd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a65fd-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a65fd-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a65fd-125">Request body</span></span>
<span data-ttu-id="a65fd-126">要求本文では、editionUpgradeConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a65fd-126">In the request body, supply a JSON representation for the editionUpgradeConfiguration object.</span></span>

<span data-ttu-id="a65fd-127">次の表に、editionUpgradeConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a65fd-127">The following table shows the properties that are required when you create the editionUpgradeConfiguration.</span></span>

|<span data-ttu-id="a65fd-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a65fd-128">Property</span></span>|<span data-ttu-id="a65fd-129">型</span><span class="sxs-lookup"><span data-stu-id="a65fd-129">Type</span></span>|<span data-ttu-id="a65fd-130">説明</span><span class="sxs-lookup"><span data-stu-id="a65fd-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a65fd-131">id</span><span class="sxs-lookup"><span data-stu-id="a65fd-131">id</span></span>|<span data-ttu-id="a65fd-132">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="a65fd-132">String</span></span>|<span data-ttu-id="a65fd-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a65fd-133">Key of the entity.</span></span> <span data-ttu-id="a65fd-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a65fd-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a65fd-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a65fd-135">lastModifiedDateTime</span></span>|<span data-ttu-id="a65fd-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a65fd-136">DateTimeOffset</span></span>|<span data-ttu-id="a65fd-137">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="a65fd-137">DateTime the object was last modified.</span></span> <span data-ttu-id="a65fd-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a65fd-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a65fd-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a65fd-139">createdDateTime</span></span>|<span data-ttu-id="a65fd-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a65fd-140">DateTimeOffset</span></span>|<span data-ttu-id="a65fd-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="a65fd-141">DateTime the object was created.</span></span> <span data-ttu-id="a65fd-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a65fd-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a65fd-143">説明</span><span class="sxs-lookup"><span data-stu-id="a65fd-143">description</span></span>|<span data-ttu-id="a65fd-144">String</span><span class="sxs-lookup"><span data-stu-id="a65fd-144">String</span></span>|<span data-ttu-id="a65fd-145">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="a65fd-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a65fd-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a65fd-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a65fd-147">displayName</span><span class="sxs-lookup"><span data-stu-id="a65fd-147">displayName</span></span>|<span data-ttu-id="a65fd-148">String</span><span class="sxs-lookup"><span data-stu-id="a65fd-148">String</span></span>|<span data-ttu-id="a65fd-149">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="a65fd-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a65fd-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a65fd-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a65fd-151">version</span><span class="sxs-lookup"><span data-stu-id="a65fd-151">version</span></span>|<span data-ttu-id="a65fd-152">Int32</span><span class="sxs-lookup"><span data-stu-id="a65fd-152">Int32</span></span>|<span data-ttu-id="a65fd-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="a65fd-153">Version of the device configuration.</span></span> <span data-ttu-id="a65fd-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a65fd-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a65fd-155">licenseType</span><span class="sxs-lookup"><span data-stu-id="a65fd-155">licenseType</span></span>|[<span data-ttu-id="a65fd-156">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="a65fd-156">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="a65fd-157">エディション アップグレード ライセンスの種類。</span><span class="sxs-lookup"><span data-stu-id="a65fd-157">Edition Upgrade License Type.</span></span> <span data-ttu-id="a65fd-158">可能な値は、`productKey`、`licenseFile` です。</span><span class="sxs-lookup"><span data-stu-id="a65fd-158">Possible values are: `productKey`, `licenseFile`.</span></span>|
|<span data-ttu-id="a65fd-159">targetEdition</span><span class="sxs-lookup"><span data-stu-id="a65fd-159">targetEdition</span></span>|[<span data-ttu-id="a65fd-160">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="a65fd-160">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="a65fd-161">エディション アップグレードの対象エディション。</span><span class="sxs-lookup"><span data-stu-id="a65fd-161">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="a65fd-162">可能な値は、`windows10Enterprise`、`windows10EnterpriseN`、`windows10Education`、`windows10EducationN`、`windows10MobileEnterprise`、`windows10HolographicEnterprise`、`windows10Professional`、`windows10ProfessionalN`、`windows10ProfessionalEducation`、`windows10ProfessionalEducationN`、`windows10ProfessionalWorkstation`、`windows10ProfessionalWorkstationN` です。</span><span class="sxs-lookup"><span data-stu-id="a65fd-162">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span></span>|
|<span data-ttu-id="a65fd-163">license</span><span class="sxs-lookup"><span data-stu-id="a65fd-163">license</span></span>|<span data-ttu-id="a65fd-164">String</span><span class="sxs-lookup"><span data-stu-id="a65fd-164">String</span></span>|<span data-ttu-id="a65fd-165">エディション アップグレード ライセンスのファイル コンテンツ。</span><span class="sxs-lookup"><span data-stu-id="a65fd-165">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="a65fd-166">productKey</span><span class="sxs-lookup"><span data-stu-id="a65fd-166">productKey</span></span>|<span data-ttu-id="a65fd-167">String</span><span class="sxs-lookup"><span data-stu-id="a65fd-167">String</span></span>|<span data-ttu-id="a65fd-168">エディション アップグレードのプロダクト キー。</span><span class="sxs-lookup"><span data-stu-id="a65fd-168">Edition Upgrade Product Key.</span></span>|



## <a name="response"></a><span data-ttu-id="a65fd-169">応答</span><span class="sxs-lookup"><span data-stu-id="a65fd-169">Response</span></span>
<span data-ttu-id="a65fd-170">このメソッドが成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a65fd-170">If successful, this method returns a `201 Created` response code and a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a65fd-171">例</span><span class="sxs-lookup"><span data-stu-id="a65fd-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="a65fd-172">要求</span><span class="sxs-lookup"><span data-stu-id="a65fd-172">Request</span></span>
<span data-ttu-id="a65fd-173">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a65fd-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a65fd-174">応答</span><span class="sxs-lookup"><span data-stu-id="a65fd-174">Response</span></span>
<span data-ttu-id="a65fd-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a65fd-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



