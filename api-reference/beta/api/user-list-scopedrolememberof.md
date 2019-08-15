---
title: scopedAdministratorOf を一覧表示する
description: ユーザーの scopedRoleMembership の一覧を取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 66f697f1b4b19b3aaa8032ba87919a6dc24c92e2
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36422032"
---
# <a name="list-scopedadministratorof"></a><span data-ttu-id="fb169-103">scopedAdministratorOf を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="fb169-103">List scopedAdministratorOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb169-104">ユーザーの[scopedRoleMembership](../resources/scopedrolemembership.md)の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="fb169-104">Retrieve a list of [scopedRoleMembership](../resources/scopedrolemembership.md) for the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="fb169-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fb169-105">Permissions</span></span>
<span data-ttu-id="fb169-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fb169-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fb169-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fb169-108">Permission type</span></span>      | <span data-ttu-id="fb169-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fb169-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb169-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fb169-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fb169-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fb169-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fb169-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fb169-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb169-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fb169-113">Not supported.</span></span>    |
|<span data-ttu-id="fb169-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fb169-114">Application</span></span> | <span data-ttu-id="fb169-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb169-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fb169-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fb169-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/scopedAdministratorOf
GET /users/{id}/scopedAdministratorOf

```
## <a name="optional-query-parameters"></a><span data-ttu-id="fb169-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="fb169-117">Optional query parameters</span></span>
<span data-ttu-id="fb169-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="fb169-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fb169-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fb169-119">Request headers</span></span>
| <span data-ttu-id="fb169-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fb169-120">Header</span></span>       | <span data-ttu-id="fb169-121">値</span><span class="sxs-lookup"><span data-stu-id="fb169-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fb169-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb169-122">Authorization</span></span>  | <span data-ttu-id="fb169-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fb169-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fb169-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="fb169-125">Request body</span></span>
<span data-ttu-id="fb169-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="fb169-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb169-127">応答</span><span class="sxs-lookup"><span data-stu-id="fb169-127">Response</span></span>

<span data-ttu-id="fb169-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[scopedRoleMembership](../resources/scopedrolemembership.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="fb169-128">If successful, this method returns a `200 OK` response code and collection of [scopedRoleMembership](../resources/scopedrolemembership.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fb169-129">例</span><span class="sxs-lookup"><span data-stu-id="fb169-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fb169-130">要求</span><span class="sxs-lookup"><span data-stu-id="fb169-130">Request</span></span>
<span data-ttu-id="fb169-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fb169-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fb169-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="fb169-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_scopedadministratorof"
}-->
```http
GET https://graph.microsoft.com/beta/me/scopedAdministratorOf
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fb169-133">C#</span><span class="sxs-lookup"><span data-stu-id="fb169-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-scopedadministratorof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fb169-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fb169-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-scopedadministratorof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fb169-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="fb169-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-scopedadministratorof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fb169-136">応答</span><span class="sxs-lookup"><span data-stu-id="fb169-136">Response</span></span>
<span data-ttu-id="fb169-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fb169-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedRoleMembership",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 307

{
  "value": [
    {
      "roleId": "roleId-value",
      "administrativeUnitId": "administrativeUnitId-value",
      "roleMemberInfo": {
        "id": "id-value",
        "displayName": "displayName-value",
        "userPrincipalName": "userPrincipalName-value"
      },
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List scopedAdministratorOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
