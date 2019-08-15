---
title: servicePrincipals を一覧表示する
description: servicePrincipal オブジェクトの一覧を取得します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 333585e304c3da9b114d45fe88b1ca59918d09a4
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410142"
---
# <a name="list-serviceprincipals"></a><span data-ttu-id="ed592-103">servicePrincipals を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ed592-103">List servicePrincipals</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed592-104">servicePrincipal オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="ed592-104">Retrieve a list of servicePrincipal objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed592-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ed592-105">Permissions</span></span>

<span data-ttu-id="ed592-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ed592-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ed592-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ed592-108">Permission type</span></span>      | <span data-ttu-id="ed592-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ed592-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed592-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ed592-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ed592-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ed592-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ed592-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ed592-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed592-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed592-113">Not supported.</span></span>    |
|<span data-ttu-id="ed592-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ed592-114">Application</span></span> | <span data-ttu-id="ed592-115">Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ed592-115">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed592-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ed592-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ed592-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ed592-117">Optional query parameters</span></span>

<span data-ttu-id="ed592-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ed592-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ed592-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ed592-119">Request headers</span></span>
| <span data-ttu-id="ed592-120">名前</span><span class="sxs-lookup"><span data-stu-id="ed592-120">Name</span></span> | <span data-ttu-id="ed592-121">説明</span><span class="sxs-lookup"><span data-stu-id="ed592-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="ed592-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed592-122">Authorization</span></span>  | <span data-ttu-id="ed592-123">string</span><span class="sxs-lookup"><span data-stu-id="ed592-123">string</span></span>  | <span data-ttu-id="ed592-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ed592-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ed592-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ed592-126">Request body</span></span>

<span data-ttu-id="ed592-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ed592-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed592-128">応答</span><span class="sxs-lookup"><span data-stu-id="ed592-128">Response</span></span>

<span data-ttu-id="ed592-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[serviceprincipal](../resources/serviceprincipal.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="ed592-129">If successful, this method returns a `200 OK` response code and collection of [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed592-130">例</span><span class="sxs-lookup"><span data-stu-id="ed592-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ed592-131">要求</span><span class="sxs-lookup"><span data-stu-id="ed592-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ed592-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="ed592-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipals"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ed592-133">C#</span><span class="sxs-lookup"><span data-stu-id="ed592-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipals-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ed592-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ed592-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipals-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ed592-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="ed592-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipals-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ed592-136">応答</span><span class="sxs-lookup"><span data-stu-id="ed592-136">Response</span></span>

<span data-ttu-id="ed592-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ed592-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 488

{
  "value": [
    {
      "accountEnabled": true,
      "addIns": [
        {
          "id": "id-value",
          "type": "type-value",
          "properties": [
            {
              "key": "key-value",
              "value": "value-value"
            }
          ]
        }
      ],
      "appDisplayName": "appDisplayName-value",
      "appId": "appId-value",
      "appOwnerOrganizationId": "appOwnerOrganizationId-value",
      "appRoleAssignmentRequired": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List servicePrincipals",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
