---
title: 組織を一覧表示する
description: 組織オブジェクトのリストを取得します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9dd1489714c4de87f0072ef0498c5acdf008d5ff
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938826"
---
# <a name="list-organization"></a><span data-ttu-id="02781-103">組織を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="02781-103">List organization</span></span>

> <span data-ttu-id="02781-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="02781-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="02781-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02781-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="02781-106">組織オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="02781-106">Retrieve a list of organization objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="02781-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="02781-107">Permissions</span></span>
<span data-ttu-id="02781-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="02781-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02781-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="02781-110">Permission type</span></span>      | <span data-ttu-id="02781-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="02781-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02781-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="02781-112">Delegated (work or school account)</span></span> | <span data-ttu-id="02781-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02781-113">Not supported.</span></span>    |
|<span data-ttu-id="02781-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="02781-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02781-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02781-115">Not supported.</span></span>    |
|<span data-ttu-id="02781-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="02781-116">Application</span></span> | <span data-ttu-id="02781-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02781-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="02781-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="02781-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /organization
```
## <a name="optional-query-parameters"></a><span data-ttu-id="02781-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="02781-119">Optional query parameters</span></span>
<span data-ttu-id="02781-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="02781-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="02781-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="02781-121">Request headers</span></span>
| <span data-ttu-id="02781-122">名前</span><span class="sxs-lookup"><span data-stu-id="02781-122">Name</span></span>       | <span data-ttu-id="02781-123">型</span><span class="sxs-lookup"><span data-stu-id="02781-123">Type</span></span> | <span data-ttu-id="02781-124">説明</span><span class="sxs-lookup"><span data-stu-id="02781-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="02781-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="02781-125">Authorization</span></span>  | <span data-ttu-id="02781-126">string</span><span class="sxs-lookup"><span data-stu-id="02781-126">string</span></span>  | <span data-ttu-id="02781-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="02781-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="02781-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="02781-129">Request body</span></span>
<span data-ttu-id="02781-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="02781-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02781-131">応答</span><span class="sxs-lookup"><span data-stu-id="02781-131">Response</span></span>

<span data-ttu-id="02781-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [organization](../resources/organization.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="02781-132">If successful, this method returns a `200 OK` response code and collection of [organization](../resources/organization.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="02781-133">例</span><span class="sxs-lookup"><span data-stu-id="02781-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="02781-134">要求</span><span class="sxs-lookup"><span data-stu-id="02781-134">Request</span></span>
<span data-ttu-id="02781-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="02781-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->
```http
GET https://graph.microsoft.com/beta/organization
```
##### <a name="response"></a><span data-ttu-id="02781-136">応答</span><span class="sxs-lookup"><span data-stu-id="02781-136">Response</span></span>
<span data-ttu-id="02781-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="02781-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 500

{
  "value": [
    {
      "assignedPlans": [
        {
          "assignedDateTime": "2016-10-19T10:37:00Z",
          "capabilityStatus": "capabilityStatus-value",
          "service": "service-value",
          "servicePlanId": "servicePlanId-value"
        }
      ],
      "businessPhones": [
        "businessPhones-value"
      ],
      "city": "city-value",
      "country": "country-value",
      "countryLetterCode": "countryLetterCode-value",
      "displayName": "displayName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
