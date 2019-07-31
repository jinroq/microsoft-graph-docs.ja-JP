---
title: リスト privilegedRoles
description: PrivilegedRole オブジェクトのリストを取得します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4c2961e9f6a2ca628b240b4eae971b2c86d8aaa5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35978841"
---
# <a name="list-privilegedroles"></a><span data-ttu-id="cba07-103">リスト privilegedRoles</span><span class="sxs-lookup"><span data-stu-id="cba07-103">List privilegedRoles</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cba07-104">[PrivilegedRole](../resources/privilegedrole.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="cba07-104">Retrieve a list of [privilegedRole](../resources/privilegedrole.md) objects.</span></span>

<span data-ttu-id="cba07-105">クエリ結果をフィルター処理するには、URI で標準の OData ``$filter`` 式を使用します。</span><span class="sxs-lookup"><span data-stu-id="cba07-105">To filter the results from the query, use the standard OData ``$filter`` expressions in the URIs.</span></span>
## <a name="permissions"></a><span data-ttu-id="cba07-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cba07-106">Permissions</span></span>
<span data-ttu-id="cba07-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cba07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="cba07-109">リクエスターは、_特権の役割管理者_、_全体管理_者、_セキュリティ管理者_、または_セキュリティ閲覧_者のいずれかの役割を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cba07-109">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="cba07-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cba07-110">Permission type</span></span>      | <span data-ttu-id="cba07-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cba07-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cba07-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cba07-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cba07-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cba07-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cba07-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cba07-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cba07-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cba07-115">Not supported.</span></span>    |
|<span data-ttu-id="cba07-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cba07-116">Application</span></span> | <span data-ttu-id="cba07-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cba07-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cba07-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cba07-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cba07-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="cba07-119">Optional query parameters</span></span>
<span data-ttu-id="cba07-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="cba07-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cba07-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cba07-121">Request headers</span></span>
| <span data-ttu-id="cba07-122">名前</span><span class="sxs-lookup"><span data-stu-id="cba07-122">Name</span></span>      |<span data-ttu-id="cba07-123">説明</span><span class="sxs-lookup"><span data-stu-id="cba07-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cba07-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="cba07-124">Authorization</span></span>  | <span data-ttu-id="cba07-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cba07-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cba07-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="cba07-127">Request body</span></span>
<span data-ttu-id="cba07-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="cba07-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cba07-129">応答</span><span class="sxs-lookup"><span data-stu-id="cba07-129">Response</span></span>

<span data-ttu-id="cba07-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[privilegedRole](../resources/privilegedrole.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="cba07-130">If successful, this method returns a `200 OK` response code and collection of [privilegedRole](../resources/privilegedrole.md) objects in the response body.</span></span>

<span data-ttu-id="cba07-131">テナントが PIM に登録されている必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="cba07-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="cba07-132">それ以外の場合、HTTP 403 の禁止状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="cba07-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="cba07-133">例</span><span class="sxs-lookup"><span data-stu-id="cba07-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cba07-134">要求</span><span class="sxs-lookup"><span data-stu-id="cba07-134">Request</span></span>
<span data-ttu-id="cba07-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cba07-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cba07-136">プロトコル</span><span class="sxs-lookup"><span data-stu-id="cba07-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroles"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cba07-137">C#</span><span class="sxs-lookup"><span data-stu-id="cba07-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cba07-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="cba07-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cba07-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="cba07-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cba07-140">Java</span><span class="sxs-lookup"><span data-stu-id="cba07-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cba07-141">応答</span><span class="sxs-lookup"><span data-stu-id="cba07-141">Response</span></span>
<span data-ttu-id="cba07-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cba07-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRole",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 83

{
  "value": [
    {
      "id": "id-value",
      "name": "name-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List privilegedRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
