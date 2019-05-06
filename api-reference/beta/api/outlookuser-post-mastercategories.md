---
title: Outlook カテゴリを作成する
description: ユーザーのマスター カテゴリ リスト内に outlookCategory オブジェクトを作成します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 4b80a7794430bcfb82f11f515959a96027458d0a
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33596069"
---
# <a name="create-outlook-category"></a><span data-ttu-id="e1581-103">Outlook カテゴリを作成する</span><span class="sxs-lookup"><span data-stu-id="e1581-103">Create Outlook category</span></span>


<span data-ttu-id="e1581-104">ユーザーのマスター カテゴリ リスト内に [outlookCategory](../resources/outlookcategory.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e1581-104">Create an [outlookCategory](../resources/outlookcategory.md) object in the user's master list of categories.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1581-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e1581-105">Permissions</span></span>
<span data-ttu-id="e1581-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e1581-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1581-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e1581-108">Permission type</span></span>      | <span data-ttu-id="e1581-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e1581-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1581-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e1581-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e1581-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1581-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="e1581-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e1581-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1581-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1581-113">MailboxSettings.ReadWrite</span></span>   |
|<span data-ttu-id="e1581-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e1581-114">Application</span></span> | <span data-ttu-id="e1581-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1581-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1581-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e1581-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/masterCategories
POST /users/{id|userPrincipalName}/outlook/masterCategories
```
## <a name="request-headers"></a><span data-ttu-id="e1581-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e1581-117">Request headers</span></span>
| <span data-ttu-id="e1581-118">名前</span><span class="sxs-lookup"><span data-stu-id="e1581-118">Name</span></span>       | <span data-ttu-id="e1581-119">説明</span><span class="sxs-lookup"><span data-stu-id="e1581-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e1581-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1581-120">Authorization</span></span>  | <span data-ttu-id="e1581-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e1581-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="e1581-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="e1581-123">Request body</span></span>
<span data-ttu-id="e1581-124">要求本文に、[outlookCategory](../resources/outlookcategory.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e1581-124">In the request body, supply a JSON representation of [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e1581-125">応答</span><span class="sxs-lookup"><span data-stu-id="e1581-125">Response</span></span>

<span data-ttu-id="e1581-126">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文に [outlookCategory](../resources/outlookcategory.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e1581-126">If successful, this method returns `201 Created` response code and [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1581-127">例</span><span class="sxs-lookup"><span data-stu-id="e1581-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e1581-128">要求</span><span class="sxs-lookup"><span data-stu-id="e1581-128">Request</span></span>
<span data-ttu-id="e1581-129">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e1581-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_outlookcategory_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/outlook/masterCategories
Content-type: application/json
Content-Length: 70

{
      "displayName":"Project expenses",
      "color":"preset9"
}
```
<span data-ttu-id="e1581-130">要求本文に、[outlookCategory](../resources/outlookcategory.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e1581-130">In the request body, supply a JSON representation of [outlookCategory](../resources/outlookcategory.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e1581-131">応答</span><span class="sxs-lookup"><span data-stu-id="e1581-131">Response</span></span>
<span data-ttu-id="e1581-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e1581-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"bac262b7-485d-4739-b436-e31467d64fac",
  "displayName":"Project expenses",
  "color":"preset9"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e1581-135">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="e1581-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e1581-136">Visual</span><span class="sxs-lookup"><span data-stu-id="e1581-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_outlookcategory_from_outlookuser-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e1581-137">Java</span><span class="sxs-lookup"><span data-stu-id="e1581-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_outlookcategory_from_outlookuser-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/outlookuser-post-mastercategories.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/outlookuser-post-mastercategories.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
