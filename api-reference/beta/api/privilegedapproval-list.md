---
title: privilegedApproval を一覧表示する
description: Privilegedapproval オブジェクトのリストを取得します。
localization_priority: Normal
ms.openlocfilehash: b2b9c71ec45033cb9fbf209cdcc97a20fd2f891e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35445087"
---
# <a name="list-privilegedapproval"></a><span data-ttu-id="4ee8f-103">privilegedApproval を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="4ee8f-103">List privilegedApproval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ee8f-104">Privilegedapproval オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="4ee8f-104">Retrieve a list of privilegedapproval objects.</span></span>

<span data-ttu-id="4ee8f-105">クエリ結果をフィルター処理するには、URI で標準の OData ``$filter`` 式を使用します。</span><span class="sxs-lookup"><span data-stu-id="4ee8f-105">To filter the results from the query, use the standard OData ``$filter`` expressions in the URIs.</span></span>
## <a name="permissions"></a><span data-ttu-id="4ee8f-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4ee8f-106">Permissions</span></span>
<span data-ttu-id="4ee8f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4ee8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4ee8f-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4ee8f-109">Permission type</span></span>      | <span data-ttu-id="4ee8f-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4ee8f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ee8f-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4ee8f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4ee8f-112">PrivilegedAccess、AzureAD、および Directory.accessasuser.all。</span><span class="sxs-lookup"><span data-stu-id="4ee8f-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4ee8f-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4ee8f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ee8f-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4ee8f-114">Not supported.</span></span>    |
|<span data-ttu-id="4ee8f-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4ee8f-115">Application</span></span> | <span data-ttu-id="4ee8f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4ee8f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ee8f-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4ee8f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4ee8f-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="4ee8f-118">Optional query parameters</span></span>
<span data-ttu-id="4ee8f-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="4ee8f-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4ee8f-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4ee8f-120">Request headers</span></span>
| <span data-ttu-id="4ee8f-121">名前</span><span class="sxs-lookup"><span data-stu-id="4ee8f-121">Name</span></span>      |<span data-ttu-id="4ee8f-122">説明</span><span class="sxs-lookup"><span data-stu-id="4ee8f-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4ee8f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ee8f-123">Authorization</span></span>  | <span data-ttu-id="4ee8f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4ee8f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ee8f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="4ee8f-126">Request body</span></span>
<span data-ttu-id="4ee8f-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4ee8f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ee8f-128">応答</span><span class="sxs-lookup"><span data-stu-id="4ee8f-128">Response</span></span>

<span data-ttu-id="4ee8f-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[privilegedApproval](../resources/privilegedapproval.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="4ee8f-129">If successful, this method returns a `200 OK` response code and collection of [privilegedApproval](../resources/privilegedapproval.md) objects in the response body.</span></span>

<span data-ttu-id="4ee8f-130">テナントが PIM に登録されている必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="4ee8f-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="4ee8f-131">それ以外の場合、HTTP 403 の禁止状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="4ee8f-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="4ee8f-132">例</span><span class="sxs-lookup"><span data-stu-id="4ee8f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4ee8f-133">要求</span><span class="sxs-lookup"><span data-stu-id="4ee8f-133">Request</span></span>
<span data-ttu-id="4ee8f-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4ee8f-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4ee8f-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="4ee8f-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4ee8f-136">C#</span><span class="sxs-lookup"><span data-stu-id="4ee8f-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4ee8f-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="4ee8f-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4ee8f-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="4ee8f-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4ee8f-139">応答</span><span class="sxs-lookup"><span data-stu-id="4ee8f-139">Response</span></span>
<span data-ttu-id="4ee8f-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4ee8f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
