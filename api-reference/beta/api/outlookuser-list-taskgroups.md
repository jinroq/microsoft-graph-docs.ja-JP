---
title: TaskGroups を一覧表示する
description: ユーザーのメールボックス内のすべての Outlook タスクグループを取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: fc6bdcbc99b682e792218d9d09e066e72cd834f1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349689"
---
# <a name="list-taskgroups"></a><span data-ttu-id="2566f-103">TaskGroups を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="2566f-103">List taskGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2566f-104">ユーザーのメールボックス内のすべての Outlook タスクグループを取得します。</span><span class="sxs-lookup"><span data-stu-id="2566f-104">Get all the Outlook task groups in the user's mailbox.</span></span>

<span data-ttu-id="2566f-105">応答には常に、既定のタスク グループ `My Tasks` およびメールボックス内に作成されたその他のタスク グループが含まれます。</span><span class="sxs-lookup"><span data-stu-id="2566f-105">The response always includes the default task group `My Tasks`, and any other task groups that have been created in the mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="2566f-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2566f-106">Permissions</span></span>
<span data-ttu-id="2566f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2566f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2566f-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2566f-109">Permission type</span></span>      | <span data-ttu-id="2566f-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2566f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2566f-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2566f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2566f-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="2566f-112">Tasks.Read</span></span>    |
|<span data-ttu-id="2566f-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2566f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2566f-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="2566f-114">Tasks.Read</span></span>    |
|<span data-ttu-id="2566f-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2566f-115">Application</span></span> | <span data-ttu-id="2566f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2566f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2566f-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2566f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskGroups
GET /users/{id|userPrincipalName}/outlook/taskGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2566f-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2566f-118">Optional query parameters</span></span>
<span data-ttu-id="2566f-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2566f-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2566f-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2566f-120">Request headers</span></span>
| <span data-ttu-id="2566f-121">名前</span><span class="sxs-lookup"><span data-stu-id="2566f-121">Name</span></span>      |<span data-ttu-id="2566f-122">説明</span><span class="sxs-lookup"><span data-stu-id="2566f-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2566f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2566f-123">Authorization</span></span>  | <span data-ttu-id="2566f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2566f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2566f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="2566f-126">Request body</span></span>
<span data-ttu-id="2566f-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2566f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2566f-128">応答</span><span class="sxs-lookup"><span data-stu-id="2566f-128">Response</span></span>

<span data-ttu-id="2566f-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[outlooktaskgroup](../resources/outlooktaskgroup.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="2566f-129">If successful, this method returns a `200 OK` response code and collection of [outlookTaskGroup](../resources/outlooktaskgroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2566f-130">例</span><span class="sxs-lookup"><span data-stu-id="2566f-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2566f-131">要求</span><span class="sxs-lookup"><span data-stu-id="2566f-131">Request</span></span>
<span data-ttu-id="2566f-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2566f-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2566f-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="2566f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_taskgroups"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskGroups
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2566f-134">C#</span><span class="sxs-lookup"><span data-stu-id="2566f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-taskgroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2566f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2566f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-taskgroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2566f-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="2566f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-taskgroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2566f-137">Java</span><span class="sxs-lookup"><span data-stu-id="2566f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-taskgroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2566f-138">応答</span><span class="sxs-lookup"><span data-stu-id="2566f-138">Response</span></span>
<span data-ttu-id="2566f-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2566f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskGroup",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 187

{
  "value": [
    {
      "id": "AAMkADIyAAADJ5pYAAA=",
      "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAInHxLA==",
      "isDefaultGroup": true,
      "name": "My Tasks",
      "groupKey": "0006f0b7-0000-0000-c000-000000000046"
    },
    {
      "id": "AAMkADIyAAAhrbe-AAA=",
      "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAInHxKw==",
      "isDefaultGroup": false,
      "name": "Leisure Tasks",
      "groupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"
    }

  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List TaskGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
