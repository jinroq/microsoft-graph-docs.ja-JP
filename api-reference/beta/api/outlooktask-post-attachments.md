---
title: 添付ファイルの作成
description: この API を使用して、outlookTask に添付ファイルを追加します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 7d0ab132b119b12e5c7359551642009d389da05f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35265780"
---
# <a name="create-attachment"></a><span data-ttu-id="683da-103">添付ファイルを作成する</span><span class="sxs-lookup"><span data-stu-id="683da-103">Create attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="683da-104">この API を使用して、 [Outlooktask](../resources/outlooktask.md)に[添付ファイル](../resources/attachment.md)を追加します。</span><span class="sxs-lookup"><span data-stu-id="683da-104">Use this API to add an [attachment](../resources/attachment.md) to an [outlookTask](../resources/outlooktask.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="683da-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="683da-105">Permissions</span></span>

<span data-ttu-id="683da-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="683da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="683da-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="683da-108">Permission type</span></span>      | <span data-ttu-id="683da-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="683da-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="683da-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="683da-110">Delegated (work or school account)</span></span> | <span data-ttu-id="683da-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="683da-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="683da-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="683da-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="683da-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="683da-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="683da-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="683da-114">Application</span></span> | <span data-ttu-id="683da-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="683da-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="683da-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="683da-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/outlook/tasks/{id}/attachments
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/attachments
```

## <a name="request-headers"></a><span data-ttu-id="683da-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="683da-117">Request headers</span></span>

| <span data-ttu-id="683da-118">名前</span><span class="sxs-lookup"><span data-stu-id="683da-118">Name</span></span>       | <span data-ttu-id="683da-119">説明</span><span class="sxs-lookup"><span data-stu-id="683da-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="683da-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="683da-120">Authorization</span></span>  | <span data-ttu-id="683da-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="683da-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="683da-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="683da-123">Content-Type</span></span> | <span data-ttu-id="683da-124">エンティティの本文に含まれるデータの種類を表す文字列。</span><span class="sxs-lookup"><span data-stu-id="683da-124">A string that represents the type of data in the body of an entity.</span></span> <span data-ttu-id="683da-125">必須です。</span><span class="sxs-lookup"><span data-stu-id="683da-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="683da-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="683da-126">Request body</span></span>

<span data-ttu-id="683da-127">要求本文で、[attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="683da-127">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="683da-128">応答</span><span class="sxs-lookup"><span data-stu-id="683da-128">Response</span></span>

<span data-ttu-id="683da-129">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [attachment](../resources/attachment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="683da-129">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="683da-130">例</span><span class="sxs-lookup"><span data-stu-id="683da-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="683da-131">要求</span><span class="sxs-lookup"><span data-stu-id="683da-131">Request</span></span>

<span data-ttu-id="683da-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="683da-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_attachment_from_outlooktask"
}-->

```http
POST https://graph.microsoft.com/beta/users/{id}/outlook/tasks/{id}/attachments
Content-type: application/json
Content-length: 142

{
  "lastModifiedDateTime": "datetime-value",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true
}
```

### <a name="response"></a><span data-ttu-id="683da-133">応答</span><span class="sxs-lookup"><span data-stu-id="683da-133">Response</span></span>

<span data-ttu-id="683da-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="683da-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 162

{
  "lastModifiedDateTime": "datetime-value",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="683da-137">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="683da-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="683da-138">C#</span><span class="sxs-lookup"><span data-stu-id="683da-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_attachment_from_outlooktask-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="683da-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="683da-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_attachment_from_outlooktask-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="683da-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="683da-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_attachment_from_outlooktask-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktask-post-attachments.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/outlooktask-post-attachments.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/outlooktask-post-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
