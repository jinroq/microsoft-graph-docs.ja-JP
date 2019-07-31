---
title: deviceConfigurationDeviceStatus の作成
description: 新しい deviceConfigurationDeviceStatus オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1ddb1f14844aa8f805043636bbdbee07db1c4657
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35949147"
---
# <a name="create-deviceconfigurationdevicestatus"></a><span data-ttu-id="855db-103">deviceConfigurationDeviceStatus の作成</span><span class="sxs-lookup"><span data-stu-id="855db-103">Create deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="855db-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="855db-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="855db-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="855db-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="855db-106">新しい [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="855db-106">Create a new [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="855db-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="855db-107">Prerequisites</span></span>
<span data-ttu-id="855db-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="855db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="855db-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="855db-110">Permission type</span></span>|<span data-ttu-id="855db-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="855db-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="855db-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="855db-112">Delegated (work or school account)</span></span>|<span data-ttu-id="855db-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="855db-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="855db-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="855db-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="855db-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="855db-115">Not supported.</span></span>|
|<span data-ttu-id="855db-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="855db-116">Application</span></span>|<span data-ttu-id="855db-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="855db-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="855db-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="855db-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="855db-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="855db-119">Request headers</span></span>
|<span data-ttu-id="855db-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="855db-120">Header</span></span>|<span data-ttu-id="855db-121">値</span><span class="sxs-lookup"><span data-stu-id="855db-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="855db-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="855db-122">Authorization</span></span>|<span data-ttu-id="855db-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="855db-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="855db-124">承諾</span><span class="sxs-lookup"><span data-stu-id="855db-124">Accept</span></span>|<span data-ttu-id="855db-125">application/json</span><span class="sxs-lookup"><span data-stu-id="855db-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="855db-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="855db-126">Request body</span></span>
<span data-ttu-id="855db-127">要求本文で、deviceConfigurationDeviceStatus オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="855db-127">In the request body, supply a JSON representation for the deviceConfigurationDeviceStatus object.</span></span>

<span data-ttu-id="855db-128">次の表に、deviceConfigurationDeviceStatus の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="855db-128">The following table shows the properties that are required when you create the deviceConfigurationDeviceStatus.</span></span>

|<span data-ttu-id="855db-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="855db-129">Property</span></span>|<span data-ttu-id="855db-130">型</span><span class="sxs-lookup"><span data-stu-id="855db-130">Type</span></span>|<span data-ttu-id="855db-131">説明</span><span class="sxs-lookup"><span data-stu-id="855db-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="855db-132">id</span><span class="sxs-lookup"><span data-stu-id="855db-132">id</span></span>|<span data-ttu-id="855db-133">文字列</span><span class="sxs-lookup"><span data-stu-id="855db-133">String</span></span>|<span data-ttu-id="855db-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="855db-134">Key of the entity.</span></span>|
|<span data-ttu-id="855db-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="855db-135">deviceDisplayName</span></span>|<span data-ttu-id="855db-136">String</span><span class="sxs-lookup"><span data-stu-id="855db-136">String</span></span>|<span data-ttu-id="855db-137">DevicePolicyStatus のデバイス名。</span><span class="sxs-lookup"><span data-stu-id="855db-137">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="855db-138">userName</span><span class="sxs-lookup"><span data-stu-id="855db-138">userName</span></span>|<span data-ttu-id="855db-139">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="855db-139">String</span></span>|<span data-ttu-id="855db-140">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="855db-140">The User Name that is being reported</span></span>|
|<span data-ttu-id="855db-141">deviceModel</span><span class="sxs-lookup"><span data-stu-id="855db-141">deviceModel</span></span>|<span data-ttu-id="855db-142">String</span><span class="sxs-lookup"><span data-stu-id="855db-142">String</span></span>|<span data-ttu-id="855db-143">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="855db-143">The device model that is being reported</span></span>|
|<span data-ttu-id="855db-144">platform</span><span class="sxs-lookup"><span data-stu-id="855db-144">platform</span></span>|<span data-ttu-id="855db-145">Int32</span><span class="sxs-lookup"><span data-stu-id="855db-145">Int32</span></span>|<span data-ttu-id="855db-146">レポートされているデバイスのプラットフォーム</span><span class="sxs-lookup"><span data-stu-id="855db-146">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="855db-147">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="855db-147">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="855db-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="855db-148">DateTimeOffset</span></span>|<span data-ttu-id="855db-149">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="855db-149">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="855db-150">status</span><span class="sxs-lookup"><span data-stu-id="855db-150">status</span></span>|[<span data-ttu-id="855db-151">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="855db-151">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="855db-152">ポリシー レポートのコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="855db-152">Compliance status of the policy report.</span></span> <span data-ttu-id="855db-153">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="855db-153">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="855db-154">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="855db-154">lastReportedDateTime</span></span>|<span data-ttu-id="855db-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="855db-155">DateTimeOffset</span></span>|<span data-ttu-id="855db-156">ポリシー レポートの最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="855db-156">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="855db-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="855db-157">userPrincipalName</span></span>|<span data-ttu-id="855db-158">String</span><span class="sxs-lookup"><span data-stu-id="855db-158">String</span></span>|<span data-ttu-id="855db-159">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="855db-159">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="855db-160">応答</span><span class="sxs-lookup"><span data-stu-id="855db-160">Response</span></span>
<span data-ttu-id="855db-161">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="855db-161">If successful, this method returns a `201 Created` response code and a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="855db-162">例</span><span class="sxs-lookup"><span data-stu-id="855db-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="855db-163">要求</span><span class="sxs-lookup"><span data-stu-id="855db-163">Request</span></span>
<span data-ttu-id="855db-164">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="855db-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
Content-type: application/json
Content-length: 447

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
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

### <a name="response"></a><span data-ttu-id="855db-165">応答</span><span class="sxs-lookup"><span data-stu-id="855db-165">Response</span></span>
<span data-ttu-id="855db-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="855db-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





