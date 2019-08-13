---
title: settingStateDeviceSummary の作成
description: 新しい settingStateDeviceSummary オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ae0c98b53e2c404f064fd6fe36afb4ae809a70ac
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36345450"
---
# <a name="create-settingstatedevicesummary"></a><span data-ttu-id="ade13-103">settingStateDeviceSummary の作成</span><span class="sxs-lookup"><span data-stu-id="ade13-103">Create settingStateDeviceSummary</span></span>

> <span data-ttu-id="ade13-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ade13-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ade13-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ade13-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ade13-106">新しい [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ade13-106">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ade13-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="ade13-107">Prerequisites</span></span>
<span data-ttu-id="ade13-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ade13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ade13-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ade13-110">Permission type</span></span>|<span data-ttu-id="ade13-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ade13-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ade13-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ade13-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ade13-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ade13-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ade13-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ade13-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ade13-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ade13-115">Not supported.</span></span>|
|<span data-ttu-id="ade13-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ade13-116">Application</span></span>|<span data-ttu-id="ade13-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ade13-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ade13-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ade13-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerCertificateProfileBase/rootCertificate/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="ade13-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ade13-119">Request headers</span></span>
|<span data-ttu-id="ade13-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ade13-120">Header</span></span>|<span data-ttu-id="ade13-121">値</span><span class="sxs-lookup"><span data-stu-id="ade13-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ade13-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ade13-122">Authorization</span></span>|<span data-ttu-id="ade13-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ade13-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ade13-124">承諾</span><span class="sxs-lookup"><span data-stu-id="ade13-124">Accept</span></span>|<span data-ttu-id="ade13-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ade13-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ade13-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ade13-126">Request body</span></span>
<span data-ttu-id="ade13-127">要求本文で、settingStateDeviceSummary オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ade13-127">In the request body, supply a JSON representation for the settingStateDeviceSummary object.</span></span>

<span data-ttu-id="ade13-128">次の表に、settingStateDeviceSummary の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ade13-128">The following table shows the properties that are required when you create the settingStateDeviceSummary.</span></span>

|<span data-ttu-id="ade13-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ade13-129">Property</span></span>|<span data-ttu-id="ade13-130">型</span><span class="sxs-lookup"><span data-stu-id="ade13-130">Type</span></span>|<span data-ttu-id="ade13-131">説明</span><span class="sxs-lookup"><span data-stu-id="ade13-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ade13-132">id</span><span class="sxs-lookup"><span data-stu-id="ade13-132">id</span></span>|<span data-ttu-id="ade13-133">String</span><span class="sxs-lookup"><span data-stu-id="ade13-133">String</span></span>|<span data-ttu-id="ade13-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ade13-134">Key of the entity.</span></span>|
|<span data-ttu-id="ade13-135">settingName</span><span class="sxs-lookup"><span data-stu-id="ade13-135">settingName</span></span>|<span data-ttu-id="ade13-136">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="ade13-136">String</span></span>|<span data-ttu-id="ade13-137">設定の名前</span><span class="sxs-lookup"><span data-stu-id="ade13-137">Name of the setting</span></span>|
|<span data-ttu-id="ade13-138">instancePath</span><span class="sxs-lookup"><span data-stu-id="ade13-138">instancePath</span></span>|<span data-ttu-id="ade13-139">String</span><span class="sxs-lookup"><span data-stu-id="ade13-139">String</span></span>|<span data-ttu-id="ade13-140">設定の InstancePath の名前</span><span class="sxs-lookup"><span data-stu-id="ade13-140">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="ade13-141">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ade13-141">unknownDeviceCount</span></span>|<span data-ttu-id="ade13-142">Int32</span><span class="sxs-lookup"><span data-stu-id="ade13-142">Int32</span></span>|<span data-ttu-id="ade13-143">設定の不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="ade13-143">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="ade13-144">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ade13-144">notApplicableDeviceCount</span></span>|<span data-ttu-id="ade13-145">Int32</span><span class="sxs-lookup"><span data-stu-id="ade13-145">Int32</span></span>|<span data-ttu-id="ade13-146">設定の該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="ade13-146">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="ade13-147">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ade13-147">compliantDeviceCount</span></span>|<span data-ttu-id="ade13-148">Int32</span><span class="sxs-lookup"><span data-stu-id="ade13-148">Int32</span></span>|<span data-ttu-id="ade13-149">設定の準拠しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="ade13-149">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="ade13-150">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ade13-150">remediatedDeviceCount</span></span>|<span data-ttu-id="ade13-151">Int32</span><span class="sxs-lookup"><span data-stu-id="ade13-151">Int32</span></span>|<span data-ttu-id="ade13-152">設定の準拠しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="ade13-152">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="ade13-153">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ade13-153">nonCompliantDeviceCount</span></span>|<span data-ttu-id="ade13-154">Int32</span><span class="sxs-lookup"><span data-stu-id="ade13-154">Int32</span></span>|<span data-ttu-id="ade13-155">設定の準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="ade13-155">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="ade13-156">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ade13-156">errorDeviceCount</span></span>|<span data-ttu-id="ade13-157">Int32</span><span class="sxs-lookup"><span data-stu-id="ade13-157">Int32</span></span>|<span data-ttu-id="ade13-158">設定のデバイス エラーの数</span><span class="sxs-lookup"><span data-stu-id="ade13-158">Device error count for the setting</span></span>|
|<span data-ttu-id="ade13-159">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ade13-159">conflictDeviceCount</span></span>|<span data-ttu-id="ade13-160">Int32</span><span class="sxs-lookup"><span data-stu-id="ade13-160">Int32</span></span>|<span data-ttu-id="ade13-161">設定のデバイス競合エラーの数</span><span class="sxs-lookup"><span data-stu-id="ade13-161">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="ade13-162">応答</span><span class="sxs-lookup"><span data-stu-id="ade13-162">Response</span></span>
<span data-ttu-id="ade13-163">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ade13-163">If successful, this method returns a `201 Created` response code and a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ade13-164">例</span><span class="sxs-lookup"><span data-stu-id="ade13-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="ade13-165">要求</span><span class="sxs-lookup"><span data-stu-id="ade13-165">Request</span></span>
<span data-ttu-id="ade13-166">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ade13-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
Content-type: application/json
Content-length: 360

{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "settingName": "Setting Name value",
  "instancePath": "Instance Path value",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="ade13-167">応答</span><span class="sxs-lookup"><span data-stu-id="ade13-167">Response</span></span>
<span data-ttu-id="ade13-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ade13-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 409

{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "id": "3e2d4526-4526-3e2d-2645-2d3e26452d3e",
  "settingName": "Setting Name value",
  "instancePath": "Instance Path value",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```






