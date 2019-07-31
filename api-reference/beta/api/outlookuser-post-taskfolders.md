---
title: OutlookTaskFolder の作成
description: ユーザーのメールボックスの既定のタスクグループ (`My Tasks`) にタスクフォルダーを作成します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: d7552e310e4d1e9fff1e559d1d92c71b2107a3d4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35983636"
---
# <a name="create-outlooktaskfolder"></a><span data-ttu-id="572f9-103">OutlookTaskFolder の作成</span><span class="sxs-lookup"><span data-stu-id="572f9-103">Create outlookTaskFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="572f9-104">ユーザーのメールボックスの既定のタスクグループ (`My Tasks`) にタスクフォルダーを作成します。</span><span class="sxs-lookup"><span data-stu-id="572f9-104">Create a task folder in the default task group (`My Tasks`) of the user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="572f9-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="572f9-105">Permissions</span></span>
<span data-ttu-id="572f9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="572f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="572f9-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="572f9-108">Permission type</span></span>      | <span data-ttu-id="572f9-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="572f9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="572f9-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="572f9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="572f9-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="572f9-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="572f9-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="572f9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="572f9-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="572f9-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="572f9-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="572f9-114">Application</span></span> | <span data-ttu-id="572f9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="572f9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="572f9-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="572f9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskFolders
```
## <a name="request-headers"></a><span data-ttu-id="572f9-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="572f9-117">Request headers</span></span>
| <span data-ttu-id="572f9-118">名前</span><span class="sxs-lookup"><span data-stu-id="572f9-118">Name</span></span>       | <span data-ttu-id="572f9-119">説明</span><span class="sxs-lookup"><span data-stu-id="572f9-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="572f9-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="572f9-120">Authorization</span></span>  | <span data-ttu-id="572f9-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="572f9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="572f9-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="572f9-123">Request body</span></span>
<span data-ttu-id="572f9-124">要求本文で、 [Outlooktaskfolder](../resources/outlooktaskfolder.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="572f9-124">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="572f9-125">応答</span><span class="sxs-lookup"><span data-stu-id="572f9-125">Response</span></span>

<span data-ttu-id="572f9-126">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[outlooktaskfolder](../resources/outlooktaskfolder.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="572f9-126">If successful, this method returns `201 Created` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="572f9-127">例</span><span class="sxs-lookup"><span data-stu-id="572f9-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="572f9-128">要求</span><span class="sxs-lookup"><span data-stu-id="572f9-128">Request</span></span>
<span data-ttu-id="572f9-129">次の例では、ユーザーのメールボックスの既定のタスクグループ`My Tasks`() に、「ボランティア」というタスクフォルダーを作成します。</span><span class="sxs-lookup"><span data-stu-id="572f9-129">The following example creates a task folder called Volunteer in the default task group (`My Tasks`) of the user's mailbox.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="572f9-130">プロトコル</span><span class="sxs-lookup"><span data-stu-id="572f9-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_outlooktaskfolder_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/taskfolders 
Content-type: application/json
Content-length: 60

{
  "name": "Volunteer"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="572f9-131">C#</span><span class="sxs-lookup"><span data-stu-id="572f9-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlooktaskfolder-from-outlookuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="572f9-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="572f9-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlooktaskfolder-from-outlookuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="572f9-133">目的-C</span><span class="sxs-lookup"><span data-stu-id="572f9-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlooktaskfolder-from-outlookuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="572f9-134">Java</span><span class="sxs-lookup"><span data-stu-id="572f9-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-outlooktaskfolder-from-outlookuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="572f9-135">要求本文で、 [Outlooktaskfolder](../resources/outlooktaskfolder.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="572f9-135">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="572f9-136">応答</span><span class="sxs-lookup"><span data-stu-id="572f9-136">Response</span></span>
<span data-ttu-id="572f9-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="572f9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskFolder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 151

{
  "id": "AAMkADIyAAAhrbPWAAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAGig==",
  "isDefaultFolder": false,
  "name": "Volunteer",
  "parentGroupKey": "0006f0b7-0000-0000-c000-000000000046"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create outlookTaskFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
