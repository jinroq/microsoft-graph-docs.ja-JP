---
title: privilegedApproval を一覧表示する
description: Privilegedapproval オブジェクトのリストを取得します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 9b030ccc69f0173fa6557ac691f3d0921be09c34
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36361244"
---
# <a name="list-privilegedapproval"></a><span data-ttu-id="d4a59-103">privilegedApproval を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="d4a59-103">List privilegedApproval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4a59-104">Privilegedapproval オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="d4a59-104">Retrieve a list of privilegedapproval objects.</span></span>

<span data-ttu-id="d4a59-105">クエリ結果をフィルター処理するには、URI で標準の OData ``$filter`` 式を使用します。</span><span class="sxs-lookup"><span data-stu-id="d4a59-105">To filter the results from the query, use the standard OData ``$filter`` expressions in the URIs.</span></span>
## <a name="permissions"></a><span data-ttu-id="d4a59-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d4a59-106">Permissions</span></span>
<span data-ttu-id="d4a59-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d4a59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d4a59-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d4a59-109">Permission type</span></span>      | <span data-ttu-id="d4a59-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d4a59-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d4a59-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d4a59-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d4a59-112">PrivilegedAccess、AzureAD、および Directory.accessasuser.all。</span><span class="sxs-lookup"><span data-stu-id="d4a59-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d4a59-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d4a59-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4a59-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d4a59-114">Not supported.</span></span>    |
|<span data-ttu-id="d4a59-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d4a59-115">Application</span></span> | <span data-ttu-id="d4a59-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d4a59-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4a59-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d4a59-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d4a59-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d4a59-118">Optional query parameters</span></span>
<span data-ttu-id="d4a59-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d4a59-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d4a59-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d4a59-120">Request headers</span></span>
| <span data-ttu-id="d4a59-121">名前</span><span class="sxs-lookup"><span data-stu-id="d4a59-121">Name</span></span>      |<span data-ttu-id="d4a59-122">説明</span><span class="sxs-lookup"><span data-stu-id="d4a59-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d4a59-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4a59-123">Authorization</span></span>  | <span data-ttu-id="d4a59-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d4a59-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d4a59-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d4a59-126">Request body</span></span>
<span data-ttu-id="d4a59-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d4a59-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4a59-128">応答</span><span class="sxs-lookup"><span data-stu-id="d4a59-128">Response</span></span>

<span data-ttu-id="d4a59-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[privilegedApproval](../resources/privilegedapproval.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="d4a59-129">If successful, this method returns a `200 OK` response code and collection of [privilegedApproval](../resources/privilegedapproval.md) objects in the response body.</span></span>

<span data-ttu-id="d4a59-130">テナントが PIM に登録されている必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="d4a59-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="d4a59-131">それ以外の場合、HTTP 403 の禁止状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="d4a59-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="d4a59-132">例</span><span class="sxs-lookup"><span data-stu-id="d4a59-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d4a59-133">要求</span><span class="sxs-lookup"><span data-stu-id="d4a59-133">Request</span></span>
<span data-ttu-id="d4a59-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d4a59-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d4a59-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="d4a59-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d4a59-136">C#</span><span class="sxs-lookup"><span data-stu-id="d4a59-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d4a59-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d4a59-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d4a59-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="d4a59-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d4a59-139">Java</span><span class="sxs-lookup"><span data-stu-id="d4a59-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedapproval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d4a59-140">応答</span><span class="sxs-lookup"><span data-stu-id="d4a59-140">Response</span></span>
<span data-ttu-id="d4a59-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d4a59-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 246

{
  "value": [
    {
      "id": "id-value",
      "userId": "userId-value",
      "roleId": "roleId-value",
      "approvalType": "approvalType-value",
      "approvalState": "approvalState-value",
      "approvalDuration": "datetime-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List privilegedApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
