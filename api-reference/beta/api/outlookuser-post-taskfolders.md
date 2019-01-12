---
title: OutlookTaskFolder を作成します。
description: 既定のタスク グループにタスク フォルダーを作成 (`My Tasks`) ユーザーのメールボックスの。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: ff3c4283bd331d2d778bdb2ef15c13b18e2624be
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925981"
---
# <a name="create-outlooktaskfolder"></a><span data-ttu-id="2183a-103">OutlookTaskFolder を作成します。</span><span class="sxs-lookup"><span data-stu-id="2183a-103">Create outlookTaskFolder</span></span>

> <span data-ttu-id="2183a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2183a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2183a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2183a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2183a-106">既定のタスク グループにタスク フォルダーを作成 (`My Tasks`) ユーザーのメールボックスの。</span><span class="sxs-lookup"><span data-stu-id="2183a-106">Create a task folder in the default task group (`My Tasks`) of the user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="2183a-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2183a-107">Permissions</span></span>
<span data-ttu-id="2183a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2183a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2183a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2183a-110">Permission type</span></span>      | <span data-ttu-id="2183a-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2183a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2183a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2183a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2183a-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2183a-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="2183a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2183a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2183a-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2183a-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="2183a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2183a-116">Application</span></span> | <span data-ttu-id="2183a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2183a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2183a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2183a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/taskFolders

```
## <a name="request-headers"></a><span data-ttu-id="2183a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2183a-119">Request headers</span></span>
| <span data-ttu-id="2183a-120">名前</span><span class="sxs-lookup"><span data-stu-id="2183a-120">Name</span></span>       | <span data-ttu-id="2183a-121">説明</span><span class="sxs-lookup"><span data-stu-id="2183a-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2183a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2183a-122">Authorization</span></span>  | <span data-ttu-id="2183a-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2183a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2183a-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="2183a-125">Request body</span></span>
<span data-ttu-id="2183a-126">要求の本文には、 [outlookTaskFolder](../resources/outlooktaskfolder.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="2183a-126">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2183a-127">応答</span><span class="sxs-lookup"><span data-stu-id="2183a-127">Response</span></span>

<span data-ttu-id="2183a-128">かどうかは成功すると、このメソッドを返します`201 Created`、応答の本体で応答コードと[outlookTaskFolder](../resources/outlooktaskfolder.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="2183a-128">If successful, this method returns `201 Created` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2183a-129">例</span><span class="sxs-lookup"><span data-stu-id="2183a-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2183a-130">要求</span><span class="sxs-lookup"><span data-stu-id="2183a-130">Request</span></span>
<span data-ttu-id="2183a-131">次の例は、既定のタスク グループでボランティアをという名前のタスク フォルダーを作成 (`My Tasks`) ユーザーのメールボックスの。</span><span class="sxs-lookup"><span data-stu-id="2183a-131">The following example creates a task folder called Volunteer in the default task group (`My Tasks`) of the user's mailbox.</span></span>
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
<span data-ttu-id="2183a-132">要求の本文には、 [outlookTaskFolder](../resources/outlooktaskfolder.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="2183a-132">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="2183a-133">応答</span><span class="sxs-lookup"><span data-stu-id="2183a-133">Response</span></span>
<span data-ttu-id="2183a-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2183a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create outlookTaskFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
