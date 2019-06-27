---
title: Update contactfolder
description: contactfolder オブジェクトのプロパティを更新します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 2b1459208f2ed99cb0d107ec9d4c9c034b6b7fc6
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273900"
---
# <a name="update-contactfolder"></a><span data-ttu-id="3e0bd-103">Update contactfolder</span><span class="sxs-lookup"><span data-stu-id="3e0bd-103">Update contactfolder</span></span>

<span data-ttu-id="3e0bd-104">contactfolder オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3e0bd-104">Update the properties of contactfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3e0bd-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3e0bd-105">Permissions</span></span>
<span data-ttu-id="3e0bd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3e0bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e0bd-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3e0bd-108">Permission type</span></span>      | <span data-ttu-id="3e0bd-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3e0bd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e0bd-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3e0bd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3e0bd-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3e0bd-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="3e0bd-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3e0bd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e0bd-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3e0bd-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="3e0bd-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3e0bd-114">Application</span></span> | <span data-ttu-id="3e0bd-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3e0bd-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e0bd-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3e0bd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/contactFolders/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3e0bd-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3e0bd-117">Request headers</span></span>
| <span data-ttu-id="3e0bd-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3e0bd-118">Header</span></span>       | <span data-ttu-id="3e0bd-119">値</span><span class="sxs-lookup"><span data-stu-id="3e0bd-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3e0bd-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e0bd-120">Authorization</span></span>  | <span data-ttu-id="3e0bd-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3e0bd-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3e0bd-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3e0bd-123">Content-Type</span></span>  | <span data-ttu-id="3e0bd-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="3e0bd-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3e0bd-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="3e0bd-126">Request body</span></span>
<span data-ttu-id="3e0bd-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="3e0bd-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3e0bd-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3e0bd-130">Property</span></span>     | <span data-ttu-id="3e0bd-131">型</span><span class="sxs-lookup"><span data-stu-id="3e0bd-131">Type</span></span>   |<span data-ttu-id="3e0bd-132">説明</span><span class="sxs-lookup"><span data-stu-id="3e0bd-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e0bd-133">displayName</span><span class="sxs-lookup"><span data-stu-id="3e0bd-133">displayName</span></span>|<span data-ttu-id="3e0bd-134">文字列</span><span class="sxs-lookup"><span data-stu-id="3e0bd-134">String</span></span>|<span data-ttu-id="3e0bd-135">フォルダーの表示名。</span><span class="sxs-lookup"><span data-stu-id="3e0bd-135">The folder's display name.</span></span>|
|<span data-ttu-id="3e0bd-136">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="3e0bd-136">parentFolderId</span></span>|<span data-ttu-id="3e0bd-137">String</span><span class="sxs-lookup"><span data-stu-id="3e0bd-137">String</span></span>|<span data-ttu-id="3e0bd-138">フォルダーの親フォルダーの ID。</span><span class="sxs-lookup"><span data-stu-id="3e0bd-138">The ID of the folder's parent folder.</span></span>|

## <a name="response"></a><span data-ttu-id="3e0bd-139">応答</span><span class="sxs-lookup"><span data-stu-id="3e0bd-139">Response</span></span>

<span data-ttu-id="3e0bd-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [contactFolder](../resources/contactfolder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3e0bd-140">If successful, this method returns a `200 OK` response code and updated [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3e0bd-141">例</span><span class="sxs-lookup"><span data-stu-id="3e0bd-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3e0bd-142">要求</span><span class="sxs-lookup"><span data-stu-id="3e0bd-142">Request</span></span>
<span data-ttu-id="3e0bd-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3e0bd-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_contactfolder"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/contactFolders/{id}
Content-type: application/json
Content-length: 84

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value"
}
```
##### <a name="response"></a><span data-ttu-id="3e0bd-144">応答</span><span class="sxs-lookup"><span data-stu-id="3e0bd-144">Response</span></span>
<span data-ttu-id="3e0bd-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3e0bd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 104

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value",
  "id": "id-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3e0bd-148">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="3e0bd-148">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3e0bd-149">C#</span><span class="sxs-lookup"><span data-stu-id="3e0bd-149">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_contactfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3e0bd-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="3e0bd-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_contactfolder-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3e0bd-151">目的-C</span><span class="sxs-lookup"><span data-stu-id="3e0bd-151">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_contactfolder-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update contactfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/contactfolder-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/contactfolder-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/contactfolder-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
