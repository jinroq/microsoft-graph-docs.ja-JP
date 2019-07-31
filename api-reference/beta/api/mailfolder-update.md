---
title: MailFolder の更新
description: MailFolder オブジェクトのプロパティを更新します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 67932ad57b819348d25cf2777311727a8015bf10
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35984028"
---
# <a name="update-mailfolder"></a><span data-ttu-id="40b08-103">MailFolder の更新</span><span class="sxs-lookup"><span data-stu-id="40b08-103">Update mailFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40b08-104">[Mailfolder](../resources/mailfolder.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="40b08-104">Update the properties of [mailFolder](../resources/mailfolder.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="40b08-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="40b08-105">Permissions</span></span>
<span data-ttu-id="40b08-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="40b08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40b08-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="40b08-108">Permission type</span></span>      | <span data-ttu-id="40b08-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="40b08-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40b08-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="40b08-110">Delegated (work or school account)</span></span> | <span data-ttu-id="40b08-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="40b08-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="40b08-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="40b08-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40b08-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="40b08-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="40b08-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="40b08-114">Application</span></span> | <span data-ttu-id="40b08-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="40b08-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="40b08-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="40b08-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="40b08-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="40b08-117">Request headers</span></span>
| <span data-ttu-id="40b08-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="40b08-118">Header</span></span>       | <span data-ttu-id="40b08-119">値</span><span class="sxs-lookup"><span data-stu-id="40b08-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="40b08-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="40b08-120">Authorization</span></span>  | <span data-ttu-id="40b08-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="40b08-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="40b08-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="40b08-123">Content-Type</span></span>  | <span data-ttu-id="40b08-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="40b08-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="40b08-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="40b08-126">Request body</span></span>
<span data-ttu-id="40b08-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="40b08-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="40b08-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="40b08-130">Property</span></span>     | <span data-ttu-id="40b08-131">型</span><span class="sxs-lookup"><span data-stu-id="40b08-131">Type</span></span>   |<span data-ttu-id="40b08-132">説明</span><span class="sxs-lookup"><span data-stu-id="40b08-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40b08-133">displayName</span><span class="sxs-lookup"><span data-stu-id="40b08-133">displayName</span></span>|<span data-ttu-id="40b08-134">String</span><span class="sxs-lookup"><span data-stu-id="40b08-134">String</span></span>|<span data-ttu-id="40b08-135">mailFolder の表示名。</span><span class="sxs-lookup"><span data-stu-id="40b08-135">The mailFolder's display name.</span></span>|

## <a name="response"></a><span data-ttu-id="40b08-136">応答</span><span class="sxs-lookup"><span data-stu-id="40b08-136">Response</span></span>
<span data-ttu-id="40b08-137">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [mailFolder](../resources/mailfolder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="40b08-137">If successful, this method returns a `200 OK` response code and updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40b08-138">例</span><span class="sxs-lookup"><span data-stu-id="40b08-138">Example</span></span>
#### <a name="request"></a><span data-ttu-id="40b08-139">要求</span><span class="sxs-lookup"><span data-stu-id="40b08-139">Request</span></span>
<span data-ttu-id="40b08-140">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="40b08-140">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="40b08-141">プロトコル</span><span class="sxs-lookup"><span data-stu-id="40b08-141">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="40b08-142">C#</span><span class="sxs-lookup"><span data-stu-id="40b08-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="40b08-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="40b08-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="40b08-144">目的-C</span><span class="sxs-lookup"><span data-stu-id="40b08-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="40b08-145">Java</span><span class="sxs-lookup"><span data-stu-id="40b08-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-mailfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="40b08-146">応答</span><span class="sxs-lookup"><span data-stu-id="40b08-146">Response</span></span>
<span data-ttu-id="40b08-147">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="40b08-147">The following is an example of the response.</span></span>
><span data-ttu-id="40b08-148">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="40b08-148">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="40b08-149">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="40b08-149">All the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
