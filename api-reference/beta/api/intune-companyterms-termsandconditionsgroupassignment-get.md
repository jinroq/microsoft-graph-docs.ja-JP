---
title: termsAndConditionsGroupAssignment を取得する
description: termsAndConditionsGroupAssignment オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 045fd64cebfe2e166d9a6e1a2fda5cf47243b0b9
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31785861"
---
# <a name="get-termsandconditionsgroupassignment"></a><span data-ttu-id="3fede-103">termsAndConditionsGroupAssignment を取得する</span><span class="sxs-lookup"><span data-stu-id="3fede-103">Get termsAndConditionsGroupAssignment</span></span>

> <span data-ttu-id="3fede-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3fede-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3fede-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3fede-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3fede-106">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="3fede-106">Read properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3fede-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="3fede-107">Prerequisites</span></span>
<span data-ttu-id="3fede-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3fede-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3fede-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3fede-110">Permission type</span></span>|<span data-ttu-id="3fede-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3fede-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3fede-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3fede-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3fede-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3fede-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="3fede-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3fede-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3fede-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3fede-115">Not supported.</span></span>|
|<span data-ttu-id="3fede-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3fede-116">Application</span></span>|<span data-ttu-id="3fede-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3fede-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3fede-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3fede-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3fede-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="3fede-119">Optional query parameters</span></span>
<span data-ttu-id="3fede-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="3fede-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3fede-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3fede-121">Request headers</span></span>
|<span data-ttu-id="3fede-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3fede-122">Header</span></span>|<span data-ttu-id="3fede-123">値</span><span class="sxs-lookup"><span data-stu-id="3fede-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3fede-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3fede-124">Authorization</span></span>|<span data-ttu-id="3fede-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="3fede-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3fede-126">承諾</span><span class="sxs-lookup"><span data-stu-id="3fede-126">Accept</span></span>|<span data-ttu-id="3fede-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3fede-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fede-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="3fede-128">Request body</span></span>
<span data-ttu-id="3fede-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3fede-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3fede-130">応答</span><span class="sxs-lookup"><span data-stu-id="3fede-130">Response</span></span>
<span data-ttu-id="3fede-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3fede-131">If successful, this method returns a `200 OK` response code and [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fede-132">例</span><span class="sxs-lookup"><span data-stu-id="3fede-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="3fede-133">要求</span><span class="sxs-lookup"><span data-stu-id="3fede-133">Request</span></span>
<span data-ttu-id="3fede-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3fede-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}
```

### <a name="response"></a><span data-ttu-id="3fede-135">応答</span><span class="sxs-lookup"><span data-stu-id="3fede-135">Response</span></span>
<span data-ttu-id="3fede-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3fede-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 194

{
  "value": {
    "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
    "id": "2eb1aab7-aab7-2eb1-b7aa-b12eb7aab12e",
    "targetGroupId": "Target Group Id value"
  }
}
```





