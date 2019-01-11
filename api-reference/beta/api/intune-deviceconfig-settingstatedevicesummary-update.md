---
title: settingStateDeviceSummary の更新
description: settingStateDeviceSummary オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: dad14281e638a65c6886d7e92e10dd7bcfc54a22
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842925"
---
# <a name="update-settingstatedevicesummary"></a><span data-ttu-id="b4015-103">settingStateDeviceSummary の更新</span><span class="sxs-lookup"><span data-stu-id="b4015-103">Update settingStateDeviceSummary</span></span>

> <span data-ttu-id="b4015-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b4015-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b4015-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b4015-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b4015-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b4015-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b4015-107">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b4015-107">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b4015-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="b4015-108">Prerequisites</span></span>
<span data-ttu-id="b4015-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b4015-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4015-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b4015-111">Permission type</span></span>|<span data-ttu-id="b4015-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b4015-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4015-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b4015-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b4015-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4015-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b4015-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b4015-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4015-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b4015-116">Not supported.</span></span>|
|<span data-ttu-id="b4015-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b4015-117">Application</span></span>|<span data-ttu-id="b4015-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b4015-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4015-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b4015-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="b4015-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b4015-120">Request headers</span></span>
|<span data-ttu-id="b4015-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b4015-121">Header</span></span>|<span data-ttu-id="b4015-122">値</span><span class="sxs-lookup"><span data-stu-id="b4015-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4015-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4015-123">Authorization</span></span>|<span data-ttu-id="b4015-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b4015-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4015-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b4015-125">Accept</span></span>|<span data-ttu-id="b4015-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b4015-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4015-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b4015-127">Request body</span></span>
<span data-ttu-id="b4015-128">要求本文で、[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b4015-128">In the request body, supply a JSON representation for the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

<span data-ttu-id="b4015-129">次の表に、[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b4015-129">The following table shows the properties that are required when you create the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>

|<span data-ttu-id="b4015-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b4015-130">Property</span></span>|<span data-ttu-id="b4015-131">種類</span><span class="sxs-lookup"><span data-stu-id="b4015-131">Type</span></span>|<span data-ttu-id="b4015-132">説明</span><span class="sxs-lookup"><span data-stu-id="b4015-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4015-133">ID</span><span class="sxs-lookup"><span data-stu-id="b4015-133">id</span></span>|<span data-ttu-id="b4015-134">String</span><span class="sxs-lookup"><span data-stu-id="b4015-134">String</span></span>|<span data-ttu-id="b4015-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b4015-135">Key of the entity.</span></span>|
|<span data-ttu-id="b4015-136">settingName</span><span class="sxs-lookup"><span data-stu-id="b4015-136">settingName</span></span>|<span data-ttu-id="b4015-137">String</span><span class="sxs-lookup"><span data-stu-id="b4015-137">String</span></span>|<span data-ttu-id="b4015-138">設定の名前</span><span class="sxs-lookup"><span data-stu-id="b4015-138">Name of the setting</span></span>|
|<span data-ttu-id="b4015-139">instancePath</span><span class="sxs-lookup"><span data-stu-id="b4015-139">instancePath</span></span>|<span data-ttu-id="b4015-140">String</span><span class="sxs-lookup"><span data-stu-id="b4015-140">String</span></span>|<span data-ttu-id="b4015-141">設定の InstancePath の名前</span><span class="sxs-lookup"><span data-stu-id="b4015-141">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="b4015-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b4015-142">unknownDeviceCount</span></span>|<span data-ttu-id="b4015-143">Int32</span><span class="sxs-lookup"><span data-stu-id="b4015-143">Int32</span></span>|<span data-ttu-id="b4015-144">設定の不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="b4015-144">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="b4015-145">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b4015-145">notApplicableDeviceCount</span></span>|<span data-ttu-id="b4015-146">Int32</span><span class="sxs-lookup"><span data-stu-id="b4015-146">Int32</span></span>|<span data-ttu-id="b4015-147">設定の該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="b4015-147">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="b4015-148">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b4015-148">compliantDeviceCount</span></span>|<span data-ttu-id="b4015-149">Int32</span><span class="sxs-lookup"><span data-stu-id="b4015-149">Int32</span></span>|<span data-ttu-id="b4015-150">設定の準拠しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="b4015-150">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="b4015-151">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b4015-151">remediatedDeviceCount</span></span>|<span data-ttu-id="b4015-152">Int32</span><span class="sxs-lookup"><span data-stu-id="b4015-152">Int32</span></span>|<span data-ttu-id="b4015-153">設定の準拠しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="b4015-153">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="b4015-154">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b4015-154">nonCompliantDeviceCount</span></span>|<span data-ttu-id="b4015-155">Int32</span><span class="sxs-lookup"><span data-stu-id="b4015-155">Int32</span></span>|<span data-ttu-id="b4015-156">設定の準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="b4015-156">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="b4015-157">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b4015-157">errorDeviceCount</span></span>|<span data-ttu-id="b4015-158">Int32</span><span class="sxs-lookup"><span data-stu-id="b4015-158">Int32</span></span>|<span data-ttu-id="b4015-159">設定のデバイス エラーの数</span><span class="sxs-lookup"><span data-stu-id="b4015-159">Device error count for the setting</span></span>|
|<span data-ttu-id="b4015-160">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b4015-160">conflictDeviceCount</span></span>|<span data-ttu-id="b4015-161">Int32</span><span class="sxs-lookup"><span data-stu-id="b4015-161">Int32</span></span>|<span data-ttu-id="b4015-162">設定のデバイス競合エラーの数</span><span class="sxs-lookup"><span data-stu-id="b4015-162">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="b4015-163">応答</span><span class="sxs-lookup"><span data-stu-id="b4015-163">Response</span></span>
<span data-ttu-id="b4015-164">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b4015-164">If successful, this method returns a `200 OK` response code and an updated [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4015-165">例</span><span class="sxs-lookup"><span data-stu-id="b4015-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="b4015-166">要求</span><span class="sxs-lookup"><span data-stu-id="b4015-166">Request</span></span>
<span data-ttu-id="b4015-167">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b4015-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
Content-type: application/json
Content-length: 296

{
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

### <a name="response"></a><span data-ttu-id="b4015-168">応答</span><span class="sxs-lookup"><span data-stu-id="b4015-168">Response</span></span>
<span data-ttu-id="b4015-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b4015-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





