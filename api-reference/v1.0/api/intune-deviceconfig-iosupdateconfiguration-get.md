---
title: Get iosUpdateConfiguration
description: iosUpdateConfiguration オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 90de0e51ca680327dbb6dc895f81f5c82914e3a7
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260397"
---
# <a name="get-iosupdateconfiguration"></a><span data-ttu-id="b9d9c-103">Get iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="b9d9c-103">Get iosUpdateConfiguration</span></span>

> <span data-ttu-id="b9d9c-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b9d9c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9d9c-105">[iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b9d9c-105">Read properties and relationships of the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9d9c-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="b9d9c-106">Prerequisites</span></span>
<span data-ttu-id="b9d9c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b9d9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b9d9c-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b9d9c-109">Permission type</span></span>|<span data-ttu-id="b9d9c-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b9d9c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9d9c-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b9d9c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b9d9c-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9d9c-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b9d9c-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b9d9c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9d9c-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b9d9c-114">Not supported.</span></span>|
|<span data-ttu-id="b9d9c-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b9d9c-115">Application</span></span>|<span data-ttu-id="b9d9c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b9d9c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9d9c-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b9d9c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b9d9c-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b9d9c-118">Optional query parameters</span></span>
<span data-ttu-id="b9d9c-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b9d9c-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b9d9c-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b9d9c-120">Request headers</span></span>
|<span data-ttu-id="b9d9c-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b9d9c-121">Header</span></span>|<span data-ttu-id="b9d9c-122">値</span><span class="sxs-lookup"><span data-stu-id="b9d9c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9d9c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9d9c-123">Authorization</span></span>|<span data-ttu-id="b9d9c-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b9d9c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9d9c-125">承諾</span><span class="sxs-lookup"><span data-stu-id="b9d9c-125">Accept</span></span>|<span data-ttu-id="b9d9c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b9d9c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9d9c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b9d9c-127">Request body</span></span>
<span data-ttu-id="b9d9c-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b9d9c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9d9c-129">応答</span><span class="sxs-lookup"><span data-stu-id="b9d9c-129">Response</span></span>
<span data-ttu-id="b9d9c-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b9d9c-130">If successful, this method returns a `200 OK` response code and [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9d9c-131">例</span><span class="sxs-lookup"><span data-stu-id="b9d9c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9d9c-132">要求</span><span class="sxs-lookup"><span data-stu-id="b9d9c-132">Request</span></span>
<span data-ttu-id="b9d9c-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b9d9c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="b9d9c-134">応答</span><span class="sxs-lookup"><span data-stu-id="b9d9c-134">Response</span></span>
<span data-ttu-id="b9d9c-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b9d9c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 542

{
  "value": {
    "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
    "id": "321aef09-ef09-321a-09ef-1a3209ef1a32",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "activeHoursStart": "12:00:05.5020000",
    "activeHoursEnd": "11:59:00.8990000",
    "scheduledInstallDays": [
      "monday"
    ],
    "utcTimeOffsetInMinutes": 6
  }
}
```



