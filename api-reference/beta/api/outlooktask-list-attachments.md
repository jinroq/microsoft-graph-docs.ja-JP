---
title: 添付ファイルを一覧表示する
description: Outlook のタスクに関連付けられている添付ファイルのオブジェクトの一覧を取得します。
author: angelgolfer-ms
ms.openlocfilehash: b998f6f7d3356728400cc7c609dd1014467ae4d6
ms.sourcegitcommit: 6b1ba9b3be038cd6247de54a255bad560034fe42
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/08/2019
ms.locfileid: "27771794"
---
# <a name="list-attachments"></a><span data-ttu-id="0f278-103">添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="0f278-103">List attachments</span></span>

> <span data-ttu-id="0f278-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0f278-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0f278-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0f278-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0f278-106">Outlook のタスクに関連付けられている[添付ファイル](../resources/attachment.md)のオブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="0f278-106">Get a list of [attachment](../resources/attachment.md) objects attached to an Outlook task.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f278-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0f278-107">Permissions</span></span>

<span data-ttu-id="0f278-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0f278-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f278-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0f278-110">Permission type</span></span>      | <span data-ttu-id="0f278-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0f278-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0f278-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0f278-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0f278-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="0f278-113">Tasks.Read</span></span>    |
|<span data-ttu-id="0f278-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0f278-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f278-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="0f278-115">Tasks.Read</span></span>    |
|<span data-ttu-id="0f278-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0f278-116">Application</span></span> | <span data-ttu-id="0f278-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0f278-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f278-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0f278-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}/attachments
GET /users/{id|userPrincipalName}/outlook/tasks/{id}/attachments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0f278-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="0f278-119">Optional query parameters</span></span>

<span data-ttu-id="0f278-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="0f278-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0f278-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0f278-121">Request headers</span></span>

| <span data-ttu-id="0f278-122">名前</span><span class="sxs-lookup"><span data-stu-id="0f278-122">Name</span></span>      |<span data-ttu-id="0f278-123">説明</span><span class="sxs-lookup"><span data-stu-id="0f278-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0f278-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f278-124">Authorization</span></span>  | <span data-ttu-id="0f278-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0f278-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0f278-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="0f278-127">Request body</span></span>

<span data-ttu-id="0f278-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0f278-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f278-129">応答</span><span class="sxs-lookup"><span data-stu-id="0f278-129">Response</span></span>

<span data-ttu-id="0f278-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の[添付ファイル](../resources/attachment.md)のオブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="0f278-130">If successful, this method returns a `200 OK` response code and collection of [attachment](../resources/attachment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f278-131">例</span><span class="sxs-lookup"><span data-stu-id="0f278-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f278-132">要求</span><span class="sxs-lookup"><span data-stu-id="0f278-132">Request</span></span>

<span data-ttu-id="0f278-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0f278-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->

```http
GET https://graph.microsoft.com/beta/users/{id}/outlook/tasks/{id}/attachments
```

### <a name="response"></a><span data-ttu-id="0f278-134">応答</span><span class="sxs-lookup"><span data-stu-id="0f278-134">Response</span></span>

<span data-ttu-id="0f278-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0f278-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->