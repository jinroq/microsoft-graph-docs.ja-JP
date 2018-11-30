---
title: deviceEnrollmentWindowsHelloForBusinessConfiguration の取得
description: deviceEnrollmentWindowsHelloForBusinessConfiguration オブジェクトのプロパティとリレーションシップを読み取ります。
ms.openlocfilehash: ab801bc5e9a80d2998ae1bd6738f3b51ec11df1b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022264"
---
# <a name="get-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="89828-103">deviceEnrollmentWindowsHelloForBusinessConfiguration の取得</span><span class="sxs-lookup"><span data-stu-id="89828-103">Get deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="89828-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="89828-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="89828-105">[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="89828-105">Read properties and relationships of the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="89828-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="89828-106">Prerequisites</span></span>
<span data-ttu-id="89828-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="89828-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89828-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="89828-109">Permission type</span></span>|<span data-ttu-id="89828-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="89828-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89828-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="89828-111">Delegated (work or school account)</span></span>|<span data-ttu-id="89828-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="89828-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="89828-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="89828-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89828-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89828-114">Not supported.</span></span>|
|<span data-ttu-id="89828-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="89828-115">Application</span></span>|<span data-ttu-id="89828-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89828-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="89828-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="89828-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="89828-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="89828-118">Optional query parameters</span></span>
<span data-ttu-id="89828-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="89828-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="89828-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="89828-120">Request headers</span></span>
|<span data-ttu-id="89828-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="89828-121">Header</span></span>|<span data-ttu-id="89828-122">値</span><span class="sxs-lookup"><span data-stu-id="89828-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89828-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="89828-123">Authorization</span></span>|<span data-ttu-id="89828-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="89828-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89828-125">Accept</span><span class="sxs-lookup"><span data-stu-id="89828-125">Accept</span></span>|<span data-ttu-id="89828-126">application/json</span><span class="sxs-lookup"><span data-stu-id="89828-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89828-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="89828-127">Request body</span></span>
<span data-ttu-id="89828-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="89828-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89828-129">応答</span><span class="sxs-lookup"><span data-stu-id="89828-129">Response</span></span>
<span data-ttu-id="89828-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="89828-130">If successful, this method returns a `200 OK` response code and [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89828-131">例</span><span class="sxs-lookup"><span data-stu-id="89828-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="89828-132">要求</span><span class="sxs-lookup"><span data-stu-id="89828-132">Request</span></span>
<span data-ttu-id="89828-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="89828-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="89828-134">応答</span><span class="sxs-lookup"><span data-stu-id="89828-134">Response</span></span>
<span data-ttu-id="89828-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="89828-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 860

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
    "id": "3068e0cd-e0cd-3068-cde0-6830cde06830",
    "displayName": "Display Name value",
    "description": "Description value",
    "priority": 8,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "version": 7,
    "pinMinimumLength": 0,
    "pinMaximumLength": 0,
    "pinUppercaseCharactersUsage": "required",
    "pinLowercaseCharactersUsage": "required",
    "pinSpecialCharactersUsage": "required",
    "state": "enabled",
    "securityDeviceRequired": true,
    "unlockWithBiometricsEnabled": true,
    "remotePassportEnabled": true,
    "pinPreviousBlockCount": 5,
    "pinExpirationInDays": 3,
    "enhancedBiometricsState": "enabled"
  }
}
```



