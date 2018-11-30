---
title: mobileThreatDefenseConnector の取得
description: mobileThreatDefenseConnector オブジェクトのプロパティとリレーションシップを読み取ります。
ms.openlocfilehash: c19bfc556306bb596c5764bd8527aba5be8f01f8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020207"
---
# <a name="get-mobilethreatdefenseconnector"></a><span data-ttu-id="f47dd-103">mobileThreatDefenseConnector の取得</span><span class="sxs-lookup"><span data-stu-id="f47dd-103">Get mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="f47dd-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f47dd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f47dd-105">[mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f47dd-105">Read properties and relationships of the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f47dd-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="f47dd-106">Prerequisites</span></span>
<span data-ttu-id="f47dd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f47dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f47dd-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f47dd-109">Permission type</span></span>|<span data-ttu-id="f47dd-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f47dd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f47dd-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f47dd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f47dd-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f47dd-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="f47dd-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f47dd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f47dd-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f47dd-114">Not supported.</span></span>|
|<span data-ttu-id="f47dd-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f47dd-115">Application</span></span>|<span data-ttu-id="f47dd-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f47dd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f47dd-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f47dd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f47dd-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f47dd-118">Optional query parameters</span></span>
<span data-ttu-id="f47dd-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f47dd-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f47dd-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f47dd-120">Request headers</span></span>
|<span data-ttu-id="f47dd-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f47dd-121">Header</span></span>|<span data-ttu-id="f47dd-122">値</span><span class="sxs-lookup"><span data-stu-id="f47dd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f47dd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f47dd-123">Authorization</span></span>|<span data-ttu-id="f47dd-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f47dd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f47dd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f47dd-125">Accept</span></span>|<span data-ttu-id="f47dd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f47dd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f47dd-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f47dd-127">Request body</span></span>
<span data-ttu-id="f47dd-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f47dd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f47dd-129">応答</span><span class="sxs-lookup"><span data-stu-id="f47dd-129">Response</span></span>
<span data-ttu-id="f47dd-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f47dd-130">If successful, this method returns a `200 OK` response code and [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f47dd-131">例</span><span class="sxs-lookup"><span data-stu-id="f47dd-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f47dd-132">要求</span><span class="sxs-lookup"><span data-stu-id="f47dd-132">Request</span></span>
<span data-ttu-id="f47dd-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f47dd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

### <a name="response"></a><span data-ttu-id="f47dd-134">応答</span><span class="sxs-lookup"><span data-stu-id="f47dd-134">Response</span></span>
<span data-ttu-id="f47dd-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f47dd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 502

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
    "id": "e4bede14-de14-e4be-14de-bee414debee4",
    "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
    "partnerState": "available",
    "androidEnabled": true,
    "iosEnabled": true,
    "androidDeviceBlockedOnMissingPartnerData": true,
    "iosDeviceBlockedOnMissingPartnerData": true,
    "partnerUnsupportedOsVersionBlocked": true,
    "partnerUnresponsivenessThresholdInDays": 6
  }
}
```



