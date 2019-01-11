---
title: Get mobileAppAssignment
description: mobileAppAssignment オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 790b6e6a8c0f970c7f4b0aa13ed739cec585d9d2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831123"
---
# <a name="get-mobileappassignment"></a><span data-ttu-id="c8732-103">Get mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="c8732-103">Get mobileAppAssignment</span></span>

> <span data-ttu-id="c8732-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c8732-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c8732-105">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c8732-105">Read properties and relationships of the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c8732-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="c8732-106">Prerequisites</span></span>
<span data-ttu-id="c8732-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c8732-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8732-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c8732-109">Permission type</span></span>|<span data-ttu-id="c8732-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c8732-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8732-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c8732-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c8732-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c8732-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c8732-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c8732-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8732-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8732-114">Not supported.</span></span>|
|<span data-ttu-id="c8732-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c8732-115">Application</span></span>|<span data-ttu-id="c8732-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8732-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8732-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c8732-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c8732-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c8732-118">Optional query parameters</span></span>
<span data-ttu-id="c8732-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c8732-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c8732-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c8732-120">Request headers</span></span>
|<span data-ttu-id="c8732-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c8732-121">Header</span></span>|<span data-ttu-id="c8732-122">値</span><span class="sxs-lookup"><span data-stu-id="c8732-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8732-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8732-123">Authorization</span></span>|<span data-ttu-id="c8732-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c8732-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8732-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c8732-125">Accept</span></span>|<span data-ttu-id="c8732-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c8732-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8732-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c8732-127">Request body</span></span>
<span data-ttu-id="c8732-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c8732-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8732-129">応答</span><span class="sxs-lookup"><span data-stu-id="c8732-129">Response</span></span>
<span data-ttu-id="c8732-130">成功した場合、このメソッドは `200 OK` 応答コードと応答本文で [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c8732-130">If successful, this method returns a `200 OK` response code and [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8732-131">例</span><span class="sxs-lookup"><span data-stu-id="c8732-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="c8732-132">要求</span><span class="sxs-lookup"><span data-stu-id="c8732-132">Request</span></span>
<span data-ttu-id="c8732-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c8732-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

### <a name="response"></a><span data-ttu-id="c8732-134">応答</span><span class="sxs-lookup"><span data-stu-id="c8732-134">Response</span></span>
<span data-ttu-id="c8732-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c8732-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 359

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppAssignment",
    "id": "591620b7-20b7-5916-b720-1659b7201659",
    "intent": "required",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    },
    "settings": {
      "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
    }
  }
}
```



