---
title: deviceConfigurationDeviceStatus の更新
description: deviceConfigurationDeviceStatus オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 70c80bb2c39139f07333a0d7a0ba9b2e37b6d9fe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858353"
---
# <a name="update-deviceconfigurationdevicestatus"></a><span data-ttu-id="fb08a-103">deviceConfigurationDeviceStatus の更新</span><span class="sxs-lookup"><span data-stu-id="fb08a-103">Update deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="fb08a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fb08a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fb08a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fb08a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fb08a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fb08a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fb08a-107">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="fb08a-107">Update the properties of a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fb08a-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="fb08a-108">Prerequisites</span></span>
<span data-ttu-id="fb08a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fb08a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb08a-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fb08a-111">Permission type</span></span>|<span data-ttu-id="fb08a-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fb08a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb08a-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fb08a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fb08a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb08a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fb08a-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fb08a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb08a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fb08a-116">Not supported.</span></span>|
|<span data-ttu-id="fb08a-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fb08a-117">Application</span></span>|<span data-ttu-id="fb08a-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fb08a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb08a-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fb08a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="fb08a-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fb08a-120">Request headers</span></span>
|<span data-ttu-id="fb08a-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fb08a-121">Header</span></span>|<span data-ttu-id="fb08a-122">値</span><span class="sxs-lookup"><span data-stu-id="fb08a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb08a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb08a-123">Authorization</span></span>|<span data-ttu-id="fb08a-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="fb08a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb08a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fb08a-125">Accept</span></span>|<span data-ttu-id="fb08a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fb08a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb08a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="fb08a-127">Request body</span></span>
<span data-ttu-id="fb08a-128">要求本文で、[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="fb08a-128">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

<span data-ttu-id="fb08a-129">次の表に、[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="fb08a-129">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span></span>

|<span data-ttu-id="fb08a-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fb08a-130">Property</span></span>|<span data-ttu-id="fb08a-131">種類</span><span class="sxs-lookup"><span data-stu-id="fb08a-131">Type</span></span>|<span data-ttu-id="fb08a-132">説明</span><span class="sxs-lookup"><span data-stu-id="fb08a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb08a-133">ID</span><span class="sxs-lookup"><span data-stu-id="fb08a-133">id</span></span>|<span data-ttu-id="fb08a-134">String</span><span class="sxs-lookup"><span data-stu-id="fb08a-134">String</span></span>|<span data-ttu-id="fb08a-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="fb08a-135">Key of the entity.</span></span>|
|<span data-ttu-id="fb08a-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="fb08a-136">deviceDisplayName</span></span>|<span data-ttu-id="fb08a-137">String</span><span class="sxs-lookup"><span data-stu-id="fb08a-137">String</span></span>|<span data-ttu-id="fb08a-138">DevicePolicyStatus のデバイス名。</span><span class="sxs-lookup"><span data-stu-id="fb08a-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="fb08a-139">userName</span><span class="sxs-lookup"><span data-stu-id="fb08a-139">userName</span></span>|<span data-ttu-id="fb08a-140">String</span><span class="sxs-lookup"><span data-stu-id="fb08a-140">String</span></span>|<span data-ttu-id="fb08a-141">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="fb08a-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="fb08a-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="fb08a-142">deviceModel</span></span>|<span data-ttu-id="fb08a-143">String</span><span class="sxs-lookup"><span data-stu-id="fb08a-143">String</span></span>|<span data-ttu-id="fb08a-144">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="fb08a-144">The device model that is being reported</span></span>|
|<span data-ttu-id="fb08a-145">platform</span><span class="sxs-lookup"><span data-stu-id="fb08a-145">platform</span></span>|<span data-ttu-id="fb08a-146">Int32</span><span class="sxs-lookup"><span data-stu-id="fb08a-146">Int32</span></span>|<span data-ttu-id="fb08a-147">報告されているデバイスのプラットフォーム</span><span class="sxs-lookup"><span data-stu-id="fb08a-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="fb08a-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="fb08a-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="fb08a-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb08a-149">DateTimeOffset</span></span>|<span data-ttu-id="fb08a-150">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="fb08a-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="fb08a-151">status</span><span class="sxs-lookup"><span data-stu-id="fb08a-151">status</span></span>|[<span data-ttu-id="fb08a-152">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="fb08a-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="fb08a-153">ポリシー レポートのコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="fb08a-153">Compliance status of the policy report.</span></span> <span data-ttu-id="fb08a-154">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="fb08a-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="fb08a-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="fb08a-155">lastReportedDateTime</span></span>|<span data-ttu-id="fb08a-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb08a-156">DateTimeOffset</span></span>|<span data-ttu-id="fb08a-157">ポリシー レポートの最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="fb08a-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="fb08a-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fb08a-158">userPrincipalName</span></span>|<span data-ttu-id="fb08a-159">String</span><span class="sxs-lookup"><span data-stu-id="fb08a-159">String</span></span>|<span data-ttu-id="fb08a-160">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="fb08a-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="fb08a-161">応答</span><span class="sxs-lookup"><span data-stu-id="fb08a-161">Response</span></span>
<span data-ttu-id="fb08a-162">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="fb08a-162">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb08a-163">例</span><span class="sxs-lookup"><span data-stu-id="fb08a-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="fb08a-164">要求</span><span class="sxs-lookup"><span data-stu-id="fb08a-164">Request</span></span>
<span data-ttu-id="fb08a-165">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fb08a-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
Content-type: application/json
Content-length: 377

{
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "platform": 8,
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="fb08a-166">応答</span><span class="sxs-lookup"><span data-stu-id="fb08a-166">Response</span></span>
<span data-ttu-id="fb08a-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fb08a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 496

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "id": "674e98e5-98e5-674e-e598-4e67e5984e67",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "platform": 8,
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```





