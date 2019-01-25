---
title: OutlookTaskGroup を取得します。
description: プロパティと指定した Outlook のタスク グループの関係を取得します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: d113c913be669df4735c902f261b0ce3f77c67c9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513096"
---
# <a name="get-outlooktaskgroup"></a><span data-ttu-id="86470-103">OutlookTaskGroup を取得します。</span><span class="sxs-lookup"><span data-stu-id="86470-103">Get outlookTaskGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86470-104">プロパティと指定した Outlook のタスク グループの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="86470-104">Get the properties and relationships of the specified Outlook task group.</span></span>
## <a name="permissions"></a><span data-ttu-id="86470-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="86470-105">Permissions</span></span>
<span data-ttu-id="86470-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="86470-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86470-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="86470-108">Permission type</span></span>      | <span data-ttu-id="86470-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="86470-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86470-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="86470-110">Delegated (work or school account)</span></span> | <span data-ttu-id="86470-111">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="86470-111">Tasks.Read</span></span>    |
|<span data-ttu-id="86470-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="86470-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86470-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="86470-113">Tasks.Read</span></span>    |
|<span data-ttu-id="86470-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="86470-114">Application</span></span> | <span data-ttu-id="86470-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86470-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="86470-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="86470-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="86470-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="86470-117">Optional query parameters</span></span>
<span data-ttu-id="86470-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="86470-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="86470-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="86470-119">Request headers</span></span>
| <span data-ttu-id="86470-120">名前</span><span class="sxs-lookup"><span data-stu-id="86470-120">Name</span></span>      |<span data-ttu-id="86470-121">説明</span><span class="sxs-lookup"><span data-stu-id="86470-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="86470-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="86470-122">Authorization</span></span>  | <span data-ttu-id="86470-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="86470-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="86470-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="86470-125">Request body</span></span>
<span data-ttu-id="86470-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="86470-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86470-127">応答</span><span class="sxs-lookup"><span data-stu-id="86470-127">Response</span></span>

<span data-ttu-id="86470-128">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[outlookTaskGroup](../resources/outlooktaskgroup.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="86470-128">If successful, this method returns a `200 OK` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="86470-129">例</span><span class="sxs-lookup"><span data-stu-id="86470-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="86470-130">要求</span><span class="sxs-lookup"><span data-stu-id="86470-130">Request</span></span>
<span data-ttu-id="86470-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="86470-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlooktaskgroup"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskGroups('AAMkADIyAAAhrbe-AAA=')
```
##### <a name="response"></a><span data-ttu-id="86470-132">応答</span><span class="sxs-lookup"><span data-stu-id="86470-132">Response</span></span>
<span data-ttu-id="86470-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="86470-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 138

{
    "id": "AAMkADIyAAAhrbe-AAA=",
    "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAInHxKw==",
    "isDefaultGroup": false,
    "name": "Leisure Tasks",
    "groupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get outlookTaskGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktaskgroup-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
