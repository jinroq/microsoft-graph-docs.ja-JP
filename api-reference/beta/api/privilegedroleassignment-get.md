---
title: privilegedRoleAssignment を取得する
description: PrivilegedRoleAssignment オブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
ms.openlocfilehash: 2a1c87f1693d0999221f62832851bdcb2c13f9f8
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35444982"
---
# <a name="get-privilegedroleassignment"></a><span data-ttu-id="a7d8e-103">privilegedRoleAssignment を取得する</span><span class="sxs-lookup"><span data-stu-id="a7d8e-103">Get privilegedRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7d8e-104">PrivilegedRoleAssignment オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="a7d8e-104">Retrieve the properties and relationships of privilegedRoleAssignment object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a7d8e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a7d8e-105">Permissions</span></span>
<span data-ttu-id="a7d8e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a7d8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a7d8e-108">リクエスターは、_特権の役割管理者_、_全体管理_者、_セキュリティ管理者_、または_セキュリティ閲覧_者のいずれかの役割を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a7d8e-108">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="a7d8e-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a7d8e-109">Permission type</span></span>      | <span data-ttu-id="a7d8e-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a7d8e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7d8e-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a7d8e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a7d8e-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a7d8e-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a7d8e-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a7d8e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7d8e-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a7d8e-114">Not supported.</span></span>    |
|<span data-ttu-id="a7d8e-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a7d8e-115">Application</span></span> | <span data-ttu-id="a7d8e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a7d8e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7d8e-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a7d8e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a7d8e-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a7d8e-118">Optional query parameters</span></span>
<span data-ttu-id="a7d8e-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a7d8e-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a7d8e-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a7d8e-120">Request headers</span></span>
| <span data-ttu-id="a7d8e-121">名前</span><span class="sxs-lookup"><span data-stu-id="a7d8e-121">Name</span></span>      |<span data-ttu-id="a7d8e-122">説明</span><span class="sxs-lookup"><span data-stu-id="a7d8e-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a7d8e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7d8e-123">Authorization</span></span>  | <span data-ttu-id="a7d8e-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a7d8e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a7d8e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a7d8e-126">Request body</span></span>
<span data-ttu-id="a7d8e-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a7d8e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7d8e-128">応答</span><span class="sxs-lookup"><span data-stu-id="a7d8e-128">Response</span></span>

<span data-ttu-id="a7d8e-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[privilegedRoleAssignment](../resources/privilegedroleassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a7d8e-129">If successful, this method returns a `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="a7d8e-130">テナントが PIM に登録されている必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="a7d8e-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="a7d8e-131">それ以外の場合、HTTP 403 の禁止状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="a7d8e-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="a7d8e-132">例</span><span class="sxs-lookup"><span data-stu-id="a7d8e-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a7d8e-133">要求</span><span class="sxs-lookup"><span data-stu-id="a7d8e-133">Request</span></span>
<span data-ttu-id="a7d8e-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a7d8e-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a7d8e-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="a7d8e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignment"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a7d8e-136">C#</span><span class="sxs-lookup"><span data-stu-id="a7d8e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a7d8e-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="a7d8e-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a7d8e-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="a7d8e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a7d8e-139">応答</span><span class="sxs-lookup"><span data-stu-id="a7d8e-139">Response</span></span>
<span data-ttu-id="a7d8e-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a7d8e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 184

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "isElevated": true,
  "expirationDateTime": "2016-10-19T10:37:00Z",
  "resultMessage": "resultMessage-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
