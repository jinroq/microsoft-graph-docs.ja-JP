---
title: 添付ファイルを一覧表示する
description: Outlook のタスクに関連付けられている添付ファイルのオブジェクトの一覧を取得します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 9d330f0a86b99bbd667ff1f32a5b5fc549dfc7f2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526908"
---
# <a name="list-attachments"></a><span data-ttu-id="f3973-103">添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="f3973-103">List attachments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3973-104">Outlook のタスクに関連付けられている[添付ファイル](../resources/attachment.md)のオブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="f3973-104">Get a list of [attachment](../resources/attachment.md) objects attached to an Outlook task.</span></span>

## <a name="permissions"></a><span data-ttu-id="f3973-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f3973-105">Permissions</span></span>

<span data-ttu-id="f3973-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f3973-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3973-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f3973-108">Permission type</span></span>      | <span data-ttu-id="f3973-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f3973-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3973-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f3973-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f3973-111">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="f3973-111">Tasks.Read</span></span>    |
|<span data-ttu-id="f3973-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f3973-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3973-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="f3973-113">Tasks.Read</span></span>    |
|<span data-ttu-id="f3973-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f3973-114">Application</span></span> | <span data-ttu-id="f3973-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3973-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3973-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f3973-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}/attachments
GET /users/{id|userPrincipalName}/outlook/tasks/{id}/attachments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f3973-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f3973-117">Optional query parameters</span></span>

<span data-ttu-id="f3973-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f3973-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f3973-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f3973-119">Request headers</span></span>

| <span data-ttu-id="f3973-120">名前</span><span class="sxs-lookup"><span data-stu-id="f3973-120">Name</span></span>      |<span data-ttu-id="f3973-121">説明</span><span class="sxs-lookup"><span data-stu-id="f3973-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f3973-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3973-122">Authorization</span></span>  | <span data-ttu-id="f3973-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f3973-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f3973-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="f3973-125">Request body</span></span>

<span data-ttu-id="f3973-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f3973-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3973-127">応答</span><span class="sxs-lookup"><span data-stu-id="f3973-127">Response</span></span>

<span data-ttu-id="f3973-128">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の[添付ファイル](../resources/attachment.md)のオブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="f3973-128">If successful, this method returns a `200 OK` response code and collection of [attachment](../resources/attachment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3973-129">例</span><span class="sxs-lookup"><span data-stu-id="f3973-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3973-130">要求</span><span class="sxs-lookup"><span data-stu-id="f3973-130">Request</span></span>

<span data-ttu-id="f3973-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f3973-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->

```http
GET https://graph.microsoft.com/beta/users/{id}/outlook/tasks/{id}/attachments
```

### <a name="response"></a><span data-ttu-id="f3973-132">応答</span><span class="sxs-lookup"><span data-stu-id="f3973-132">Response</span></span>

<span data-ttu-id="f3973-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f3973-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "lastModifiedDateTime": "datetime-value",
      "name": "name-value",
      "contentType": "contentType-value",
      "size": 99,
      "isInline": true,
      "id": "id-value"
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
    "Error: /api-reference/beta/api/outlooktask-list-attachments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
