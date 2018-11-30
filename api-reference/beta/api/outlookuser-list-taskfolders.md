---
title: リスト taskFolders
description: ユーザーのメールボックス内のすべての Outlook タスク フォルダーを取得します。
ms.openlocfilehash: 5c5636af9abe46b67d29fa03ae39d3020173849a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068693"
---
# <a name="list-taskfolders"></a><span data-ttu-id="c10a6-103">リスト taskFolders</span><span class="sxs-lookup"><span data-stu-id="c10a6-103">List taskFolders</span></span>

> <span data-ttu-id="c10a6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c10a6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c10a6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c10a6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c10a6-106">ユーザーのメールボックス内のすべての Outlook タスク フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="c10a6-106">Get all the Outlook task folders in the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="c10a6-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c10a6-107">Permissions</span></span>
<span data-ttu-id="c10a6-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c10a6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c10a6-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c10a6-110">Permission type</span></span>      | <span data-ttu-id="c10a6-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c10a6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c10a6-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c10a6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c10a6-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="c10a6-113">Tasks.Read</span></span>    |
|<span data-ttu-id="c10a6-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c10a6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c10a6-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="c10a6-115">Tasks.Read</span></span>    |
|<span data-ttu-id="c10a6-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c10a6-116">Application</span></span> | <span data-ttu-id="c10a6-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c10a6-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c10a6-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c10a6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id|userPrincipalName}/outlook/taskFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c10a6-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c10a6-119">Optional query parameters</span></span>
<span data-ttu-id="c10a6-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c10a6-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c10a6-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c10a6-121">Request headers</span></span>
| <span data-ttu-id="c10a6-122">名前</span><span class="sxs-lookup"><span data-stu-id="c10a6-122">Name</span></span>      |<span data-ttu-id="c10a6-123">説明</span><span class="sxs-lookup"><span data-stu-id="c10a6-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c10a6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c10a6-124">Authorization</span></span>  | <span data-ttu-id="c10a6-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c10a6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c10a6-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c10a6-127">Request body</span></span>
<span data-ttu-id="c10a6-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c10a6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c10a6-129">応答</span><span class="sxs-lookup"><span data-stu-id="c10a6-129">Response</span></span>

<span data-ttu-id="c10a6-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[outlookTaskFolder](../resources/outlooktaskfolder.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="c10a6-130">If successful, this method returns a `200 OK` response code and collection of [outlookTaskFolder](../resources/outlooktaskfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c10a6-131">例</span><span class="sxs-lookup"><span data-stu-id="c10a6-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c10a6-132">要求</span><span class="sxs-lookup"><span data-stu-id="c10a6-132">Request</span></span>
<span data-ttu-id="c10a6-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c10a6-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_taskfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskFolders
```
##### <a name="response"></a><span data-ttu-id="c10a6-134">応答</span><span class="sxs-lookup"><span data-stu-id="c10a6-134">Response</span></span>
<span data-ttu-id="c10a6-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c10a6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 200

{
  "value": [
   {
      "id": "AAMkADIyAAAAABrJAAA=",
      "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAAAAeAA==",
      "isDefaultFolder": false,
      "name": "Monthly tasks",
      "parentGroupKey": "0006f0b7-0000-0000-c000-000000000046"
    },
    {
      "id": "AAMkADIyAAAAAAESAAA=",
      "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAAAAAPA==",
      "isDefaultFolder": true,
      "name": "Tasks",
      "parentGroupKey": "0006f0b7-0000-0000-c000-000000000046"
    }

  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List TaskFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->