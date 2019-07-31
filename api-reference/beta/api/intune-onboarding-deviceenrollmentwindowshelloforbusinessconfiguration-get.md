---
title: deviceEnrollmentWindowsHelloForBusinessConfiguration の取得
description: deviceEnrollmentWindowsHelloForBusinessConfiguration オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2e62f62a4d61ba0167076c079bec74fab5127703
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35984553"
---
# <a name="get-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="a90fe-103">deviceEnrollmentWindowsHelloForBusinessConfiguration の取得</span><span class="sxs-lookup"><span data-stu-id="a90fe-103">Get deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="a90fe-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a90fe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a90fe-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a90fe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a90fe-106">[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a90fe-106">Read properties and relationships of the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a90fe-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="a90fe-107">Prerequisites</span></span>
<span data-ttu-id="a90fe-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a90fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a90fe-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a90fe-110">Permission type</span></span>|<span data-ttu-id="a90fe-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a90fe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a90fe-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a90fe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a90fe-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a90fe-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="a90fe-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a90fe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a90fe-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a90fe-115">Not supported.</span></span>|
|<span data-ttu-id="a90fe-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a90fe-116">Application</span></span>|<span data-ttu-id="a90fe-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a90fe-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a90fe-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a90fe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a90fe-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a90fe-119">Optional query parameters</span></span>
<span data-ttu-id="a90fe-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a90fe-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a90fe-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a90fe-121">Request headers</span></span>
|<span data-ttu-id="a90fe-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a90fe-122">Header</span></span>|<span data-ttu-id="a90fe-123">値</span><span class="sxs-lookup"><span data-stu-id="a90fe-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a90fe-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a90fe-124">Authorization</span></span>|<span data-ttu-id="a90fe-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a90fe-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a90fe-126">承諾</span><span class="sxs-lookup"><span data-stu-id="a90fe-126">Accept</span></span>|<span data-ttu-id="a90fe-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a90fe-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a90fe-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="a90fe-128">Request body</span></span>
<span data-ttu-id="a90fe-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a90fe-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a90fe-130">応答</span><span class="sxs-lookup"><span data-stu-id="a90fe-130">Response</span></span>
<span data-ttu-id="a90fe-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a90fe-131">If successful, this method returns a `200 OK` response code and [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a90fe-132">例</span><span class="sxs-lookup"><span data-stu-id="a90fe-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a90fe-133">要求</span><span class="sxs-lookup"><span data-stu-id="a90fe-133">Request</span></span>
<span data-ttu-id="a90fe-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a90fe-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="a90fe-135">応答</span><span class="sxs-lookup"><span data-stu-id="a90fe-135">Response</span></span>
<span data-ttu-id="a90fe-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a90fe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 900

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
    "enhancedBiometricsState": "enabled",
    "securityKeyForSignIn": "enabled"
  }
}
```





