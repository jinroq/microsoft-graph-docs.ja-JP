---
title: Get deviceComplianceUserStatus
description: deviceComplianceUserStatus オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 540462f1cc4fd0dca592c5cdf7e519d41c6be450
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253681"
---
# <a name="get-devicecomplianceuserstatus"></a><span data-ttu-id="87238-103">Get deviceComplianceUserStatus</span><span class="sxs-lookup"><span data-stu-id="87238-103">Get deviceComplianceUserStatus</span></span>

> <span data-ttu-id="87238-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="87238-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87238-105">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="87238-105">Read properties and relationships of the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87238-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="87238-106">Prerequisites</span></span>
<span data-ttu-id="87238-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="87238-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="87238-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="87238-109">Permission type</span></span>|<span data-ttu-id="87238-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="87238-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87238-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="87238-111">Delegated (work or school account)</span></span>|<span data-ttu-id="87238-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="87238-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="87238-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="87238-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87238-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="87238-114">Not supported.</span></span>|
|<span data-ttu-id="87238-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="87238-115">Application</span></span>|<span data-ttu-id="87238-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="87238-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87238-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="87238-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="87238-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="87238-118">Optional query parameters</span></span>
<span data-ttu-id="87238-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="87238-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="87238-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="87238-120">Request headers</span></span>
|<span data-ttu-id="87238-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="87238-121">Header</span></span>|<span data-ttu-id="87238-122">値</span><span class="sxs-lookup"><span data-stu-id="87238-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87238-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="87238-123">Authorization</span></span>|<span data-ttu-id="87238-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="87238-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87238-125">承諾</span><span class="sxs-lookup"><span data-stu-id="87238-125">Accept</span></span>|<span data-ttu-id="87238-126">application/json</span><span class="sxs-lookup"><span data-stu-id="87238-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87238-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="87238-127">Request body</span></span>
<span data-ttu-id="87238-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="87238-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87238-129">応答</span><span class="sxs-lookup"><span data-stu-id="87238-129">Response</span></span>
<span data-ttu-id="87238-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="87238-130">If successful, this method returns a `200 OK` response code and [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87238-131">例</span><span class="sxs-lookup"><span data-stu-id="87238-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="87238-132">要求</span><span class="sxs-lookup"><span data-stu-id="87238-132">Request</span></span>
<span data-ttu-id="87238-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="87238-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
```

### <a name="response"></a><span data-ttu-id="87238-134">応答</span><span class="sxs-lookup"><span data-stu-id="87238-134">Response</span></span>
<span data-ttu-id="87238-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="87238-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 369

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
    "id": "a0b566cd-66cd-a0b5-cd66-b5a0cd66b5a0",
    "userDisplayName": "User Display Name value",
    "devicesCount": 12,
    "status": "notApplicable",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```



