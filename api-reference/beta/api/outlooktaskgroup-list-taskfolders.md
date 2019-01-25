---
title: リスト taskFolders
description: 特定の outlookTaskGroup では、Outlook の仕事フォルダーを取得します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 16a3463a7cdc4a3bc4efd401c7ca1a8932c82b7c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508287"
---
# <a name="list-taskfolders"></a><span data-ttu-id="bfe28-103">リスト taskFolders</span><span class="sxs-lookup"><span data-stu-id="bfe28-103">List taskFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bfe28-104">特定の[outlookTaskGroup](../resources/outlooktaskgroup.md)では、Outlook の仕事フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="bfe28-104">Get Outlook task folders in a specific [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="bfe28-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bfe28-105">Permissions</span></span>
<span data-ttu-id="bfe28-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bfe28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfe28-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bfe28-108">Permission type</span></span>      | <span data-ttu-id="bfe28-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bfe28-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bfe28-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bfe28-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bfe28-111">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="bfe28-111">Tasks.Read</span></span>    |
|<span data-ttu-id="bfe28-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bfe28-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bfe28-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="bfe28-113">Tasks.Read</span></span>    |
|<span data-ttu-id="bfe28-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bfe28-114">Application</span></span> | <span data-ttu-id="bfe28-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bfe28-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bfe28-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bfe28-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bfe28-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="bfe28-117">Optional query parameters</span></span>
<span data-ttu-id="bfe28-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="bfe28-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bfe28-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bfe28-119">Request headers</span></span>
| <span data-ttu-id="bfe28-120">名前</span><span class="sxs-lookup"><span data-stu-id="bfe28-120">Name</span></span>      |<span data-ttu-id="bfe28-121">説明</span><span class="sxs-lookup"><span data-stu-id="bfe28-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bfe28-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bfe28-122">Authorization</span></span>  | <span data-ttu-id="bfe28-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bfe28-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bfe28-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="bfe28-125">Request body</span></span>
<span data-ttu-id="bfe28-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="bfe28-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bfe28-127">応答</span><span class="sxs-lookup"><span data-stu-id="bfe28-127">Response</span></span>

<span data-ttu-id="bfe28-128">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[outlookTaskFolder](../resources/outlooktaskfolder.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="bfe28-128">If successful, this method returns a `200 OK` response code and collection of [outlookTaskFolder](../resources/outlooktaskfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bfe28-129">例</span><span class="sxs-lookup"><span data-stu-id="bfe28-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bfe28-130">要求</span><span class="sxs-lookup"><span data-stu-id="bfe28-130">Request</span></span>
<span data-ttu-id="bfe28-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bfe28-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_taskfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskGroups('AAMkADIyAAAhrbe-AAA=')/taskFolders
```
##### <a name="response"></a><span data-ttu-id="bfe28-132">応答</span><span class="sxs-lookup"><span data-stu-id="bfe28-132">Response</span></span>
<span data-ttu-id="bfe28-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bfe28-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "id": "AAMkADIyAAAhrbPXAAA=",
      "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAOlA==",
      "isDefaultFolder": false,
      "name": "Cooking",
      "parentGroupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"
    }

  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List taskFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktaskgroup-list-taskfolders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
