---
title: settingStateDeviceSummary の作成
description: 新しい settingStateDeviceSummary オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 44cb33bd0445586ead64c5101c297b7a27351344
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333370"
---
# <a name="create-settingstatedevicesummary"></a><span data-ttu-id="d1a5e-103">settingStateDeviceSummary の作成</span><span class="sxs-lookup"><span data-stu-id="d1a5e-103">Create settingStateDeviceSummary</span></span>

> <span data-ttu-id="d1a5e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d1a5e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d1a5e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1a5e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d1a5e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d1a5e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d1a5e-107">新しい [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d1a5e-107">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d1a5e-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="d1a5e-108">Prerequisites</span></span>
<span data-ttu-id="d1a5e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d1a5e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1a5e-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d1a5e-111">Permission type</span></span>|<span data-ttu-id="d1a5e-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d1a5e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1a5e-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d1a5e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d1a5e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1a5e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d1a5e-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d1a5e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1a5e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1a5e-116">Not supported.</span></span>|
|<span data-ttu-id="d1a5e-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d1a5e-117">Application</span></span>|<span data-ttu-id="d1a5e-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1a5e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1a5e-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d1a5e-119">HTTP Request</span></span>
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
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="d1a5e-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d1a5e-120">Request headers</span></span>
|<span data-ttu-id="d1a5e-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d1a5e-121">Header</span></span>|<span data-ttu-id="d1a5e-122">値</span><span class="sxs-lookup"><span data-stu-id="d1a5e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1a5e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1a5e-123">Authorization</span></span>|<span data-ttu-id="d1a5e-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d1a5e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1a5e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d1a5e-125">Accept</span></span>|<span data-ttu-id="d1a5e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d1a5e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1a5e-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="d1a5e-127">Request body</span></span>
<span data-ttu-id="d1a5e-128">要求本文で、settingStateDeviceSummary オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d1a5e-128">In the request body, supply a JSON representation for the settingStateDeviceSummary object.</span></span>

<span data-ttu-id="d1a5e-129">次の表に、settingStateDeviceSummary の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d1a5e-129">The following table shows the properties that are required when you create the settingStateDeviceSummary.</span></span>

|<span data-ttu-id="d1a5e-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d1a5e-130">Property</span></span>|<span data-ttu-id="d1a5e-131">種類</span><span class="sxs-lookup"><span data-stu-id="d1a5e-131">Type</span></span>|<span data-ttu-id="d1a5e-132">説明</span><span class="sxs-lookup"><span data-stu-id="d1a5e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1a5e-133">ID</span><span class="sxs-lookup"><span data-stu-id="d1a5e-133">id</span></span>|<span data-ttu-id="d1a5e-134">String</span><span class="sxs-lookup"><span data-stu-id="d1a5e-134">String</span></span>|<span data-ttu-id="d1a5e-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d1a5e-135">Key of the entity.</span></span>|
|<span data-ttu-id="d1a5e-136">settingName</span><span class="sxs-lookup"><span data-stu-id="d1a5e-136">settingName</span></span>|<span data-ttu-id="d1a5e-137">String</span><span class="sxs-lookup"><span data-stu-id="d1a5e-137">String</span></span>|<span data-ttu-id="d1a5e-138">設定の名前</span><span class="sxs-lookup"><span data-stu-id="d1a5e-138">Name of the setting</span></span>|
|<span data-ttu-id="d1a5e-139">instancePath</span><span class="sxs-lookup"><span data-stu-id="d1a5e-139">instancePath</span></span>|<span data-ttu-id="d1a5e-140">String</span><span class="sxs-lookup"><span data-stu-id="d1a5e-140">String</span></span>|<span data-ttu-id="d1a5e-141">設定の InstancePath の名前</span><span class="sxs-lookup"><span data-stu-id="d1a5e-141">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="d1a5e-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d1a5e-142">unknownDeviceCount</span></span>|<span data-ttu-id="d1a5e-143">Int32</span><span class="sxs-lookup"><span data-stu-id="d1a5e-143">Int32</span></span>|<span data-ttu-id="d1a5e-144">設定の不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d1a5e-144">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="d1a5e-145">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d1a5e-145">notApplicableDeviceCount</span></span>|<span data-ttu-id="d1a5e-146">Int32</span><span class="sxs-lookup"><span data-stu-id="d1a5e-146">Int32</span></span>|<span data-ttu-id="d1a5e-147">設定の該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d1a5e-147">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="d1a5e-148">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d1a5e-148">compliantDeviceCount</span></span>|<span data-ttu-id="d1a5e-149">Int32</span><span class="sxs-lookup"><span data-stu-id="d1a5e-149">Int32</span></span>|<span data-ttu-id="d1a5e-150">設定の準拠しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d1a5e-150">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="d1a5e-151">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d1a5e-151">remediatedDeviceCount</span></span>|<span data-ttu-id="d1a5e-152">Int32</span><span class="sxs-lookup"><span data-stu-id="d1a5e-152">Int32</span></span>|<span data-ttu-id="d1a5e-153">設定の準拠しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d1a5e-153">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="d1a5e-154">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d1a5e-154">nonCompliantDeviceCount</span></span>|<span data-ttu-id="d1a5e-155">Int32</span><span class="sxs-lookup"><span data-stu-id="d1a5e-155">Int32</span></span>|<span data-ttu-id="d1a5e-156">設定の準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d1a5e-156">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="d1a5e-157">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d1a5e-157">errorDeviceCount</span></span>|<span data-ttu-id="d1a5e-158">Int32</span><span class="sxs-lookup"><span data-stu-id="d1a5e-158">Int32</span></span>|<span data-ttu-id="d1a5e-159">設定のデバイス エラーの数</span><span class="sxs-lookup"><span data-stu-id="d1a5e-159">Device error count for the setting</span></span>|
|<span data-ttu-id="d1a5e-160">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d1a5e-160">conflictDeviceCount</span></span>|<span data-ttu-id="d1a5e-161">Int32</span><span class="sxs-lookup"><span data-stu-id="d1a5e-161">Int32</span></span>|<span data-ttu-id="d1a5e-162">設定のデバイス競合エラーの数</span><span class="sxs-lookup"><span data-stu-id="d1a5e-162">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="d1a5e-163">応答</span><span class="sxs-lookup"><span data-stu-id="d1a5e-163">Response</span></span>
<span data-ttu-id="d1a5e-164">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d1a5e-164">If successful, this method returns a `201 Created` response code and a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1a5e-165">例</span><span class="sxs-lookup"><span data-stu-id="d1a5e-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="d1a5e-166">要求</span><span class="sxs-lookup"><span data-stu-id="d1a5e-166">Request</span></span>
<span data-ttu-id="d1a5e-167">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d1a5e-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d1a5e-168">応答</span><span class="sxs-lookup"><span data-stu-id="d1a5e-168">Response</span></span>
<span data-ttu-id="d1a5e-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d1a5e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




