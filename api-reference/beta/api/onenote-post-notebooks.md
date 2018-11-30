---
title: ノートブックを作成する
description: 新しい OneNote ノートブックを作成します。
ms.openlocfilehash: b1f32bc8aadb5e5ec42e751453535b3ef116e907
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074505"
---
# <a name="create-notebook"></a><span data-ttu-id="82d42-103">ノートブックを作成する</span><span class="sxs-lookup"><span data-stu-id="82d42-103">Create notebook</span></span>

> <span data-ttu-id="82d42-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="82d42-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="82d42-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="82d42-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="82d42-106">新しい OneNote [ノートブック](../resources/notebook.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="82d42-106">Create a new OneNote [notebook](../resources/notebook.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="82d42-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="82d42-107">Permissions</span></span>
<span data-ttu-id="82d42-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="82d42-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82d42-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="82d42-110">Permission type</span></span>      | <span data-ttu-id="82d42-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="82d42-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82d42-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="82d42-112">Delegated (work or school account)</span></span> | <span data-ttu-id="82d42-113">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82d42-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="82d42-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="82d42-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82d42-115">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="82d42-115">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="82d42-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="82d42-116">Application</span></span> | <span data-ttu-id="82d42-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82d42-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="82d42-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="82d42-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks
POST /users/{id | userPrincipalName}/onenote/notebooks
POST /groups/{id}/onenote/notebooks
POST /sites/{id}/onenote/notebooks
```
## <a name="request-headers"></a><span data-ttu-id="82d42-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="82d42-119">Request headers</span></span>
| <span data-ttu-id="82d42-120">名前</span><span class="sxs-lookup"><span data-stu-id="82d42-120">Name</span></span>       | <span data-ttu-id="82d42-121">型</span><span class="sxs-lookup"><span data-stu-id="82d42-121">Type</span></span> | <span data-ttu-id="82d42-122">説明</span><span class="sxs-lookup"><span data-stu-id="82d42-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="82d42-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="82d42-123">Authorization</span></span>  | <span data-ttu-id="82d42-124">string</span><span class="sxs-lookup"><span data-stu-id="82d42-124">string</span></span>  | <span data-ttu-id="82d42-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="82d42-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="82d42-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="82d42-127">Content-Type</span></span> | <span data-ttu-id="82d42-128">string</span><span class="sxs-lookup"><span data-stu-id="82d42-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="82d42-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="82d42-129">Request body</span></span>
<span data-ttu-id="82d42-130">要求本文で、ノートブックの名前を入力します。</span><span class="sxs-lookup"><span data-stu-id="82d42-130">In the request body, supply a name for the notebook.</span></span> 

<span data-ttu-id="82d42-p104">ノートブック名は一意にする必要があります。名前は 128 文字以内で、次の文字は使用できません:  ?\*\/:<>|'"</span><span class="sxs-lookup"><span data-stu-id="82d42-p104">Notebook names must be unique. The name cannot contain more than 128 characters or contain the following characters:  ?\*\/:<>|'"</span></span>

## <a name="response"></a><span data-ttu-id="82d42-133">応答</span><span class="sxs-lookup"><span data-stu-id="82d42-133">Response</span></span>

<span data-ttu-id="82d42-134">成功した場合、このメソッドは応答本文で `201 Created` 応答コードと新しい [notebook](../resources/notebook.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="82d42-134">If successful, this method returns a `201 Created` response code and the new [notebook](../resources/notebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82d42-135">例</span><span class="sxs-lookup"><span data-stu-id="82d42-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="82d42-136">要求</span><span class="sxs-lookup"><span data-stu-id="82d42-136">Request</span></span>
<span data-ttu-id="82d42-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="82d42-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_notebook_from_onenote"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks
Content-type: application/json
Content-length: 30

{
  "displayName": "Notebook name"
}
```

##### <a name="response"></a><span data-ttu-id="82d42-138">応答</span><span class="sxs-lookup"><span data-stu-id="82d42-138">Response</span></span>
<span data-ttu-id="82d42-p105">以下は、応答の例です。注:ここに示す応答オブジェクトは切り詰めて簡略化されています。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="82d42-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 284

{
  "isDefault": true,
  "userRole": {
  },
  "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
  "isShared": true,
  "sectionsUrl": "sectionsUrl-value",
  "sectionGroupsUrl": "sectionGroupsUrl-value",
  "links": {
    "oneNoteClientUrl": {
      "href": "href-value"
    },
    "oneNoteWebUrl": {
      "href": "href-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Notebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->