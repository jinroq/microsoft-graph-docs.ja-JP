---
title: OrgContacts を一覧表示する
description: この組織の組織の連絡先のリストを取得します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7f77eecb49173c35a4e1499ab5f113bce8c1865f
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657204"
---
# <a name="list-orgcontacts"></a><span data-ttu-id="5e400-103">OrgContacts を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="5e400-103">List orgContacts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e400-104">この組織の組織の連絡先のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="5e400-104">Retrieve the list of organizational contacts for this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="5e400-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5e400-105">Permissions</span></span>
<span data-ttu-id="5e400-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5e400-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e400-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5e400-108">Permission type</span></span>      | <span data-ttu-id="5e400-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5e400-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e400-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5e400-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5e400-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5e400-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5e400-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5e400-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e400-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5e400-113">Not supported.</span></span>    |
|<span data-ttu-id="5e400-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5e400-114">Application</span></span> | <span data-ttu-id="5e400-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e400-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5e400-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5e400-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5e400-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="5e400-117">Optional query parameters</span></span>
<span data-ttu-id="5e400-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5e400-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5e400-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5e400-119">Request headers</span></span>
| <span data-ttu-id="5e400-120">名前</span><span class="sxs-lookup"><span data-stu-id="5e400-120">Name</span></span>       | <span data-ttu-id="5e400-121">型</span><span class="sxs-lookup"><span data-stu-id="5e400-121">Type</span></span> | <span data-ttu-id="5e400-122">説明</span><span class="sxs-lookup"><span data-stu-id="5e400-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5e400-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e400-123">Authorization</span></span>  | <span data-ttu-id="5e400-124">string</span><span class="sxs-lookup"><span data-stu-id="5e400-124">string</span></span>  | <span data-ttu-id="5e400-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5e400-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5e400-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="5e400-127">Request body</span></span>
<span data-ttu-id="5e400-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5e400-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5e400-129">応答</span><span class="sxs-lookup"><span data-stu-id="5e400-129">Response</span></span>

<span data-ttu-id="5e400-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[orgcontact](../resources/orgcontact.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="5e400-130">If successful, this method returns a `200 OK` response code and a collection of [orgContact](../resources/orgcontact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5e400-131">例</span><span class="sxs-lookup"><span data-stu-id="5e400-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5e400-132">要求</span><span class="sxs-lookup"><span data-stu-id="5e400-132">Request</span></span>
<span data-ttu-id="5e400-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5e400-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_orgcontact"
}-->
```http
GET https://graph.microsoft.com/beta/contacts
```
##### <a name="response"></a><span data-ttu-id="5e400-134">応答</span><span class="sxs-lookup"><span data-stu-id="5e400-134">Response</span></span>
<span data-ttu-id="5e400-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5e400-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 222

{
  "value": [
    {
      "addresses":[
          {
            "city": "string",
            "countryOrRegion": "string",
            "officeLocation": "string",
            "postalCode": "string",
            "state": "string",
            "street": "string"
          }
      ],
      "companyName": "companyName-value",
      "department": "department-value",
      "displayName": "displayName-value",
      "phones":[
          {
            "type": "string",
            "number": "string"
          }
      ]
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5e400-138">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="5e400-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5e400-139">C#</span><span class="sxs-lookup"><span data-stu-id="5e400-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/list_orgcontact-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5e400-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="5e400-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/list_orgcontact-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List orgContact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/orgcontact-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/orgcontact-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
