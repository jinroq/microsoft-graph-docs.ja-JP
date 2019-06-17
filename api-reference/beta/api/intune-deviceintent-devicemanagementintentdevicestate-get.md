---
title: DeviceManagementIntentDeviceState の取得
description: DeviceManagementIntentDeviceState オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 59397340c2e38402dc2d377c2fc30cd8fbdf3bc6
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34960273"
---
# <a name="get-devicemanagementintentdevicestate"></a><span data-ttu-id="fa105-103">DeviceManagementIntentDeviceState の取得</span><span class="sxs-lookup"><span data-stu-id="fa105-103">Get deviceManagementIntentDeviceState</span></span>

> <span data-ttu-id="fa105-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fa105-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa105-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fa105-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa105-106">[Devicemanagementintentdevicestate](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="fa105-106">Read properties and relationships of the [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa105-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="fa105-107">Prerequisites</span></span>
<span data-ttu-id="fa105-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fa105-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa105-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fa105-110">Permission type</span></span>|<span data-ttu-id="fa105-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fa105-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa105-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fa105-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fa105-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa105-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fa105-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fa105-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa105-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fa105-115">Not supported.</span></span>|
|<span data-ttu-id="fa105-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fa105-116">Application</span></span>|<span data-ttu-id="fa105-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fa105-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa105-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fa105-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/deviceStates/{deviceManagementIntentDeviceStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fa105-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="fa105-119">Optional query parameters</span></span>
<span data-ttu-id="fa105-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="fa105-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fa105-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fa105-121">Request headers</span></span>
|<span data-ttu-id="fa105-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fa105-122">Header</span></span>|<span data-ttu-id="fa105-123">値</span><span class="sxs-lookup"><span data-stu-id="fa105-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa105-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa105-124">Authorization</span></span>|<span data-ttu-id="fa105-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="fa105-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa105-126">承諾</span><span class="sxs-lookup"><span data-stu-id="fa105-126">Accept</span></span>|<span data-ttu-id="fa105-127">application/json</span><span class="sxs-lookup"><span data-stu-id="fa105-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa105-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="fa105-128">Request body</span></span>
<span data-ttu-id="fa105-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="fa105-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa105-130">応答</span><span class="sxs-lookup"><span data-stu-id="fa105-130">Response</span></span>
<span data-ttu-id="fa105-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[Devicemanagementintentdevicestate](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="fa105-131">If successful, this method returns a `200 OK` response code and [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa105-132">例</span><span class="sxs-lookup"><span data-stu-id="fa105-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa105-133">要求</span><span class="sxs-lookup"><span data-stu-id="fa105-133">Request</span></span>
<span data-ttu-id="fa105-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fa105-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceStates/{deviceManagementIntentDeviceStateId}
```

### <a name="response"></a><span data-ttu-id="fa105-135">応答</span><span class="sxs-lookup"><span data-stu-id="fa105-135">Response</span></span>
<span data-ttu-id="fa105-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fa105-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 426

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceState",
    "id": "8db75881-5881-8db7-8158-b78d8158b78d",
    "userPrincipalName": "User Principal Name value",
    "userName": "User Name value",
    "deviceDisplayName": "Device Display Name value",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "state": "notApplicable",
    "deviceId": "Device Id value"
  }
}
```





