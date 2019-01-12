---
title: Get termsAndConditions
description: termsAndConditions オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 97c4a4bf3c449c5771563c55cf924f94fd4ee85b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924784"
---
# <a name="get-termsandconditions"></a><span data-ttu-id="2ce3e-103">Get termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="2ce3e-103">Get termsAndConditions</span></span>

> <span data-ttu-id="2ce3e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2ce3e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2ce3e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ce3e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2ce3e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2ce3e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2ce3e-107">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="2ce3e-107">Read properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2ce3e-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="2ce3e-108">Prerequisites</span></span>
<span data-ttu-id="2ce3e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2ce3e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ce3e-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2ce3e-111">Permission type</span></span>|<span data-ttu-id="2ce3e-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2ce3e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ce3e-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2ce3e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2ce3e-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ce3e-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="2ce3e-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2ce3e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ce3e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ce3e-116">Not supported.</span></span>|
|<span data-ttu-id="2ce3e-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2ce3e-117">Application</span></span>|<span data-ttu-id="2ce3e-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ce3e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ce3e-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2ce3e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}/termsAndConditions
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2ce3e-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2ce3e-120">Optional query parameters</span></span>
<span data-ttu-id="2ce3e-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2ce3e-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2ce3e-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2ce3e-122">Request headers</span></span>
|<span data-ttu-id="2ce3e-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2ce3e-123">Header</span></span>|<span data-ttu-id="2ce3e-124">値</span><span class="sxs-lookup"><span data-stu-id="2ce3e-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ce3e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ce3e-125">Authorization</span></span>|<span data-ttu-id="2ce3e-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="2ce3e-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ce3e-127">Accept</span><span class="sxs-lookup"><span data-stu-id="2ce3e-127">Accept</span></span>|<span data-ttu-id="2ce3e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2ce3e-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ce3e-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="2ce3e-129">Request body</span></span>
<span data-ttu-id="2ce3e-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2ce3e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ce3e-131">応答</span><span class="sxs-lookup"><span data-stu-id="2ce3e-131">Response</span></span>
<span data-ttu-id="2ce3e-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2ce3e-132">If successful, this method returns a `200 OK` response code and [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ce3e-133">例</span><span class="sxs-lookup"><span data-stu-id="2ce3e-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="2ce3e-134">要求</span><span class="sxs-lookup"><span data-stu-id="2ce3e-134">Request</span></span>
<span data-ttu-id="2ce3e-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2ce3e-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}
```

### <a name="response"></a><span data-ttu-id="2ce3e-136">応答</span><span class="sxs-lookup"><span data-stu-id="2ce3e-136">Response</span></span>
<span data-ttu-id="2ce3e-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2ce3e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 546

{
  "value": {
    "@odata.type": "#microsoft.graph.termsAndConditions",
    "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "description": "Description value",
    "title": "Title value",
    "bodyText": "Body Text value",
    "acceptanceStatement": "Acceptance Statement value",
    "version": 7
  }
}
```





