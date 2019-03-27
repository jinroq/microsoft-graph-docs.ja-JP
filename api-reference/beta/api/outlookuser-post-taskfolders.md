---
title: outlooktaskfolder の作成
description: ユーザーのメールボックスの既定のタスクグループ (`My Tasks`) にタスクフォルダーを作成します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 16f54dffc1ff2fff71a22658a2418be99fde7353
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/27/2019
ms.locfileid: "30869373"
---
# <a name="create-outlooktaskfolder"></a><span data-ttu-id="dc7fb-103">outlooktaskfolder の作成</span><span class="sxs-lookup"><span data-stu-id="dc7fb-103">Create outlookTaskFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc7fb-104">ユーザーのメールボックスの既定のタスクグループ (`My Tasks`) にタスクフォルダーを作成します。</span><span class="sxs-lookup"><span data-stu-id="dc7fb-104">Create a task folder in the default task group (`My Tasks`) of the user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc7fb-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="dc7fb-105">Permissions</span></span>
<span data-ttu-id="dc7fb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dc7fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc7fb-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dc7fb-108">Permission type</span></span>      | <span data-ttu-id="dc7fb-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="dc7fb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc7fb-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dc7fb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dc7fb-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dc7fb-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="dc7fb-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dc7fb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc7fb-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dc7fb-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="dc7fb-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dc7fb-114">Application</span></span> | <span data-ttu-id="dc7fb-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dc7fb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dc7fb-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dc7fb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskFolders
```
## <a name="request-headers"></a><span data-ttu-id="dc7fb-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dc7fb-117">Request headers</span></span>
| <span data-ttu-id="dc7fb-118">名前</span><span class="sxs-lookup"><span data-stu-id="dc7fb-118">Name</span></span>       | <span data-ttu-id="dc7fb-119">説明</span><span class="sxs-lookup"><span data-stu-id="dc7fb-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dc7fb-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc7fb-120">Authorization</span></span>  | <span data-ttu-id="dc7fb-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="dc7fb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dc7fb-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="dc7fb-123">Request body</span></span>
<span data-ttu-id="dc7fb-124">要求本文で、 [outlooktaskfolder](../resources/outlooktaskfolder.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="dc7fb-124">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="dc7fb-125">応答</span><span class="sxs-lookup"><span data-stu-id="dc7fb-125">Response</span></span>

<span data-ttu-id="dc7fb-126">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[outlooktaskfolder](../resources/outlooktaskfolder.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="dc7fb-126">If successful, this method returns `201 Created` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc7fb-127">例</span><span class="sxs-lookup"><span data-stu-id="dc7fb-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dc7fb-128">要求</span><span class="sxs-lookup"><span data-stu-id="dc7fb-128">Request</span></span>
<span data-ttu-id="dc7fb-129">次の例では、ユーザーのメールボックスの既定のタスクグループ`My Tasks`() に、「ボランティア」というタスクフォルダーを作成します。</span><span class="sxs-lookup"><span data-stu-id="dc7fb-129">The following example creates a task folder called Volunteer in the default task group (`My Tasks`) of the user's mailbox.</span></span>
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
<span data-ttu-id="dc7fb-130">要求本文で、 [outlooktaskfolder](../resources/outlooktaskfolder.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="dc7fb-130">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="dc7fb-131">応答</span><span class="sxs-lookup"><span data-stu-id="dc7fb-131">Response</span></span>
<span data-ttu-id="dc7fb-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="dc7fb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/outlookuser-post-taskfolders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
