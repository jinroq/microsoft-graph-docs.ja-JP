---
title: privilegedRole を取得する
description: 'PrivilegedRole オブジェクトのプロパティとリレーションシップを取得します。 '
localization_priority: Normal
ms.openlocfilehash: 2884c886bcf5327aaaa3af1a3972a9338e5a60a9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875865"
---
# <a name="get-privilegedrole"></a><span data-ttu-id="dacc3-103">privilegedRole を取得する</span><span class="sxs-lookup"><span data-stu-id="dacc3-103">Get privilegedRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dacc3-104">[PrivilegedRole](../resources/privilegedrole.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="dacc3-104">Retrieve the properties and relationships of [privilegedRole](../resources/privilegedrole.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="dacc3-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="dacc3-105">Permissions</span></span>
<span data-ttu-id="dacc3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dacc3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="dacc3-108">リクエスターは、_特権の役割管理者_、_全体管理_者、_セキュリティ管理者_、または_セキュリティ閲覧_者のいずれかの役割を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="dacc3-108">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="dacc3-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dacc3-109">Permission type</span></span>      | <span data-ttu-id="dacc3-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="dacc3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dacc3-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dacc3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dacc3-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dacc3-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dacc3-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dacc3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dacc3-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dacc3-114">Not supported.</span></span>    |
|<span data-ttu-id="dacc3-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dacc3-115">Application</span></span> | <span data-ttu-id="dacc3-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dacc3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dacc3-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dacc3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}
GET /privilegedRoleAssignments/{id}/roleInfo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dacc3-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="dacc3-118">Optional query parameters</span></span>
<span data-ttu-id="dacc3-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="dacc3-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dacc3-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dacc3-120">Request headers</span></span>
| <span data-ttu-id="dacc3-121">名前</span><span class="sxs-lookup"><span data-stu-id="dacc3-121">Name</span></span>      |<span data-ttu-id="dacc3-122">説明</span><span class="sxs-lookup"><span data-stu-id="dacc3-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dacc3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dacc3-123">Authorization</span></span>  | <span data-ttu-id="dacc3-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="dacc3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dacc3-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="dacc3-126">Request body</span></span>
<span data-ttu-id="dacc3-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="dacc3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dacc3-128">応答</span><span class="sxs-lookup"><span data-stu-id="dacc3-128">Response</span></span>

<span data-ttu-id="dacc3-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[privilegedRole](../resources/privilegedrole.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="dacc3-129">If successful, this method returns a `200 OK` response code and [privilegedRole](../resources/privilegedrole.md) object in the response body.</span></span>

<span data-ttu-id="dacc3-130">テナントが PIM に登録されている必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="dacc3-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="dacc3-131">それ以外の場合、HTTP 403 の禁止状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="dacc3-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="dacc3-132">例</span><span class="sxs-lookup"><span data-stu-id="dacc3-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dacc3-133">要求</span><span class="sxs-lookup"><span data-stu-id="dacc3-133">Request</span></span>
<span data-ttu-id="dacc3-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dacc3-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dacc3-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="dacc3-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedrole"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dacc3-136">C#</span><span class="sxs-lookup"><span data-stu-id="dacc3-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dacc3-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="dacc3-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dacc3-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="dacc3-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dacc3-139">Java</span><span class="sxs-lookup"><span data-stu-id="dacc3-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="dacc3-140">応答</span><span class="sxs-lookup"><span data-stu-id="dacc3-140">Response</span></span>
<span data-ttu-id="dacc3-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="dacc3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 46

{
  "id": "id-value",
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
