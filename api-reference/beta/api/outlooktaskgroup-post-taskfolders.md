---
title: OutlookTaskFolder を作成します。
description: 指定された outlookTaskGroup の下の Outlook タスク フォルダーを作成します。
ms.openlocfilehash: 38fbc4766a520e5d671b37b98442096ceb481fd3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066266"
---
# <a name="create-outlooktaskfolder"></a><span data-ttu-id="be001-103">OutlookTaskFolder を作成します。</span><span class="sxs-lookup"><span data-stu-id="be001-103">Create outlookTaskFolder</span></span>

> <span data-ttu-id="be001-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="be001-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="be001-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="be001-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="be001-106">指定された[outlookTaskGroup](../resources/outlooktaskgroup.md)の下の Outlook タスク フォルダーを作成します。</span><span class="sxs-lookup"><span data-stu-id="be001-106">Create an Outlook task folder under a specified [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="be001-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="be001-107">Permissions</span></span>
<span data-ttu-id="be001-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="be001-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be001-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="be001-110">Permission type</span></span>      | <span data-ttu-id="be001-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="be001-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be001-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="be001-112">Delegated (work or school account)</span></span> | <span data-ttu-id="be001-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be001-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="be001-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="be001-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be001-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be001-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="be001-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="be001-116">Application</span></span> | <span data-ttu-id="be001-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="be001-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="be001-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="be001-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders

```
## <a name="request-headers"></a><span data-ttu-id="be001-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="be001-119">Request headers</span></span>
| <span data-ttu-id="be001-120">名前</span><span class="sxs-lookup"><span data-stu-id="be001-120">Name</span></span>       | <span data-ttu-id="be001-121">説明</span><span class="sxs-lookup"><span data-stu-id="be001-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="be001-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="be001-122">Authorization</span></span>  | <span data-ttu-id="be001-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="be001-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="be001-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="be001-125">Request body</span></span>
<span data-ttu-id="be001-126">要求の本文には、 [outlookTaskFolder](../resources/outlooktaskfolder.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="be001-126">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="be001-127">応答</span><span class="sxs-lookup"><span data-stu-id="be001-127">Response</span></span>

<span data-ttu-id="be001-128">かどうかは成功すると、このメソッドを返します`201 Created`、応答の本体で応答コードと[outlookTaskFolder](../resources/outlooktaskfolder.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="be001-128">If successful, this method returns `201 Created` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be001-129">例</span><span class="sxs-lookup"><span data-stu-id="be001-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="be001-130">要求</span><span class="sxs-lookup"><span data-stu-id="be001-130">Request</span></span>
<span data-ttu-id="be001-131">という名前のタスク フォルダーを作成する例を次`Cooking`で指定したタスク グループ。</span><span class="sxs-lookup"><span data-stu-id="be001-131">The following example creates a task folder called `Cooking` in the specified task group.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_outlooktaskfolder_from_outlooktaskgroup"
}-->
```http
POST https://graph.microsoft.com/beta/me/taskgroups('AAMkADIyAAAhrbe-AAA')/taskfolders 

Content-type: application/json
Content-length: 131

{
  "name": "Cooking"
}
```
<span data-ttu-id="be001-132">要求の本文には、 [outlookTaskFolder](../resources/outlooktaskfolder.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="be001-132">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="be001-133">応答</span><span class="sxs-lookup"><span data-stu-id="be001-133">Response</span></span>
<span data-ttu-id="be001-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="be001-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "id": "AAMkADIyAAAhrbPXAAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAOlA==",
  "isDefaultFolder": false,
  "name": "Cooking",
  "parentGroupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create outlookTaskFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->