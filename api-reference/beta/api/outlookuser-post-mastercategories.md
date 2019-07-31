---
title: Outlook カテゴリを作成する
description: ユーザーのマスター カテゴリ リスト内に outlookCategory オブジェクトを作成します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b459135a4de48b783ab5fc96506a08626041446b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35992508"
---
# <a name="create-outlook-category"></a><span data-ttu-id="0920b-103">Outlook カテゴリを作成する</span><span class="sxs-lookup"><span data-stu-id="0920b-103">Create Outlook category</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0920b-104">ユーザーのマスター カテゴリ リスト内に [outlookCategory](../resources/outlookcategory.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0920b-104">Create an [outlookCategory](../resources/outlookcategory.md) object in the user's master list of categories.</span></span>

## <a name="permissions"></a><span data-ttu-id="0920b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0920b-105">Permissions</span></span>
<span data-ttu-id="0920b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0920b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0920b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0920b-108">Permission type</span></span>      | <span data-ttu-id="0920b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0920b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0920b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0920b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0920b-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0920b-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="0920b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0920b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0920b-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0920b-113">MailboxSettings.ReadWrite</span></span>   |
|<span data-ttu-id="0920b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0920b-114">Application</span></span> | <span data-ttu-id="0920b-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0920b-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0920b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0920b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/masterCategories
POST /users/{id|userPrincipalName}/outlook/masterCategories
```
## <a name="request-headers"></a><span data-ttu-id="0920b-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0920b-117">Request headers</span></span>
| <span data-ttu-id="0920b-118">名前</span><span class="sxs-lookup"><span data-stu-id="0920b-118">Name</span></span>       | <span data-ttu-id="0920b-119">説明</span><span class="sxs-lookup"><span data-stu-id="0920b-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0920b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0920b-120">Authorization</span></span>  | <span data-ttu-id="0920b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0920b-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="0920b-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="0920b-123">Request body</span></span>
<span data-ttu-id="0920b-124">要求本文に、[outlookCategory](../resources/outlookcategory.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0920b-124">In the request body, supply a JSON representation of [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0920b-125">応答</span><span class="sxs-lookup"><span data-stu-id="0920b-125">Response</span></span>

<span data-ttu-id="0920b-126">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文に [outlookCategory](../resources/outlookcategory.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0920b-126">If successful, this method returns `201 Created` response code and [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0920b-127">例</span><span class="sxs-lookup"><span data-stu-id="0920b-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0920b-128">要求</span><span class="sxs-lookup"><span data-stu-id="0920b-128">Request</span></span>
<span data-ttu-id="0920b-129">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0920b-129">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0920b-130">プロトコル</span><span class="sxs-lookup"><span data-stu-id="0920b-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_outlookcategory_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/masterCategories
Content-type: application/json
Content-Length: 70

{
      "displayName":"Project expenses",
      "color":"preset9"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0920b-131">C#</span><span class="sxs-lookup"><span data-stu-id="0920b-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlookcategory-from-outlookuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0920b-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="0920b-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlookcategory-from-outlookuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0920b-133">目的-C</span><span class="sxs-lookup"><span data-stu-id="0920b-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlookcategory-from-outlookuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0920b-134">Java</span><span class="sxs-lookup"><span data-stu-id="0920b-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-outlookcategory-from-outlookuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="0920b-135">要求本文に、[outlookCategory](../resources/outlookcategory.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0920b-135">In the request body, supply a JSON representation of [outlookCategory](../resources/outlookcategory.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="0920b-136">応答</span><span class="sxs-lookup"><span data-stu-id="0920b-136">Response</span></span>
<span data-ttu-id="0920b-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0920b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 250

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"bac262b7-485d-4739-b436-e31467d64fac",
  "displayName":"Project expenses",
  "color":"preset9"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
