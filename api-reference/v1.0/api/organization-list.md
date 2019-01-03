---
title: 組織を一覧表示する
description: 組織オブジェクトのリストを取得します。
ms.openlocfilehash: 9a66fac482e5bc4a6fe822210ae274abdb725360
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024097"
---
# <a name="list-organization"></a><span data-ttu-id="f1515-103">組織を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="f1515-103">List organization</span></span>



<span data-ttu-id="f1515-104">組織オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="f1515-104">Retrieve a list of organization objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="f1515-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f1515-105">Permissions</span></span>
<span data-ttu-id="f1515-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f1515-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1515-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f1515-108">Permission type</span></span>      | <span data-ttu-id="f1515-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f1515-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1515-110">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="f1515-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f1515-111">User.Read、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1515-111">User.Read, Directory.Read.All, Directory.ReadWrite.All</span></span>   |
|<span data-ttu-id="f1515-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f1515-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1515-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f1515-113">Not supported.</span></span>    |
|<span data-ttu-id="f1515-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f1515-114">Application</span></span> | <span data-ttu-id="f1515-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1515-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="f1515-116">注: User.Read アクセス許可を付与されたアプリケーションは、組織の *id*、*displayName*、および *verifiedDomains* プロパティのみを読み取ることができます。</span><span class="sxs-lookup"><span data-stu-id="f1515-116">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="f1515-117">他のすべてのプロパティは `null` 値を返します。</span><span class="sxs-lookup"><span data-stu-id="f1515-117">All other properties will return with `null` values.</span></span> <span data-ttu-id="f1515-118">すべてのプロパティを読み取るには、Directory.Read.All を使用します。</span><span class="sxs-lookup"><span data-stu-id="f1515-118">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="f1515-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f1515-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /organization
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f1515-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f1515-120">Optional query parameters</span></span>
<span data-ttu-id="f1515-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f1515-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f1515-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f1515-122">Request headers</span></span>
| <span data-ttu-id="f1515-123">名前</span><span class="sxs-lookup"><span data-stu-id="f1515-123">Name</span></span>       | <span data-ttu-id="f1515-124">型</span><span class="sxs-lookup"><span data-stu-id="f1515-124">Type</span></span> | <span data-ttu-id="f1515-125">説明</span><span class="sxs-lookup"><span data-stu-id="f1515-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f1515-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1515-126">Authorization</span></span>  | <span data-ttu-id="f1515-127">string</span><span class="sxs-lookup"><span data-stu-id="f1515-127">string</span></span>  | <span data-ttu-id="f1515-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f1515-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1515-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="f1515-130">Request body</span></span>
<span data-ttu-id="f1515-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f1515-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1515-132">応答</span><span class="sxs-lookup"><span data-stu-id="f1515-132">Response</span></span>

<span data-ttu-id="f1515-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [organization](../resources/organization.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="f1515-133">If successful, this method returns a `200 OK` response code and collection of [organization](../resources/organization.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f1515-134">例</span><span class="sxs-lookup"><span data-stu-id="f1515-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f1515-135">要求</span><span class="sxs-lookup"><span data-stu-id="f1515-135">Request</span></span>
<span data-ttu-id="f1515-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f1515-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->
```http
GET https://graph.microsoft.com/beta/organization
```
##### <a name="response"></a><span data-ttu-id="f1515-137">応答</span><span class="sxs-lookup"><span data-stu-id="f1515-137">Response</span></span>
<span data-ttu-id="f1515-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f1515-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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