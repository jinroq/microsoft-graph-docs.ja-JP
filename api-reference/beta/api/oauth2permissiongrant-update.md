---
title: OAuth2PermissionGrant の更新
description: OAuth2PermissionGrant オブジェクトのプロパティを更新します。
localization_priority: Normal
ms.openlocfilehash: 6fd8e872a2eee7305026aae37aea15e19d3da3cd
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33597093"
---
# <a name="update-oauth2permissiongrant"></a><span data-ttu-id="3d9c4-103">OAuth2PermissionGrant の更新</span><span class="sxs-lookup"><span data-stu-id="3d9c4-103">Update oAuth2PermissionGrant</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d9c4-104">OAuth2PermissionGrant オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3d9c4-104">Update the properties of oAuth2PermissionGrant object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3d9c4-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3d9c4-105">Permissions</span></span>

<span data-ttu-id="3d9c4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3d9c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3d9c4-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3d9c4-108">Permission type</span></span>      | <span data-ttu-id="3d9c4-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3d9c4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d9c4-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3d9c4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3d9c4-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3d9c4-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3d9c4-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3d9c4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d9c4-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3d9c4-113">Not supported.</span></span>    |
|<span data-ttu-id="3d9c4-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3d9c4-114">Application</span></span> | <span data-ttu-id="3d9c4-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d9c4-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d9c4-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3d9c4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /oAuth2Permissiongrants/{id}
PATCH /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
PATCH /drive/root/createdByUser/oAuth2Permissiongrants/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3d9c4-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3d9c4-117">Request headers</span></span>
| <span data-ttu-id="3d9c4-118">名前</span><span class="sxs-lookup"><span data-stu-id="3d9c4-118">Name</span></span>       | <span data-ttu-id="3d9c4-119">型</span><span class="sxs-lookup"><span data-stu-id="3d9c4-119">Type</span></span> | <span data-ttu-id="3d9c4-120">説明</span><span class="sxs-lookup"><span data-stu-id="3d9c4-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3d9c4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d9c4-121">Authorization</span></span>  | <span data-ttu-id="3d9c4-122">string</span><span class="sxs-lookup"><span data-stu-id="3d9c4-122">string</span></span>  | <span data-ttu-id="3d9c4-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3d9c4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3d9c4-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="3d9c4-125">Request body</span></span>
<span data-ttu-id="3d9c4-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="3d9c4-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3d9c4-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3d9c4-129">Property</span></span>     | <span data-ttu-id="3d9c4-130">型</span><span class="sxs-lookup"><span data-stu-id="3d9c4-130">Type</span></span>   |<span data-ttu-id="3d9c4-131">説明</span><span class="sxs-lookup"><span data-stu-id="3d9c4-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3d9c4-132">scope</span><span class="sxs-lookup"><span data-stu-id="3d9c4-132">scope</span></span>|<span data-ttu-id="3d9c4-133">String</span><span class="sxs-lookup"><span data-stu-id="3d9c4-133">String</span></span>| <span data-ttu-id="3d9c4-134">OAuth 2.0 アクセストークンでリソースアプリケーションが想定するスコープ要求の値を指定します。</span><span class="sxs-lookup"><span data-stu-id="3d9c4-134">Specifies the value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="response"></a><span data-ttu-id="3d9c4-135">応答</span><span class="sxs-lookup"><span data-stu-id="3d9c4-135">Response</span></span>

<span data-ttu-id="3d9c4-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="3d9c4-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d9c4-138">例</span><span class="sxs-lookup"><span data-stu-id="3d9c4-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3d9c4-139">要求</span><span class="sxs-lookup"><span data-stu-id="3d9c4-139">Request</span></span>

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
##### <a name="response"></a><span data-ttu-id="3d9c4-140">応答</span><span class="sxs-lookup"><span data-stu-id="3d9c4-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3d9c4-141">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="3d9c4-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3d9c4-142">Visual</span><span class="sxs-lookup"><span data-stu-id="3d9c4-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_oAuth2Permissiongrant-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3d9c4-143">Java</span><span class="sxs-lookup"><span data-stu-id="3d9c4-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_oAuth2Permissiongrant-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/oauth2permissiongrant-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/oauth2permissiongrant-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
