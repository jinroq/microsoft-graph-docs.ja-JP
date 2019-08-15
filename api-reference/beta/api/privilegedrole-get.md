---
title: privilegedRole を取得する
description: 'PrivilegedRole オブジェクトのプロパティとリレーションシップを取得します。 '
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: a366130529de2c06273f34e8fc336c7ad433a8f8
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412818"
---
# <a name="get-privilegedrole"></a><span data-ttu-id="5411c-103">privilegedRole を取得する</span><span class="sxs-lookup"><span data-stu-id="5411c-103">Get privilegedRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5411c-104">[PrivilegedRole](../resources/privilegedrole.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="5411c-104">Retrieve the properties and relationships of [privilegedRole](../resources/privilegedrole.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="5411c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5411c-105">Permissions</span></span>
<span data-ttu-id="5411c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5411c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="5411c-108">リクエスターは、_特権の役割管理者_、_全体管理_者、_セキュリティ管理者_、または_セキュリティ閲覧_者のいずれかの役割を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5411c-108">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="5411c-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5411c-109">Permission type</span></span>      | <span data-ttu-id="5411c-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5411c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5411c-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5411c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5411c-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5411c-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5411c-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5411c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5411c-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5411c-114">Not supported.</span></span>    |
|<span data-ttu-id="5411c-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5411c-115">Application</span></span> | <span data-ttu-id="5411c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5411c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5411c-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5411c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}
GET /privilegedRoleAssignments/{id}/roleInfo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5411c-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="5411c-118">Optional query parameters</span></span>
<span data-ttu-id="5411c-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5411c-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5411c-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5411c-120">Request headers</span></span>
| <span data-ttu-id="5411c-121">名前</span><span class="sxs-lookup"><span data-stu-id="5411c-121">Name</span></span>      |<span data-ttu-id="5411c-122">説明</span><span class="sxs-lookup"><span data-stu-id="5411c-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5411c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5411c-123">Authorization</span></span>  | <span data-ttu-id="5411c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5411c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5411c-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="5411c-126">Request body</span></span>
<span data-ttu-id="5411c-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5411c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5411c-128">応答</span><span class="sxs-lookup"><span data-stu-id="5411c-128">Response</span></span>

<span data-ttu-id="5411c-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[privilegedRole](../resources/privilegedrole.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5411c-129">If successful, this method returns a `200 OK` response code and [privilegedRole](../resources/privilegedrole.md) object in the response body.</span></span>

<span data-ttu-id="5411c-130">テナントが PIM に登録されている必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="5411c-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="5411c-131">それ以外の場合、HTTP 403 の禁止状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="5411c-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="5411c-132">例</span><span class="sxs-lookup"><span data-stu-id="5411c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5411c-133">要求</span><span class="sxs-lookup"><span data-stu-id="5411c-133">Request</span></span>
<span data-ttu-id="5411c-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5411c-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5411c-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="5411c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedrole"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5411c-136">C#</span><span class="sxs-lookup"><span data-stu-id="5411c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5411c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5411c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5411c-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="5411c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5411c-139">応答</span><span class="sxs-lookup"><span data-stu-id="5411c-139">Response</span></span>
<span data-ttu-id="5411c-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5411c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
