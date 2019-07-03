---
title: 添付ファイルを一覧表示する
description: attachment オブジェクトのリストを取得します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 58e93e2ab3af94ea0126e49ebb1df527a92b1199
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35440912"
---
# <a name="list-attachments"></a><span data-ttu-id="42fb0-103">添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="42fb0-103">List attachments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42fb0-104">attachment オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="42fb0-104">Retrieve a list of attachment objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="42fb0-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="42fb0-105">Permissions</span></span>
<span data-ttu-id="42fb0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="42fb0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42fb0-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="42fb0-108">Permission type</span></span>      | <span data-ttu-id="42fb0-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="42fb0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42fb0-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="42fb0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="42fb0-111">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="42fb0-111">Mail.Read</span></span>    |
|<span data-ttu-id="42fb0-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="42fb0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42fb0-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="42fb0-113">Mail.Read</span></span>    |
|<span data-ttu-id="42fb0-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="42fb0-114">Application</span></span> | <span data-ttu-id="42fb0-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="42fb0-115">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="42fb0-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="42fb0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="42fb0-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="42fb0-117">Optional query parameters</span></span>
<span data-ttu-id="42fb0-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="42fb0-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="42fb0-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="42fb0-119">Request headers</span></span>
| <span data-ttu-id="42fb0-120">名前</span><span class="sxs-lookup"><span data-stu-id="42fb0-120">Name</span></span>       | <span data-ttu-id="42fb0-121">型</span><span class="sxs-lookup"><span data-stu-id="42fb0-121">Type</span></span> | <span data-ttu-id="42fb0-122">説明</span><span class="sxs-lookup"><span data-stu-id="42fb0-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="42fb0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="42fb0-123">Authorization</span></span>  | <span data-ttu-id="42fb0-124">string</span><span class="sxs-lookup"><span data-stu-id="42fb0-124">string</span></span>  | <span data-ttu-id="42fb0-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="42fb0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42fb0-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="42fb0-127">Request body</span></span>
<span data-ttu-id="42fb0-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="42fb0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42fb0-129">応答</span><span class="sxs-lookup"><span data-stu-id="42fb0-129">Response</span></span>

<span data-ttu-id="42fb0-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Attachment](../resources/attachment.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="42fb0-130">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="42fb0-131">例</span><span class="sxs-lookup"><span data-stu-id="42fb0-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="42fb0-132">要求</span><span class="sxs-lookup"><span data-stu-id="42fb0-132">Request</span></span>
<span data-ttu-id="42fb0-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="42fb0-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="42fb0-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="42fb0-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages/{id}/attachments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="42fb0-135">C#</span><span class="sxs-lookup"><span data-stu-id="42fb0-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-attachments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="42fb0-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="42fb0-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-attachments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="42fb0-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="42fb0-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-attachments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="42fb0-138">応答</span><span class="sxs-lookup"><span data-stu-id="42fb0-138">Response</span></span>
<span data-ttu-id="42fb0-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="42fb0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "isInline": false,
      "isContactPhoto": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
