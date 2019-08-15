---
title: privilegedApproval を一覧表示する
description: Privilegedapproval オブジェクトのリストを取得します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 53f344d92de141ff5df27c95db92133dde199112
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412888"
---
# <a name="list-privilegedapproval"></a><span data-ttu-id="32f0c-103">privilegedApproval を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="32f0c-103">List privilegedApproval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32f0c-104">Privilegedapproval オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="32f0c-104">Retrieve a list of privilegedapproval objects.</span></span>

<span data-ttu-id="32f0c-105">クエリ結果をフィルター処理するには、URI で標準の OData ``$filter`` 式を使用します。</span><span class="sxs-lookup"><span data-stu-id="32f0c-105">To filter the results from the query, use the standard OData ``$filter`` expressions in the URIs.</span></span>
## <a name="permissions"></a><span data-ttu-id="32f0c-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="32f0c-106">Permissions</span></span>
<span data-ttu-id="32f0c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="32f0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="32f0c-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="32f0c-109">Permission type</span></span>      | <span data-ttu-id="32f0c-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="32f0c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32f0c-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="32f0c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="32f0c-112">PrivilegedAccess、AzureAD、および Directory.accessasuser.all。</span><span class="sxs-lookup"><span data-stu-id="32f0c-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="32f0c-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="32f0c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32f0c-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="32f0c-114">Not supported.</span></span>    |
|<span data-ttu-id="32f0c-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="32f0c-115">Application</span></span> | <span data-ttu-id="32f0c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="32f0c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="32f0c-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="32f0c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval
```
## <a name="optional-query-parameters"></a><span data-ttu-id="32f0c-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="32f0c-118">Optional query parameters</span></span>
<span data-ttu-id="32f0c-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="32f0c-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="32f0c-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="32f0c-120">Request headers</span></span>
| <span data-ttu-id="32f0c-121">名前</span><span class="sxs-lookup"><span data-stu-id="32f0c-121">Name</span></span>      |<span data-ttu-id="32f0c-122">説明</span><span class="sxs-lookup"><span data-stu-id="32f0c-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="32f0c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="32f0c-123">Authorization</span></span>  | <span data-ttu-id="32f0c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="32f0c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="32f0c-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="32f0c-126">Request body</span></span>
<span data-ttu-id="32f0c-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="32f0c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32f0c-128">応答</span><span class="sxs-lookup"><span data-stu-id="32f0c-128">Response</span></span>

<span data-ttu-id="32f0c-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[privilegedApproval](../resources/privilegedapproval.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="32f0c-129">If successful, this method returns a `200 OK` response code and collection of [privilegedApproval](../resources/privilegedapproval.md) objects in the response body.</span></span>

<span data-ttu-id="32f0c-130">テナントが PIM に登録されている必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="32f0c-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="32f0c-131">それ以外の場合、HTTP 403 の禁止状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="32f0c-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="32f0c-132">例</span><span class="sxs-lookup"><span data-stu-id="32f0c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="32f0c-133">要求</span><span class="sxs-lookup"><span data-stu-id="32f0c-133">Request</span></span>
<span data-ttu-id="32f0c-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="32f0c-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="32f0c-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="32f0c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="32f0c-136">C#</span><span class="sxs-lookup"><span data-stu-id="32f0c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="32f0c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32f0c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="32f0c-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="32f0c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="32f0c-139">応答</span><span class="sxs-lookup"><span data-stu-id="32f0c-139">Response</span></span>
<span data-ttu-id="32f0c-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="32f0c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
