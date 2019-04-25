---
title: applicationSignInDetailedSummary を取得する
description: applicationSignInDetailSummary オブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0d9cf9fb87e2de381cd347db84e2c8007c64e41a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32639985"
---
# <a name="get-applicationsignindetailedsummary"></a><span data-ttu-id="e37d9-103">applicationSignInDetailedSummary を取得する</span><span class="sxs-lookup"><span data-stu-id="e37d9-103">Get applicationSignInDetailedSummary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e37d9-104">[applicationSignInDetailSummary](../resources/applicationsignindetailedsummary.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="e37d9-104">Retrieve the properties and relationships of an [applicationSignInDetailSummary](../resources/applicationsignindetailedsummary.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e37d9-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e37d9-105">Permissions</span></span>
<span data-ttu-id="e37d9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e37d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="e37d9-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e37d9-108">Permission type</span></span>                        | <span data-ttu-id="e37d9-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e37d9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e37d9-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e37d9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e37d9-111">すべてのレポートを取得します。</span><span class="sxs-lookup"><span data-stu-id="e37d9-111">Report.Read.All</span></span> |
|<span data-ttu-id="e37d9-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e37d9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e37d9-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e37d9-113">Not supported.</span></span> |
|<span data-ttu-id="e37d9-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e37d9-114">Application</span></span>                            | <span data-ttu-id="e37d9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e37d9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e37d9-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e37d9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
GET /reports/applicationSignInDetailedSummary/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e37d9-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e37d9-117">Optional query parameters</span></span>

<span data-ttu-id="e37d9-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e37d9-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e37d9-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e37d9-119">Request headers</span></span>

| <span data-ttu-id="e37d9-120">名前</span><span class="sxs-lookup"><span data-stu-id="e37d9-120">Name</span></span>      |<span data-ttu-id="e37d9-121">説明</span><span class="sxs-lookup"><span data-stu-id="e37d9-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e37d9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e37d9-122">Authorization</span></span> | <span data-ttu-id="e37d9-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="e37d9-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e37d9-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="e37d9-124">Request body</span></span>
<span data-ttu-id="e37d9-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e37d9-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e37d9-126">応答</span><span class="sxs-lookup"><span data-stu-id="e37d9-126">Response</span></span>
<span data-ttu-id="e37d9-127">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e37d9-127">If successful, this method returns a `200 OK` response code and an [applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e37d9-128">例</span><span class="sxs-lookup"><span data-stu-id="e37d9-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="e37d9-129">要求</span><span class="sxs-lookup"><span data-stu-id="e37d9-129">Request</span></span>
<span data-ttu-id="e37d9-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e37d9-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_applicationsignindetailedsummary"
}-->
```http
GET https://graph.microsoft.com/beta/reports/applicationSignInDetailedSummary/<id>
```

### <a name="response"></a><span data-ttu-id="e37d9-131">応答</span><span class="sxs-lookup"><span data-stu-id="e37d9-131">Response</span></span>
<span data-ttu-id="e37d9-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e37d9-132">The following is an example of the response.</span></span> 

><span data-ttu-id="e37d9-p102">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e37d9-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationSignInDetailedSummary"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 295

{
  "id": "id-value",
  "appId": "appId-value",
  "appDisplayName": "appDisplayName-value",
  "status": {
    "errorCode": 99,
    "failureReason": "failureReason-value",
    "additionalDetails": "additionalDetails-value"
  },
  "signInCount": 99,
  "aggregatedEventDateTime": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get applicationSignInDetailedSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
