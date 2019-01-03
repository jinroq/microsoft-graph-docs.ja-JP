---
title: OAuth2PermissionGrant を更新します。
description: OAuth2PermissionGrant オブジェクトのプロパティを更新します。
ms.openlocfilehash: fdf196e672b19a2775644dada4a33b036df83bf8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067486"
---
# <a name="update-oauth2permissiongrant"></a><span data-ttu-id="6f450-103">OAuth2PermissionGrant を更新します。</span><span class="sxs-lookup"><span data-stu-id="6f450-103">Update oAuth2PermissionGrant</span></span>

> <span data-ttu-id="6f450-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6f450-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6f450-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6f450-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6f450-106">OAuth2PermissionGrant オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6f450-106">Update the properties of oAuth2PermissionGrant object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f450-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6f450-107">Permissions</span></span>

<span data-ttu-id="6f450-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6f450-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6f450-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6f450-110">Permission type</span></span>      | <span data-ttu-id="6f450-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6f450-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f450-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6f450-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6f450-113">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6f450-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6f450-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6f450-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f450-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6f450-115">Not supported.</span></span>    |
|<span data-ttu-id="6f450-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6f450-116">Application</span></span> | <span data-ttu-id="6f450-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f450-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f450-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6f450-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /oAuth2Permissiongrants/{id}
PATCH /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
PATCH /drive/root/createdByUser/oAuth2Permissiongrants/{id}
```
## <a name="request-headers"></a><span data-ttu-id="6f450-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6f450-119">Request headers</span></span>
| <span data-ttu-id="6f450-120">名前</span><span class="sxs-lookup"><span data-stu-id="6f450-120">Name</span></span>       | <span data-ttu-id="6f450-121">型</span><span class="sxs-lookup"><span data-stu-id="6f450-121">Type</span></span> | <span data-ttu-id="6f450-122">説明</span><span class="sxs-lookup"><span data-stu-id="6f450-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6f450-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f450-123">Authorization</span></span>  | <span data-ttu-id="6f450-124">string</span><span class="sxs-lookup"><span data-stu-id="6f450-124">string</span></span>  | <span data-ttu-id="6f450-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6f450-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6f450-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="6f450-127">Request body</span></span>
<span data-ttu-id="6f450-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="6f450-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6f450-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6f450-131">Property</span></span>     | <span data-ttu-id="6f450-132">型</span><span class="sxs-lookup"><span data-stu-id="6f450-132">Type</span></span>   |<span data-ttu-id="6f450-133">説明</span><span class="sxs-lookup"><span data-stu-id="6f450-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6f450-134">scope</span><span class="sxs-lookup"><span data-stu-id="6f450-134">scope</span></span>|<span data-ttu-id="6f450-135">String</span><span class="sxs-lookup"><span data-stu-id="6f450-135">String</span></span>| <span data-ttu-id="6f450-136">OAuth 2.0 のアクセス トークンには、リソース アプリケーションが期待するスコープの要求の値を指定します。</span><span class="sxs-lookup"><span data-stu-id="6f450-136">Specifies the value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="response"></a><span data-ttu-id="6f450-137">応答</span><span class="sxs-lookup"><span data-stu-id="6f450-137">Response</span></span>

<span data-ttu-id="6f450-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="6f450-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f450-140">例</span><span class="sxs-lookup"><span data-stu-id="6f450-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6f450-141">要求</span><span class="sxs-lookup"><span data-stu-id="6f450-141">Request</span></span>

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
##### <a name="response"></a><span data-ttu-id="6f450-142">応答</span><span class="sxs-lookup"><span data-stu-id="6f450-142">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update oAuth2Permissiongrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->