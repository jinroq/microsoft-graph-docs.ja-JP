---
title: softwareUpdateStatusSummary の取得
description: softwareUpdateStatusSummary オブジェクトのプロパティとリレーションシップを読み取ります。
ms.openlocfilehash: f22c63235848bfe86f5ced684c66103a7203bedd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022534"
---
# <a name="get-softwareupdatestatussummary"></a><span data-ttu-id="7b339-103">softwareUpdateStatusSummary の取得</span><span class="sxs-lookup"><span data-stu-id="7b339-103">Get softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="7b339-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7b339-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7b339-105">[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7b339-105">Read properties and relationships of the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7b339-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="7b339-106">Prerequisites</span></span>
<span data-ttu-id="7b339-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7b339-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b339-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7b339-109">Permission type</span></span>|<span data-ttu-id="7b339-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7b339-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b339-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7b339-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7b339-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b339-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7b339-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7b339-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b339-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7b339-114">Not supported.</span></span>|
|<span data-ttu-id="7b339-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7b339-115">Application</span></span>|<span data-ttu-id="7b339-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7b339-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b339-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7b339-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/softwareUpdateStatusSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7b339-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7b339-118">Optional query parameters</span></span>
<span data-ttu-id="7b339-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7b339-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7b339-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7b339-120">Request headers</span></span>
|<span data-ttu-id="7b339-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7b339-121">Header</span></span>|<span data-ttu-id="7b339-122">値</span><span class="sxs-lookup"><span data-stu-id="7b339-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b339-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b339-123">Authorization</span></span>|<span data-ttu-id="7b339-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7b339-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b339-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7b339-125">Accept</span></span>|<span data-ttu-id="7b339-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7b339-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b339-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="7b339-127">Request body</span></span>
<span data-ttu-id="7b339-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7b339-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b339-129">応答</span><span class="sxs-lookup"><span data-stu-id="7b339-129">Response</span></span>
<span data-ttu-id="7b339-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7b339-130">If successful, this method returns a `200 OK` response code and [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b339-131">例</span><span class="sxs-lookup"><span data-stu-id="7b339-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="7b339-132">要求</span><span class="sxs-lookup"><span data-stu-id="7b339-132">Request</span></span>
<span data-ttu-id="7b339-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7b339-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/softwareUpdateStatusSummary
```

### <a name="response"></a><span data-ttu-id="7b339-134">応答</span><span class="sxs-lookup"><span data-stu-id="7b339-134">Response</span></span>
<span data-ttu-id="7b339-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7b339-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 620

{
  "value": {
    "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
    "id": "4f71421f-421f-4f71-1f42-714f1f42714f",
    "displayName": "Display Name value",
    "compliantDeviceCount": 4,
    "nonCompliantDeviceCount": 7,
    "remediatedDeviceCount": 5,
    "errorDeviceCount": 0,
    "unknownDeviceCount": 2,
    "conflictDeviceCount": 3,
    "notApplicableDeviceCount": 8,
    "compliantUserCount": 2,
    "nonCompliantUserCount": 5,
    "remediatedUserCount": 3,
    "errorUserCount": 14,
    "unknownUserCount": 0,
    "conflictUserCount": 1,
    "notApplicableUserCount": 6
  }
}
```


