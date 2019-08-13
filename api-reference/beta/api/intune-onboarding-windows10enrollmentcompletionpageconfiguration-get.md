---
title: Windows10EnrollmentCompletionPageConfiguration を取得する
description: Windows10EnrollmentCompletionPageConfiguration オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a272732d8e55e55ecad445d7aed71e94f827b243
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36352232"
---
# <a name="get-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="56711-103">Windows10EnrollmentCompletionPageConfiguration を取得する</span><span class="sxs-lookup"><span data-stu-id="56711-103">Get windows10EnrollmentCompletionPageConfiguration</span></span>

> <span data-ttu-id="56711-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="56711-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56711-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="56711-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56711-106">[Windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="56711-106">Read properties and relationships of the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="56711-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="56711-107">Prerequisites</span></span>
<span data-ttu-id="56711-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="56711-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56711-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="56711-110">Permission type</span></span>|<span data-ttu-id="56711-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="56711-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56711-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="56711-112">Delegated (work or school account)</span></span>|<span data-ttu-id="56711-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="56711-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="56711-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="56711-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56711-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="56711-115">Not supported.</span></span>|
|<span data-ttu-id="56711-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="56711-116">Application</span></span>|<span data-ttu-id="56711-117">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="56711-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="56711-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="56711-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="56711-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="56711-119">Optional query parameters</span></span>
<span data-ttu-id="56711-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="56711-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="56711-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="56711-121">Request headers</span></span>
|<span data-ttu-id="56711-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="56711-122">Header</span></span>|<span data-ttu-id="56711-123">値</span><span class="sxs-lookup"><span data-stu-id="56711-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56711-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="56711-124">Authorization</span></span>|<span data-ttu-id="56711-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="56711-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56711-126">承諾</span><span class="sxs-lookup"><span data-stu-id="56711-126">Accept</span></span>|<span data-ttu-id="56711-127">application/json</span><span class="sxs-lookup"><span data-stu-id="56711-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56711-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="56711-128">Request body</span></span>
<span data-ttu-id="56711-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="56711-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56711-130">応答</span><span class="sxs-lookup"><span data-stu-id="56711-130">Response</span></span>
<span data-ttu-id="56711-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="56711-131">If successful, this method returns a `200 OK` response code and [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56711-132">例</span><span class="sxs-lookup"><span data-stu-id="56711-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="56711-133">要求</span><span class="sxs-lookup"><span data-stu-id="56711-133">Request</span></span>
<span data-ttu-id="56711-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="56711-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="56711-135">応答</span><span class="sxs-lookup"><span data-stu-id="56711-135">Response</span></span>
<span data-ttu-id="56711-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="56711-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 810

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfiguration",
    "id": "77bf8248-8248-77bf-4882-bf774882bf77",
    "displayName": "Display Name value",
    "description": "Description value",
    "priority": 8,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "version": 7,
    "showInstallationProgress": true,
    "blockDeviceSetupRetryByUser": true,
    "allowDeviceResetOnInstallFailure": true,
    "allowLogCollectionOnInstallFailure": true,
    "customErrorMessage": "Custom Error Message value",
    "installProgressTimeoutInMinutes": 15,
    "allowDeviceUseOnInstallFailure": true,
    "selectedMobileAppIds": [
      "Selected Mobile App Ids value"
    ]
  }
}
```






