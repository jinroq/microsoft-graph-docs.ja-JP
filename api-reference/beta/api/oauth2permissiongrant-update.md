---
title: OAuth2PermissionGrant の更新
description: OAuth2PermissionGrant オブジェクトのプロパティを更新します。
localization_priority: Normal
ms.openlocfilehash: b54254123b38865e16e9fb5780c06effd538a970
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878936"
---
# <a name="update-oauth2permissiongrant"></a><span data-ttu-id="75842-103">OAuth2PermissionGrant の更新</span><span class="sxs-lookup"><span data-stu-id="75842-103">Update oAuth2PermissionGrant</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75842-104">OAuth2PermissionGrant オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="75842-104">Update the properties of oAuth2PermissionGrant object.</span></span>

## <a name="permissions"></a><span data-ttu-id="75842-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="75842-105">Permissions</span></span>

<span data-ttu-id="75842-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="75842-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="75842-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="75842-108">Permission type</span></span>      | <span data-ttu-id="75842-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="75842-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75842-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="75842-110">Delegated (work or school account)</span></span> | <span data-ttu-id="75842-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="75842-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="75842-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="75842-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75842-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="75842-113">Not supported.</span></span>    |
|<span data-ttu-id="75842-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="75842-114">Application</span></span> | <span data-ttu-id="75842-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75842-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="75842-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="75842-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /oAuth2Permissiongrants/{id}
PATCH /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
PATCH /drive/root/createdByUser/oAuth2Permissiongrants/{id}
```
## <a name="request-headers"></a><span data-ttu-id="75842-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="75842-117">Request headers</span></span>
| <span data-ttu-id="75842-118">名前</span><span class="sxs-lookup"><span data-stu-id="75842-118">Name</span></span>       | <span data-ttu-id="75842-119">型</span><span class="sxs-lookup"><span data-stu-id="75842-119">Type</span></span> | <span data-ttu-id="75842-120">説明</span><span class="sxs-lookup"><span data-stu-id="75842-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="75842-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="75842-121">Authorization</span></span>  | <span data-ttu-id="75842-122">string</span><span class="sxs-lookup"><span data-stu-id="75842-122">string</span></span>  | <span data-ttu-id="75842-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="75842-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="75842-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="75842-125">Request body</span></span>
<span data-ttu-id="75842-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="75842-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="75842-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="75842-129">Property</span></span>     | <span data-ttu-id="75842-130">型</span><span class="sxs-lookup"><span data-stu-id="75842-130">Type</span></span>   |<span data-ttu-id="75842-131">説明</span><span class="sxs-lookup"><span data-stu-id="75842-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75842-132">scope</span><span class="sxs-lookup"><span data-stu-id="75842-132">scope</span></span>|<span data-ttu-id="75842-133">String</span><span class="sxs-lookup"><span data-stu-id="75842-133">String</span></span>| <span data-ttu-id="75842-134">OAuth 2.0 アクセストークンでリソースアプリケーションが想定するスコープ要求の値を指定します。</span><span class="sxs-lookup"><span data-stu-id="75842-134">Specifies the value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="response"></a><span data-ttu-id="75842-135">応答</span><span class="sxs-lookup"><span data-stu-id="75842-135">Response</span></span>

<span data-ttu-id="75842-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="75842-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75842-138">例</span><span class="sxs-lookup"><span data-stu-id="75842-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="75842-139">要求</span><span class="sxs-lookup"><span data-stu-id="75842-139">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="75842-140">プロトコル</span><span class="sxs-lookup"><span data-stu-id="75842-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_oAuth2Permissiongrant"
}-->
```http
PATCH https://graph.microsoft.com/beta/oAuth2Permissiongrants/{id}
Content-type: application/json
Content-length: 30

{
  "scope": "scope-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="75842-141">C#</span><span class="sxs-lookup"><span data-stu-id="75842-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="75842-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="75842-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="75842-143">目的-C</span><span class="sxs-lookup"><span data-stu-id="75842-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="75842-144">Java</span><span class="sxs-lookup"><span data-stu-id="75842-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-oauth2permissiongrant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="75842-145">応答</span><span class="sxs-lookup"><span data-stu-id="75842-145">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update oAuth2Permissiongrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
