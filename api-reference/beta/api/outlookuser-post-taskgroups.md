---
title: OutlookTaskGroup の作成
description: ユーザーのメールボックスに Outlook のタスクグループを作成します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9fbfcf6f9bbf14db0eb94b71de5ce6978a55a51f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349737"
---
# <a name="create-outlooktaskgroup"></a><span data-ttu-id="3bfec-103">OutlookTaskGroup の作成</span><span class="sxs-lookup"><span data-stu-id="3bfec-103">Create outlookTaskGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3bfec-104">ユーザーのメールボックスに Outlook のタスクグループを作成します。</span><span class="sxs-lookup"><span data-stu-id="3bfec-104">Create an Outlook task group in the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="3bfec-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3bfec-105">Permissions</span></span>
<span data-ttu-id="3bfec-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3bfec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3bfec-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3bfec-108">Permission type</span></span>      | <span data-ttu-id="3bfec-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3bfec-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3bfec-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3bfec-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3bfec-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3bfec-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="3bfec-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3bfec-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3bfec-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3bfec-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="3bfec-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3bfec-114">Application</span></span> | <span data-ttu-id="3bfec-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3bfec-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3bfec-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3bfec-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskGroups
POST /users/{id|userPrincipalName}/outlook/taskGroups
```
## <a name="request-headers"></a><span data-ttu-id="3bfec-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3bfec-117">Request headers</span></span>
| <span data-ttu-id="3bfec-118">名前</span><span class="sxs-lookup"><span data-stu-id="3bfec-118">Name</span></span>       | <span data-ttu-id="3bfec-119">説明</span><span class="sxs-lookup"><span data-stu-id="3bfec-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3bfec-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3bfec-120">Authorization</span></span>  | <span data-ttu-id="3bfec-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3bfec-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3bfec-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="3bfec-123">Request body</span></span>
<span data-ttu-id="3bfec-124">要求本文で、 [Outlooktaskgroup](../resources/outlooktaskgroup.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3bfec-124">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3bfec-125">応答</span><span class="sxs-lookup"><span data-stu-id="3bfec-125">Response</span></span>

<span data-ttu-id="3bfec-126">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[outlooktaskgroup](../resources/outlooktaskgroup.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3bfec-126">If successful, this method returns `201 Created` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3bfec-127">例</span><span class="sxs-lookup"><span data-stu-id="3bfec-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3bfec-128">要求</span><span class="sxs-lookup"><span data-stu-id="3bfec-128">Request</span></span>
<span data-ttu-id="3bfec-129">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3bfec-129">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3bfec-130">プロトコル</span><span class="sxs-lookup"><span data-stu-id="3bfec-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_outlooktaskgroup_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/taskGroups
Content-type: application/json
Content-length: 40

{
  "name": "Leisure tasks"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3bfec-131">C#</span><span class="sxs-lookup"><span data-stu-id="3bfec-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlooktaskgroup-from-outlookuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3bfec-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3bfec-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlooktaskgroup-from-outlookuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3bfec-133">目的-C</span><span class="sxs-lookup"><span data-stu-id="3bfec-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlooktaskgroup-from-outlookuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3bfec-134">Java</span><span class="sxs-lookup"><span data-stu-id="3bfec-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-outlooktaskgroup-from-outlookuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="3bfec-135">要求本文で、 [Outlooktaskgroup](../resources/outlooktaskgroup.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3bfec-135">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="3bfec-136">応答</span><span class="sxs-lookup"><span data-stu-id="3bfec-136">Response</span></span>
<span data-ttu-id="3bfec-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3bfec-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 138

{
  "id": "AAMkADIyAAAhrbe-AAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAGjg==",
  "isDefaultGroup": false,
  "name": "Leisure tasks",
  "groupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create outlookTaskGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
