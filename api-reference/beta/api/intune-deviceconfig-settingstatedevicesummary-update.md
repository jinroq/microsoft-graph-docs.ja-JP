---
title: settingStateDeviceSummary の更新
description: settingStateDeviceSummary オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 45a79cb82ad895cd4bda70c9c7d216cb08454590
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36345422"
---
# <a name="update-settingstatedevicesummary"></a><span data-ttu-id="72cae-103">settingStateDeviceSummary の更新</span><span class="sxs-lookup"><span data-stu-id="72cae-103">Update settingStateDeviceSummary</span></span>

> <span data-ttu-id="72cae-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="72cae-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="72cae-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="72cae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72cae-106">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="72cae-106">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="72cae-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="72cae-107">Prerequisites</span></span>
<span data-ttu-id="72cae-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="72cae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72cae-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="72cae-110">Permission type</span></span>|<span data-ttu-id="72cae-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="72cae-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72cae-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="72cae-112">Delegated (work or school account)</span></span>|<span data-ttu-id="72cae-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72cae-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="72cae-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="72cae-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72cae-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="72cae-115">Not supported.</span></span>|
|<span data-ttu-id="72cae-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="72cae-116">Application</span></span>|<span data-ttu-id="72cae-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72cae-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="72cae-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="72cae-118">HTTP Request</span></span>
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
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerCertificateProfileBase/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="72cae-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="72cae-119">Request headers</span></span>
|<span data-ttu-id="72cae-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="72cae-120">Header</span></span>|<span data-ttu-id="72cae-121">値</span><span class="sxs-lookup"><span data-stu-id="72cae-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72cae-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="72cae-122">Authorization</span></span>|<span data-ttu-id="72cae-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="72cae-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72cae-124">承諾</span><span class="sxs-lookup"><span data-stu-id="72cae-124">Accept</span></span>|<span data-ttu-id="72cae-125">application/json</span><span class="sxs-lookup"><span data-stu-id="72cae-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72cae-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="72cae-126">Request body</span></span>
<span data-ttu-id="72cae-127">要求本文で、[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="72cae-127">In the request body, supply a JSON representation for the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

<span data-ttu-id="72cae-128">次の表に、[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="72cae-128">The following table shows the properties that are required when you create the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>

|<span data-ttu-id="72cae-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="72cae-129">Property</span></span>|<span data-ttu-id="72cae-130">型</span><span class="sxs-lookup"><span data-stu-id="72cae-130">Type</span></span>|<span data-ttu-id="72cae-131">説明</span><span class="sxs-lookup"><span data-stu-id="72cae-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72cae-132">id</span><span class="sxs-lookup"><span data-stu-id="72cae-132">id</span></span>|<span data-ttu-id="72cae-133">String</span><span class="sxs-lookup"><span data-stu-id="72cae-133">String</span></span>|<span data-ttu-id="72cae-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="72cae-134">Key of the entity.</span></span>|
|<span data-ttu-id="72cae-135">settingName</span><span class="sxs-lookup"><span data-stu-id="72cae-135">settingName</span></span>|<span data-ttu-id="72cae-136">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="72cae-136">String</span></span>|<span data-ttu-id="72cae-137">設定の名前</span><span class="sxs-lookup"><span data-stu-id="72cae-137">Name of the setting</span></span>|
|<span data-ttu-id="72cae-138">instancePath</span><span class="sxs-lookup"><span data-stu-id="72cae-138">instancePath</span></span>|<span data-ttu-id="72cae-139">String</span><span class="sxs-lookup"><span data-stu-id="72cae-139">String</span></span>|<span data-ttu-id="72cae-140">設定の InstancePath の名前</span><span class="sxs-lookup"><span data-stu-id="72cae-140">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="72cae-141">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="72cae-141">unknownDeviceCount</span></span>|<span data-ttu-id="72cae-142">Int32</span><span class="sxs-lookup"><span data-stu-id="72cae-142">Int32</span></span>|<span data-ttu-id="72cae-143">設定の不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="72cae-143">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="72cae-144">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="72cae-144">notApplicableDeviceCount</span></span>|<span data-ttu-id="72cae-145">Int32</span><span class="sxs-lookup"><span data-stu-id="72cae-145">Int32</span></span>|<span data-ttu-id="72cae-146">設定の該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="72cae-146">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="72cae-147">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="72cae-147">compliantDeviceCount</span></span>|<span data-ttu-id="72cae-148">Int32</span><span class="sxs-lookup"><span data-stu-id="72cae-148">Int32</span></span>|<span data-ttu-id="72cae-149">設定の準拠しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="72cae-149">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="72cae-150">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="72cae-150">remediatedDeviceCount</span></span>|<span data-ttu-id="72cae-151">Int32</span><span class="sxs-lookup"><span data-stu-id="72cae-151">Int32</span></span>|<span data-ttu-id="72cae-152">設定の準拠しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="72cae-152">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="72cae-153">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="72cae-153">nonCompliantDeviceCount</span></span>|<span data-ttu-id="72cae-154">Int32</span><span class="sxs-lookup"><span data-stu-id="72cae-154">Int32</span></span>|<span data-ttu-id="72cae-155">設定の準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="72cae-155">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="72cae-156">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="72cae-156">errorDeviceCount</span></span>|<span data-ttu-id="72cae-157">Int32</span><span class="sxs-lookup"><span data-stu-id="72cae-157">Int32</span></span>|<span data-ttu-id="72cae-158">設定のデバイス エラーの数</span><span class="sxs-lookup"><span data-stu-id="72cae-158">Device error count for the setting</span></span>|
|<span data-ttu-id="72cae-159">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="72cae-159">conflictDeviceCount</span></span>|<span data-ttu-id="72cae-160">Int32</span><span class="sxs-lookup"><span data-stu-id="72cae-160">Int32</span></span>|<span data-ttu-id="72cae-161">設定のデバイス競合エラーの数</span><span class="sxs-lookup"><span data-stu-id="72cae-161">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="72cae-162">応答</span><span class="sxs-lookup"><span data-stu-id="72cae-162">Response</span></span>
<span data-ttu-id="72cae-163">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="72cae-163">If successful, this method returns a `200 OK` response code and an updated [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72cae-164">例</span><span class="sxs-lookup"><span data-stu-id="72cae-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="72cae-165">要求</span><span class="sxs-lookup"><span data-stu-id="72cae-165">Request</span></span>
<span data-ttu-id="72cae-166">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="72cae-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
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

### <a name="response"></a><span data-ttu-id="72cae-167">応答</span><span class="sxs-lookup"><span data-stu-id="72cae-167">Response</span></span>
<span data-ttu-id="72cae-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="72cae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






