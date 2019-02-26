---
title: deviceEnrollmentWindowsHelloForBusinessConfiguration の取得
description: deviceEnrollmentWindowsHelloForBusinessConfiguration オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 03d9957f1c51132c74cdc4b190d5770370cf1e63
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252162"
---
# <a name="get-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="b3cf1-103">deviceEnrollmentWindowsHelloForBusinessConfiguration の取得</span><span class="sxs-lookup"><span data-stu-id="b3cf1-103">Get deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="b3cf1-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b3cf1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3cf1-105">[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b3cf1-105">Read properties and relationships of the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3cf1-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="b3cf1-106">Prerequisites</span></span>
<span data-ttu-id="b3cf1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b3cf1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b3cf1-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b3cf1-109">Permission type</span></span>|<span data-ttu-id="b3cf1-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b3cf1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3cf1-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b3cf1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b3cf1-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b3cf1-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="b3cf1-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b3cf1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3cf1-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b3cf1-114">Not supported.</span></span>|
|<span data-ttu-id="b3cf1-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b3cf1-115">Application</span></span>|<span data-ttu-id="b3cf1-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b3cf1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3cf1-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b3cf1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b3cf1-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b3cf1-118">Optional query parameters</span></span>
<span data-ttu-id="b3cf1-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b3cf1-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b3cf1-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b3cf1-120">Request headers</span></span>
|<span data-ttu-id="b3cf1-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b3cf1-121">Header</span></span>|<span data-ttu-id="b3cf1-122">値</span><span class="sxs-lookup"><span data-stu-id="b3cf1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3cf1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3cf1-123">Authorization</span></span>|<span data-ttu-id="b3cf1-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b3cf1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3cf1-125">承諾</span><span class="sxs-lookup"><span data-stu-id="b3cf1-125">Accept</span></span>|<span data-ttu-id="b3cf1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b3cf1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3cf1-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b3cf1-127">Request body</span></span>
<span data-ttu-id="b3cf1-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b3cf1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3cf1-129">応答</span><span class="sxs-lookup"><span data-stu-id="b3cf1-129">Response</span></span>
<span data-ttu-id="b3cf1-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b3cf1-130">If successful, this method returns a `200 OK` response code and [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3cf1-131">例</span><span class="sxs-lookup"><span data-stu-id="b3cf1-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3cf1-132">要求</span><span class="sxs-lookup"><span data-stu-id="b3cf1-132">Request</span></span>
<span data-ttu-id="b3cf1-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b3cf1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="b3cf1-134">応答</span><span class="sxs-lookup"><span data-stu-id="b3cf1-134">Response</span></span>
<span data-ttu-id="b3cf1-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b3cf1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



