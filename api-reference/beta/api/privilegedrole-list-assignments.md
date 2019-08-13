---
title: 割り当てを一覧表示する
description: ロールに関連付けられている privilegedRoleAssignment オブジェクトのリストを取得します。 各 privilegedRoleAssignment はユーザーに対するロールの割り当てを表します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 15fe4000cab7cc4925ddb9eac798e9fc768cf185
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36361269"
---
# <a name="list-assignments"></a><span data-ttu-id="02962-104">割り当てを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="02962-104">List assignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02962-105">ロールに関連付けられている[privilegedRoleAssignment](../resources/privilegedroleassignment.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="02962-105">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects that are associated with the role.</span></span> <span data-ttu-id="02962-106">各[privilegedRoleAssignment](../resources/privilegedroleassignment.md)は、ユーザーへの役割の割り当てを表します。</span><span class="sxs-lookup"><span data-stu-id="02962-106">Each [privilegedRoleAssignment](../resources/privilegedroleassignment.md) represents a role assignment to a user.</span></span>
## <a name="permissions"></a><span data-ttu-id="02962-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="02962-107">Permissions</span></span>
<span data-ttu-id="02962-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="02962-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="02962-110">リクエスターは、_特権の役割管理者_、_全体管理_者、_セキュリティ管理者_、または_セキュリティ閲覧_者のいずれかの役割を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="02962-110">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="02962-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="02962-111">Permission type</span></span>      | <span data-ttu-id="02962-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="02962-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02962-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="02962-113">Delegated (work or school account)</span></span> | <span data-ttu-id="02962-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="02962-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="02962-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="02962-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02962-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02962-116">Not supported.</span></span>    |
|<span data-ttu-id="02962-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="02962-117">Application</span></span> | <span data-ttu-id="02962-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02962-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="02962-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="02962-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/assignments
```

<span data-ttu-id="02962-120">これは``<id>`` 、ターゲットの役割 id であることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="02962-120">Note that ``<id>`` is the target role id.</span></span>
## <a name="optional-query-parameters"></a><span data-ttu-id="02962-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="02962-121">Optional query parameters</span></span>
<span data-ttu-id="02962-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="02962-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="02962-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="02962-123">Request headers</span></span>
| <span data-ttu-id="02962-124">名前</span><span class="sxs-lookup"><span data-stu-id="02962-124">Name</span></span>      |<span data-ttu-id="02962-125">説明</span><span class="sxs-lookup"><span data-stu-id="02962-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="02962-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="02962-126">Authorization</span></span>  | <span data-ttu-id="02962-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="02962-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="02962-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="02962-129">Request body</span></span>
<span data-ttu-id="02962-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="02962-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02962-131">応答</span><span class="sxs-lookup"><span data-stu-id="02962-131">Response</span></span>

<span data-ttu-id="02962-132">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[privilegedRoleAssignment](../resources/privilegedroleassignment.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="02962-132">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="02962-133">テナントが PIM に登録されている必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="02962-133">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="02962-134">それ以外の場合、HTTP 403 の禁止状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="02962-134">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="02962-135">例</span><span class="sxs-lookup"><span data-stu-id="02962-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="02962-136">要求</span><span class="sxs-lookup"><span data-stu-id="02962-136">Request</span></span>
<span data-ttu-id="02962-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="02962-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="02962-138">プロトコル</span><span class="sxs-lookup"><span data-stu-id="02962-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_assignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/assignments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="02962-139">C#</span><span class="sxs-lookup"><span data-stu-id="02962-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-assignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="02962-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02962-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-assignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="02962-141">目的-C</span><span class="sxs-lookup"><span data-stu-id="02962-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-assignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="02962-142">Java</span><span class="sxs-lookup"><span data-stu-id="02962-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-assignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="02962-143">応答</span><span class="sxs-lookup"><span data-stu-id="02962-143">Response</span></span>
<span data-ttu-id="02962-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="02962-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
    {
      "id": "id-value",
      "userId": "userId-value",
      "roleId": "roleId-value",
      "isElevated": true,
      "expirationDateTime": "2016-10-19T10:37:00Z",
      "resultMessage": "resultMessage-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List assignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
