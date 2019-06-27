---
title: MailFolder の更新
description: MailFolder オブジェクトのプロパティを更新します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 4cada1bcec35bbdf098537a692e196f53e06cebe
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266627"
---
# <a name="update-mailfolder"></a><span data-ttu-id="cfe56-103">MailFolder の更新</span><span class="sxs-lookup"><span data-stu-id="cfe56-103">Update mailFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cfe56-104">[Mailfolder](../resources/mailfolder.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="cfe56-104">Update the properties of [mailFolder](../resources/mailfolder.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cfe56-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cfe56-105">Permissions</span></span>
<span data-ttu-id="cfe56-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cfe56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfe56-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cfe56-108">Permission type</span></span>      | <span data-ttu-id="cfe56-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cfe56-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cfe56-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cfe56-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cfe56-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cfe56-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="cfe56-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cfe56-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cfe56-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cfe56-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="cfe56-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cfe56-114">Application</span></span> | <span data-ttu-id="cfe56-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cfe56-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="cfe56-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cfe56-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cfe56-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cfe56-117">Request headers</span></span>
| <span data-ttu-id="cfe56-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cfe56-118">Header</span></span>       | <span data-ttu-id="cfe56-119">値</span><span class="sxs-lookup"><span data-stu-id="cfe56-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cfe56-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="cfe56-120">Authorization</span></span>  | <span data-ttu-id="cfe56-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cfe56-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cfe56-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cfe56-123">Content-Type</span></span>  | <span data-ttu-id="cfe56-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="cfe56-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cfe56-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="cfe56-126">Request body</span></span>
<span data-ttu-id="cfe56-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="cfe56-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="cfe56-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cfe56-130">Property</span></span>     | <span data-ttu-id="cfe56-131">型</span><span class="sxs-lookup"><span data-stu-id="cfe56-131">Type</span></span>   |<span data-ttu-id="cfe56-132">説明</span><span class="sxs-lookup"><span data-stu-id="cfe56-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cfe56-133">displayName</span><span class="sxs-lookup"><span data-stu-id="cfe56-133">displayName</span></span>|<span data-ttu-id="cfe56-134">String</span><span class="sxs-lookup"><span data-stu-id="cfe56-134">String</span></span>|<span data-ttu-id="cfe56-135">mailFolder の表示名。</span><span class="sxs-lookup"><span data-stu-id="cfe56-135">The mailFolder's display name.</span></span>|

## <a name="response"></a><span data-ttu-id="cfe56-136">応答</span><span class="sxs-lookup"><span data-stu-id="cfe56-136">Response</span></span>
<span data-ttu-id="cfe56-137">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [mailFolder](../resources/mailfolder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="cfe56-137">If successful, this method returns a `200 OK` response code and updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cfe56-138">例</span><span class="sxs-lookup"><span data-stu-id="cfe56-138">Example</span></span>
#### <a name="request"></a><span data-ttu-id="cfe56-139">要求</span><span class="sxs-lookup"><span data-stu-id="cfe56-139">Request</span></span>
<span data-ttu-id="cfe56-140">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cfe56-140">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_mailfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```

#### <a name="response"></a><span data-ttu-id="cfe56-141">応答</span><span class="sxs-lookup"><span data-stu-id="cfe56-141">Response</span></span>
<span data-ttu-id="cfe56-142">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cfe56-142">The following is an example of the response.</span></span>
><span data-ttu-id="cfe56-143">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="cfe56-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cfe56-144">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="cfe56-144">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
    "id": "AAMkAGVmMDEzM",
    "displayName": "displayName-value",
    "parentFolderId": "AAMkAGVmMDEzI",
    "childFolderCount": 2,
    "unreadItemCount": 59,
    "totalItemCount": 60,
    "wellKnownName": "inbox"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="cfe56-145">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="cfe56-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="cfe56-146">C#</span><span class="sxs-lookup"><span data-stu-id="cfe56-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_mailfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cfe56-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="cfe56-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_mailfolder-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="cfe56-148">目的-C</span><span class="sxs-lookup"><span data-stu-id="cfe56-148">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_mailfolder-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update mailfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/mailfolder-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/mailfolder-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/mailfolder-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
