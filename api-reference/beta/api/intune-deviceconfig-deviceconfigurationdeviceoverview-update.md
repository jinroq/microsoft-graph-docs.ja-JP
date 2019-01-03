---
title: deviceConfigurationDeviceOverview の更新
description: deviceConfigurationDeviceOverview オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: a6ff0247fbc242aeb230e351e974baaa60f58e55
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308947"
---
# <a name="update-deviceconfigurationdeviceoverview"></a><span data-ttu-id="619be-103">deviceConfigurationDeviceOverview の更新</span><span class="sxs-lookup"><span data-stu-id="619be-103">Update deviceConfigurationDeviceOverview</span></span>

> <span data-ttu-id="619be-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="619be-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="619be-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="619be-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="619be-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="619be-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="619be-107">[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="619be-107">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="619be-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="619be-108">Prerequisites</span></span>
<span data-ttu-id="619be-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="619be-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="619be-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="619be-111">Permission type</span></span>|<span data-ttu-id="619be-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="619be-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="619be-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="619be-113">Delegated (work or school account)</span></span>|<span data-ttu-id="619be-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="619be-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="619be-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="619be-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="619be-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="619be-116">Not supported.</span></span>|
|<span data-ttu-id="619be-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="619be-117">Application</span></span>|<span data-ttu-id="619be-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="619be-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="619be-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="619be-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="619be-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="619be-120">Request headers</span></span>
|<span data-ttu-id="619be-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="619be-121">Header</span></span>|<span data-ttu-id="619be-122">値</span><span class="sxs-lookup"><span data-stu-id="619be-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="619be-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="619be-123">Authorization</span></span>|<span data-ttu-id="619be-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="619be-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="619be-125">Accept</span><span class="sxs-lookup"><span data-stu-id="619be-125">Accept</span></span>|<span data-ttu-id="619be-126">application/json</span><span class="sxs-lookup"><span data-stu-id="619be-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="619be-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="619be-127">Request body</span></span>
<span data-ttu-id="619be-128">要求本文で、[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="619be-128">In the request body, supply a JSON representation for the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

<span data-ttu-id="619be-129">次の表に、[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="619be-129">The following table shows the properties that are required when you create the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span></span>

|<span data-ttu-id="619be-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="619be-130">Property</span></span>|<span data-ttu-id="619be-131">種類</span><span class="sxs-lookup"><span data-stu-id="619be-131">Type</span></span>|<span data-ttu-id="619be-132">説明</span><span class="sxs-lookup"><span data-stu-id="619be-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="619be-133">ID</span><span class="sxs-lookup"><span data-stu-id="619be-133">id</span></span>|<span data-ttu-id="619be-134">String</span><span class="sxs-lookup"><span data-stu-id="619be-134">String</span></span>|<span data-ttu-id="619be-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="619be-135">Key of the entity.</span></span>|
|<span data-ttu-id="619be-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="619be-136">pendingCount</span></span>|<span data-ttu-id="619be-137">Int32</span><span class="sxs-lookup"><span data-stu-id="619be-137">Int32</span></span>|<span data-ttu-id="619be-138">保留中のデバイスの数</span><span class="sxs-lookup"><span data-stu-id="619be-138">Number of pending devices</span></span>|
|<span data-ttu-id="619be-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="619be-139">notApplicableCount</span></span>|<span data-ttu-id="619be-140">Int32</span><span class="sxs-lookup"><span data-stu-id="619be-140">Int32</span></span>|<span data-ttu-id="619be-141">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="619be-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="619be-142">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="619be-142">notApplicablePlatformCount</span></span>|<span data-ttu-id="619be-143">Int32</span><span class="sxs-lookup"><span data-stu-id="619be-143">Int32</span></span>|<span data-ttu-id="619be-144">一致していないプラットフォームとポリシーが適用されないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="619be-144">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="619be-145">successCount</span><span class="sxs-lookup"><span data-stu-id="619be-145">successCount</span></span>|<span data-ttu-id="619be-146">Int32</span><span class="sxs-lookup"><span data-stu-id="619be-146">Int32</span></span>|<span data-ttu-id="619be-147">成功したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="619be-147">Number of succeeded devices</span></span>|
|<span data-ttu-id="619be-148">errorCount</span><span class="sxs-lookup"><span data-stu-id="619be-148">errorCount</span></span>|<span data-ttu-id="619be-149">Int32</span><span class="sxs-lookup"><span data-stu-id="619be-149">Int32</span></span>|<span data-ttu-id="619be-150">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="619be-150">Number of error devices</span></span>|
|<span data-ttu-id="619be-151">failedCount</span><span class="sxs-lookup"><span data-stu-id="619be-151">failedCount</span></span>|<span data-ttu-id="619be-152">Int32</span><span class="sxs-lookup"><span data-stu-id="619be-152">Int32</span></span>|<span data-ttu-id="619be-153">失敗したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="619be-153">Number of failed devices</span></span>|
|<span data-ttu-id="619be-154">conflictCount</span><span class="sxs-lookup"><span data-stu-id="619be-154">conflictCount</span></span>|<span data-ttu-id="619be-155">Int32</span><span class="sxs-lookup"><span data-stu-id="619be-155">Int32</span></span>|<span data-ttu-id="619be-156">競合しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="619be-156">Number of devices in conflict</span></span>|
|<span data-ttu-id="619be-157">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="619be-157">lastUpdateDateTime</span></span>|<span data-ttu-id="619be-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="619be-158">DateTimeOffset</span></span>|<span data-ttu-id="619be-159">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="619be-159">Last update time</span></span>|
|<span data-ttu-id="619be-160">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="619be-160">configurationVersion</span></span>|<span data-ttu-id="619be-161">Int32</span><span class="sxs-lookup"><span data-stu-id="619be-161">Int32</span></span>|<span data-ttu-id="619be-162">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="619be-162">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="619be-163">応答</span><span class="sxs-lookup"><span data-stu-id="619be-163">Response</span></span>
<span data-ttu-id="619be-164">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="619be-164">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="619be-165">例</span><span class="sxs-lookup"><span data-stu-id="619be-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="619be-166">要求</span><span class="sxs-lookup"><span data-stu-id="619be-166">Request</span></span>
<span data-ttu-id="619be-167">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="619be-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
Content-type: application/json
Content-length: 273

{
  "pendingCount": 12,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="619be-168">応答</span><span class="sxs-lookup"><span data-stu-id="619be-168">Response</span></span>
<span data-ttu-id="619be-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="619be-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 394

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
  "id": "62d48e3a-8e3a-62d4-3a8e-d4623a8ed462",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```




