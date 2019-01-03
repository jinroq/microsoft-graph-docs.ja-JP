---
title: 上司を一覧表示する
description: ユーザーの上司を取得します。ユーザーの上司として割り当てられているユーザーまたは連絡先を返します。
ms.openlocfilehash: eb25449970311ceb7790b54c64191c669daeb004
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020226"
---
# <a name="list-manager"></a><span data-ttu-id="29c6f-104">上司を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="29c6f-104">List manager</span></span>

<span data-ttu-id="29c6f-p102">ユーザーの上司を取得します。ユーザーの上司として割り当てられているユーザーまたは連絡先を返します。</span><span class="sxs-lookup"><span data-stu-id="29c6f-p102">Get user's manager. Returns the user or contact assigned as the user's manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="29c6f-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="29c6f-107">Permissions</span></span>
<span data-ttu-id="29c6f-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="29c6f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29c6f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="29c6f-110">Permission type</span></span>      | <span data-ttu-id="29c6f-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="29c6f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29c6f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="29c6f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="29c6f-113">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="29c6f-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="29c6f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="29c6f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29c6f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29c6f-115">Not supported.</span></span>    |
|<span data-ttu-id="29c6f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="29c6f-116">Application</span></span> | <span data-ttu-id="29c6f-117">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29c6f-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="29c6f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="29c6f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/manager
```
## <a name="optional-query-parameters"></a><span data-ttu-id="29c6f-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="29c6f-119">Optional query parameters</span></span>
<span data-ttu-id="29c6f-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="29c6f-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="29c6f-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="29c6f-121">Request headers</span></span>
| <span data-ttu-id="29c6f-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="29c6f-122">Header</span></span>       | <span data-ttu-id="29c6f-123">値</span><span class="sxs-lookup"><span data-stu-id="29c6f-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="29c6f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="29c6f-124">Authorization</span></span>  | <span data-ttu-id="29c6f-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="29c6f-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="29c6f-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="29c6f-127">Content-Type</span></span>   | <span data-ttu-id="29c6f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="29c6f-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="29c6f-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="29c6f-129">Request body</span></span>
<span data-ttu-id="29c6f-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="29c6f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29c6f-131">応答</span><span class="sxs-lookup"><span data-stu-id="29c6f-131">Response</span></span>

<span data-ttu-id="29c6f-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="29c6f-132">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="29c6f-133">例</span><span class="sxs-lookup"><span data-stu-id="29c6f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="29c6f-134">要求</span><span class="sxs-lookup"><span data-stu-id="29c6f-134">Request</span></span>
<span data-ttu-id="29c6f-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="29c6f-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/manager
```
##### <a name="response"></a><span data-ttu-id="29c6f-136">応答</span><span class="sxs-lookup"><span data-stu-id="29c6f-136">Response</span></span>
<span data-ttu-id="29c6f-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="29c6f-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "objectType": "User",
  "id": "111048d2-2761-4347-b978-07354283363b",
  "accountEnabled": true,
  "city": "San Diego",
  "country": "United States",
  "department": "Sales & Marketing",
  "displayName": "Sara Davis",
  "givenName": "Sara",
  "jobTitle": "Finance VP",
  "mail": "SaraD@contoso.onmicrosoft.com",
  "mailNickname": "SaraD",
  "state": "CA",
  "streetAddress": "9256 Towne Center Dr., Suite 400",
  "surname": "Davis",
  "usageLocation": "US",
  "userPrincipalName": "SaraD@contoso.onmicrosoft.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->