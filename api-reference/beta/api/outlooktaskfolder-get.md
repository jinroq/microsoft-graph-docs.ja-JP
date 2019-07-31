---
title: OutlookTaskFolder の取得
description: 指定された Outlook タスクフォルダーのプロパティとリレーションシップを取得します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c7288f3a5abc5dbc5327ed11cf5680906b45c98a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35992529"
---
# <a name="get-outlooktaskfolder"></a><span data-ttu-id="ce2b8-103">OutlookTaskFolder の取得</span><span class="sxs-lookup"><span data-stu-id="ce2b8-103">Get outlookTaskFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce2b8-104">指定された Outlook タスクフォルダーのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="ce2b8-104">Get the properties and relationships of the specified Outlook task folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="ce2b8-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ce2b8-105">Permissions</span></span>
<span data-ttu-id="ce2b8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ce2b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce2b8-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ce2b8-108">Permission type</span></span>      | <span data-ttu-id="ce2b8-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ce2b8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce2b8-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ce2b8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ce2b8-111">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="ce2b8-111">Tasks.Read</span></span>    |
|<span data-ttu-id="ce2b8-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ce2b8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce2b8-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="ce2b8-113">Tasks.Read</span></span>    |
|<span data-ttu-id="ce2b8-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ce2b8-114">Application</span></span> | <span data-ttu-id="ce2b8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce2b8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce2b8-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ce2b8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskFolders/{id}
GET /me/outlook/taskGroups/{id}/taskFolders/{id}
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ce2b8-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ce2b8-117">Optional query parameters</span></span>
<span data-ttu-id="ce2b8-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ce2b8-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ce2b8-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ce2b8-119">Request headers</span></span>
| <span data-ttu-id="ce2b8-120">名前</span><span class="sxs-lookup"><span data-stu-id="ce2b8-120">Name</span></span>      |<span data-ttu-id="ce2b8-121">説明</span><span class="sxs-lookup"><span data-stu-id="ce2b8-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ce2b8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce2b8-122">Authorization</span></span>  | <span data-ttu-id="ce2b8-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ce2b8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ce2b8-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="ce2b8-125">Request body</span></span>
<span data-ttu-id="ce2b8-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ce2b8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce2b8-127">応答</span><span class="sxs-lookup"><span data-stu-id="ce2b8-127">Response</span></span>

<span data-ttu-id="ce2b8-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[outlooktaskfolder](../resources/outlooktaskfolder.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ce2b8-128">If successful, this method returns a `200 OK` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ce2b8-129">例</span><span class="sxs-lookup"><span data-stu-id="ce2b8-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ce2b8-130">要求</span><span class="sxs-lookup"><span data-stu-id="ce2b8-130">Request</span></span>
<span data-ttu-id="ce2b8-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ce2b8-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ce2b8-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="ce2b8-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outlooktaskfolder"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskFolders/AAMkADIyAAAAABrJAAA=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ce2b8-133">C#</span><span class="sxs-lookup"><span data-stu-id="ce2b8-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outlooktaskfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ce2b8-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="ce2b8-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outlooktaskfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ce2b8-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="ce2b8-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outlooktaskfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ce2b8-136">Java</span><span class="sxs-lookup"><span data-stu-id="ce2b8-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-outlooktaskfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ce2b8-137">応答</span><span class="sxs-lookup"><span data-stu-id="ce2b8-137">Response</span></span>
<span data-ttu-id="ce2b8-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ce2b8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 151

{
  "id": "AAMkADIyAAAAABrJAAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAAAAeAA==",
  "isDefaultFolder": false,
  "name": "Monthly tasks",
  "parentGroupKey": "0006f0b7-0000-0000-c000-000000000046"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get outlookTaskFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
