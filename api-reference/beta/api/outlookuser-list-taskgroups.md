---
title: TaskGroups のリスト
description: ユーザーのメールボックス内のすべての Outlook のタスク グループを取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: ba8e0982fabcc9a82ae3ba2ec3b9f34b1655932b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511094"
---
# <a name="list-taskgroups"></a><span data-ttu-id="b6480-103">TaskGroups のリスト</span><span class="sxs-lookup"><span data-stu-id="b6480-103">List taskGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6480-104">ユーザーのメールボックス内のすべての Outlook のタスク グループを取得します。</span><span class="sxs-lookup"><span data-stu-id="b6480-104">Get all the Outlook task groups in the user's mailbox.</span></span>

<span data-ttu-id="b6480-105">応答には常に、既定のタスク グループ `My Tasks` およびメールボックス内に作成されたその他のタスク グループが含まれます。</span><span class="sxs-lookup"><span data-stu-id="b6480-105">The response always includes the default task group `My Tasks`, and any other task groups that have been created in the mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="b6480-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b6480-106">Permissions</span></span>
<span data-ttu-id="b6480-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b6480-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6480-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b6480-109">Permission type</span></span>      | <span data-ttu-id="b6480-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b6480-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6480-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b6480-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b6480-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="b6480-112">Tasks.Read</span></span>    |
|<span data-ttu-id="b6480-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b6480-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6480-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="b6480-114">Tasks.Read</span></span>    |
|<span data-ttu-id="b6480-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b6480-115">Application</span></span> | <span data-ttu-id="b6480-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b6480-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b6480-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b6480-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id|userPrincipalName}/outlook/taskGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b6480-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b6480-118">Optional query parameters</span></span>
<span data-ttu-id="b6480-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b6480-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b6480-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b6480-120">Request headers</span></span>
| <span data-ttu-id="b6480-121">名前</span><span class="sxs-lookup"><span data-stu-id="b6480-121">Name</span></span>      |<span data-ttu-id="b6480-122">説明</span><span class="sxs-lookup"><span data-stu-id="b6480-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b6480-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6480-123">Authorization</span></span>  | <span data-ttu-id="b6480-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b6480-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b6480-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="b6480-126">Request body</span></span>
<span data-ttu-id="b6480-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b6480-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6480-128">応答</span><span class="sxs-lookup"><span data-stu-id="b6480-128">Response</span></span>

<span data-ttu-id="b6480-129">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[outlookTaskGroup](../resources/outlooktaskgroup.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="b6480-129">If successful, this method returns a `200 OK` response code and collection of [outlookTaskGroup](../resources/outlooktaskgroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b6480-130">例</span><span class="sxs-lookup"><span data-stu-id="b6480-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b6480-131">要求</span><span class="sxs-lookup"><span data-stu-id="b6480-131">Request</span></span>
<span data-ttu-id="b6480-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b6480-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_taskgroups"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskGroups
```
##### <a name="response"></a><span data-ttu-id="b6480-133">応答</span><span class="sxs-lookup"><span data-stu-id="b6480-133">Response</span></span>
<span data-ttu-id="b6480-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b6480-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/outlookuser-list-taskgroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
