---
title: DepOnboardingSetting を取得します。
description: DepOnboardingSetting オブジェクトのプロパティと関係を参照してください。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d5eb969b06216a756ad41ea92dd297e6ef25326f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393019"
---
# <a name="get-deponboardingsetting"></a><span data-ttu-id="f4ae6-103">DepOnboardingSetting を取得します。</span><span class="sxs-lookup"><span data-stu-id="f4ae6-103">Get depOnboardingSetting</span></span>

> <span data-ttu-id="f4ae6-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f4ae6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f4ae6-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f4ae6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f4ae6-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f4ae6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4ae6-107">[DepOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f4ae6-107">Read properties and relationships of the [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4ae6-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="f4ae6-108">Prerequisites</span></span>
<span data-ttu-id="f4ae6-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f4ae6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f4ae6-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f4ae6-111">Permission type</span></span>|<span data-ttu-id="f4ae6-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f4ae6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4ae6-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f4ae6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f4ae6-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4ae6-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="f4ae6-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f4ae6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4ae6-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f4ae6-116">Not supported.</span></span>|
|<span data-ttu-id="f4ae6-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f4ae6-117">Application</span></span>|<span data-ttu-id="f4ae6-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f4ae6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4ae6-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f4ae6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f4ae6-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f4ae6-120">Optional query parameters</span></span>
<span data-ttu-id="f4ae6-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f4ae6-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f4ae6-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f4ae6-122">Request headers</span></span>
|<span data-ttu-id="f4ae6-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f4ae6-123">Header</span></span>|<span data-ttu-id="f4ae6-124">値</span><span class="sxs-lookup"><span data-stu-id="f4ae6-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4ae6-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4ae6-125">Authorization</span></span>|<span data-ttu-id="f4ae6-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f4ae6-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4ae6-127">Accept</span><span class="sxs-lookup"><span data-stu-id="f4ae6-127">Accept</span></span>|<span data-ttu-id="f4ae6-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f4ae6-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4ae6-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="f4ae6-129">Request body</span></span>
<span data-ttu-id="f4ae6-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f4ae6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4ae6-131">応答</span><span class="sxs-lookup"><span data-stu-id="f4ae6-131">Response</span></span>
<span data-ttu-id="f4ae6-132">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="f4ae6-132">If successful, this method returns a `200 OK` response code and [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4ae6-133">例</span><span class="sxs-lookup"><span data-stu-id="f4ae6-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4ae6-134">要求</span><span class="sxs-lookup"><span data-stu-id="f4ae6-134">Request</span></span>
<span data-ttu-id="f4ae6-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f4ae6-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
```

### <a name="response"></a><span data-ttu-id="f4ae6-136">応答</span><span class="sxs-lookup"><span data-stu-id="f4ae6-136">Response</span></span>
<span data-ttu-id="f4ae6-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f4ae6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 672

{
  "value": {
    "@odata.type": "#microsoft.graph.depOnboardingSetting",
    "id": "40342229-2229-4034-2922-344029223440",
    "appleIdentifier": "Apple Identifier value",
    "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "lastSuccessfulSyncDateTime": "2017-01-01T00:03:28.120883-08:00",
    "lastSyncTriggeredDateTime": "2017-01-01T00:00:02.0916369-08:00",
    "shareTokenWithSchoolDataSyncService": true,
    "lastSyncErrorCode": 1,
    "tokenType": "dep",
    "tokenName": "Token Name value",
    "syncedDeviceCount": 1,
    "dataSharingConsentGranted": true
  }
}
```




