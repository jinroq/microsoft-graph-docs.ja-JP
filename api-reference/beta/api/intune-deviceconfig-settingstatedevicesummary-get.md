---
title: Get settingStateDeviceSummary
description: settingStateDeviceSummary オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
ms.openlocfilehash: 3308a4fff48b6433d7c35303566ddc73f03c23e6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333510"
---
# <a name="get-settingstatedevicesummary"></a><span data-ttu-id="c3c65-103">Get settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="c3c65-103">Get settingStateDeviceSummary</span></span>

> <span data-ttu-id="c3c65-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c3c65-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c3c65-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3c65-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c3c65-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c3c65-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c3c65-107">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c3c65-107">Read properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c3c65-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="c3c65-108">Prerequisites</span></span>
<span data-ttu-id="c3c65-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c3c65-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3c65-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c3c65-111">Permission type</span></span>|<span data-ttu-id="c3c65-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c3c65-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3c65-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c3c65-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c3c65-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c3c65-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c3c65-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c3c65-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3c65-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3c65-116">Not supported.</span></span>|
|<span data-ttu-id="c3c65-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c3c65-117">Application</span></span>|<span data-ttu-id="c3c65-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3c65-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3c65-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c3c65-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c3c65-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c3c65-120">Optional query parameters</span></span>
<span data-ttu-id="c3c65-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c3c65-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c3c65-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c3c65-122">Request headers</span></span>
|<span data-ttu-id="c3c65-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c3c65-123">Header</span></span>|<span data-ttu-id="c3c65-124">値</span><span class="sxs-lookup"><span data-stu-id="c3c65-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3c65-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3c65-125">Authorization</span></span>|<span data-ttu-id="c3c65-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c3c65-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3c65-127">Accept</span><span class="sxs-lookup"><span data-stu-id="c3c65-127">Accept</span></span>|<span data-ttu-id="c3c65-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c3c65-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3c65-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="c3c65-129">Request body</span></span>
<span data-ttu-id="c3c65-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c3c65-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3c65-131">応答</span><span class="sxs-lookup"><span data-stu-id="c3c65-131">Response</span></span>
<span data-ttu-id="c3c65-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c3c65-132">If successful, this method returns a `200 OK` response code and [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3c65-133">例</span><span class="sxs-lookup"><span data-stu-id="c3c65-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="c3c65-134">要求</span><span class="sxs-lookup"><span data-stu-id="c3c65-134">Request</span></span>
<span data-ttu-id="c3c65-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c3c65-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

### <a name="response"></a><span data-ttu-id="c3c65-136">応答</span><span class="sxs-lookup"><span data-stu-id="c3c65-136">Response</span></span>
<span data-ttu-id="c3c65-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c3c65-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 450

{
  "value": {
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
}
```




