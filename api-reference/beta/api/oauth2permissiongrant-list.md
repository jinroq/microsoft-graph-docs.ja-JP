---
title: oauth2PermissionGrants を一覧表示する
description: Oauth2PermissionGrant オブジェクトのリストを取得します。
localization_priority: Normal
ms.openlocfilehash: b6ec733c73d281e64978b11ebdf3c43d9eb94378
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878913"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="6d1f6-103">oauth2PermissionGrants を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="6d1f6-103">List oauth2PermissionGrants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d1f6-104">Oauth2PermissionGrant オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="6d1f6-104">Retrieve a list of oauth2PermissionGrant objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d1f6-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6d1f6-105">Permissions</span></span>

<span data-ttu-id="6d1f6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6d1f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6d1f6-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6d1f6-108">Permission type</span></span>      | <span data-ttu-id="6d1f6-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6d1f6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d1f6-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6d1f6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6d1f6-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6d1f6-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6d1f6-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6d1f6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d1f6-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6d1f6-113">Not supported.</span></span>    |
|<span data-ttu-id="6d1f6-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6d1f6-114">Application</span></span> | <span data-ttu-id="6d1f6-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d1f6-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d1f6-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6d1f6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /oauth2PermissionGrants
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6d1f6-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6d1f6-117">Optional query parameters</span></span>
<span data-ttu-id="6d1f6-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6d1f6-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6d1f6-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6d1f6-119">Request headers</span></span>
| <span data-ttu-id="6d1f6-120">名前</span><span class="sxs-lookup"><span data-stu-id="6d1f6-120">Name</span></span> | <span data-ttu-id="6d1f6-121">説明</span><span class="sxs-lookup"><span data-stu-id="6d1f6-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="6d1f6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d1f6-122">Authorization</span></span>  | <span data-ttu-id="6d1f6-123">string</span><span class="sxs-lookup"><span data-stu-id="6d1f6-123">string</span></span>  | <span data-ttu-id="6d1f6-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6d1f6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6d1f6-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="6d1f6-126">Request body</span></span>
<span data-ttu-id="6d1f6-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6d1f6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d1f6-128">応答</span><span class="sxs-lookup"><span data-stu-id="6d1f6-128">Response</span></span>

<span data-ttu-id="6d1f6-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[oAuth2PermissionGrant](../resources/oauth2permissiongrant.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="6d1f6-129">If successful, this method returns a `200 OK` response code and collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6d1f6-130">例</span><span class="sxs-lookup"><span data-stu-id="6d1f6-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6d1f6-131">要求</span><span class="sxs-lookup"><span data-stu-id="6d1f6-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6d1f6-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="6d1f6-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_oauth2permissiongrants"
}-->
```http
GET https://graph.microsoft.com/beta/oauth2PermissionGrants
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6d1f6-133">C#</span><span class="sxs-lookup"><span data-stu-id="6d1f6-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-oauth2permissiongrants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6d1f6-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="6d1f6-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-oauth2permissiongrants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6d1f6-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="6d1f6-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-oauth2permissiongrants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6d1f6-136">Java</span><span class="sxs-lookup"><span data-stu-id="6d1f6-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-oauth2permissiongrants-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6d1f6-137">応答</span><span class="sxs-lookup"><span data-stu-id="6d1f6-137">Response</span></span>

<span data-ttu-id="6d1f6-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6d1f6-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 259

{
  "value": [
    {
      "clientId": "clientId-value",
      "consentType": "consentType-value",
      "expiryTime": "datetime-value",
      "id": "id-value",
      "principalId": "principalId-value",
      "resourceId": "resourceId-value",
      "scope": "scope-value",
      "startTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List oauth2PermissionGrants",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
