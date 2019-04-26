---
title: taskgroups を一覧表示する
description: ユーザーのメールボックス内のすべての Outlook タスクグループを取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7ec1d32d40c1d9478111fac937f5a72a01965e96
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337936"
---
# <a name="list-taskgroups"></a><span data-ttu-id="4debf-103">taskgroups を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="4debf-103">List taskGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4debf-104">ユーザーのメールボックス内のすべての Outlook タスクグループを取得します。</span><span class="sxs-lookup"><span data-stu-id="4debf-104">Get all the Outlook task groups in the user's mailbox.</span></span>

<span data-ttu-id="4debf-105">応答には常に、既定のタスク グループ `My Tasks` およびメールボックス内に作成されたその他のタスク グループが含まれます。</span><span class="sxs-lookup"><span data-stu-id="4debf-105">The response always includes the default task group `My Tasks`, and any other task groups that have been created in the mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="4debf-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4debf-106">Permissions</span></span>
<span data-ttu-id="4debf-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4debf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4debf-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4debf-109">Permission type</span></span>      | <span data-ttu-id="4debf-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4debf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4debf-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4debf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4debf-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="4debf-112">Tasks.Read</span></span>    |
|<span data-ttu-id="4debf-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4debf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4debf-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="4debf-114">Tasks.Read</span></span>    |
|<span data-ttu-id="4debf-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4debf-115">Application</span></span> | <span data-ttu-id="4debf-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4debf-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4debf-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4debf-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskGroups
GET /users/{id|userPrincipalName}/outlook/taskGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4debf-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="4debf-118">Optional query parameters</span></span>
<span data-ttu-id="4debf-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="4debf-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4debf-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4debf-120">Request headers</span></span>
| <span data-ttu-id="4debf-121">名前</span><span class="sxs-lookup"><span data-stu-id="4debf-121">Name</span></span>      |<span data-ttu-id="4debf-122">説明</span><span class="sxs-lookup"><span data-stu-id="4debf-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4debf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4debf-123">Authorization</span></span>  | <span data-ttu-id="4debf-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4debf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4debf-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="4debf-126">Request body</span></span>
<span data-ttu-id="4debf-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4debf-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4debf-128">応答</span><span class="sxs-lookup"><span data-stu-id="4debf-128">Response</span></span>

<span data-ttu-id="4debf-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[outlooktaskgroup](../resources/outlooktaskgroup.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="4debf-129">If successful, this method returns a `200 OK` response code and collection of [outlookTaskGroup](../resources/outlooktaskgroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4debf-130">例</span><span class="sxs-lookup"><span data-stu-id="4debf-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4debf-131">要求</span><span class="sxs-lookup"><span data-stu-id="4debf-131">Request</span></span>
<span data-ttu-id="4debf-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4debf-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_taskgroups"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskGroups
```
##### <a name="response"></a><span data-ttu-id="4debf-133">応答</span><span class="sxs-lookup"><span data-stu-id="4debf-133">Response</span></span>
<span data-ttu-id="4debf-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4debf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
