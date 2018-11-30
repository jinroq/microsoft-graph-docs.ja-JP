---
title: 添付ファイルを一覧表示する
description: 添付ファイル オブジェクトのリストを取得します。
ms.openlocfilehash: c9540db402a39cf8bf8f35318d06e7e699e9c7f6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023612"
---
# <a name="list-attachments"></a><span data-ttu-id="afdcf-103">添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="afdcf-103">List attachments</span></span>

<span data-ttu-id="afdcf-104">添付ファイル オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="afdcf-104">Retrieve a list of attachment objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="afdcf-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="afdcf-105">Permissions</span></span>
<span data-ttu-id="afdcf-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="afdcf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afdcf-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="afdcf-108">Permission type</span></span>      | <span data-ttu-id="afdcf-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="afdcf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="afdcf-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="afdcf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="afdcf-111">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="afdcf-111">Mail.Read</span></span>    |
|<span data-ttu-id="afdcf-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="afdcf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="afdcf-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="afdcf-113">Mail.Read</span></span>    |
|<span data-ttu-id="afdcf-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="afdcf-114">Application</span></span> | <span data-ttu-id="afdcf-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="afdcf-115">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="afdcf-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="afdcf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="afdcf-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="afdcf-117">Optional query parameters</span></span>
<span data-ttu-id="afdcf-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="afdcf-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="afdcf-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="afdcf-119">Request headers</span></span>
| <span data-ttu-id="afdcf-120">名前</span><span class="sxs-lookup"><span data-stu-id="afdcf-120">Name</span></span>       | <span data-ttu-id="afdcf-121">型</span><span class="sxs-lookup"><span data-stu-id="afdcf-121">Type</span></span> | <span data-ttu-id="afdcf-122">説明</span><span class="sxs-lookup"><span data-stu-id="afdcf-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="afdcf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="afdcf-123">Authorization</span></span>  | <span data-ttu-id="afdcf-124">string</span><span class="sxs-lookup"><span data-stu-id="afdcf-124">string</span></span>  | <span data-ttu-id="afdcf-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="afdcf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="afdcf-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="afdcf-127">Request body</span></span>
<span data-ttu-id="afdcf-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="afdcf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="afdcf-129">応答</span><span class="sxs-lookup"><span data-stu-id="afdcf-129">Response</span></span>

<span data-ttu-id="afdcf-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Attachment](../resources/attachment.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="afdcf-130">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="afdcf-131">例</span><span class="sxs-lookup"><span data-stu-id="afdcf-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="afdcf-132">要求</span><span class="sxs-lookup"><span data-stu-id="afdcf-132">Request</span></span>
<span data-ttu-id="afdcf-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="afdcf-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="afdcf-134">応答</span><span class="sxs-lookup"><span data-stu-id="afdcf-134">Response</span></span>
<span data-ttu-id="afdcf-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="afdcf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.attachment)",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "microsoft.graph.fileAttachment",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "base64-contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "datetime-value",
      "id": "id-value",
      "isInline": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
