---
title: ページを更新する
description: OneNote ページの内容を更新します。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: ef51342aba7bab49fde6d69ea0c77c62dc841b7d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971712"
---
# <a name="update-page"></a><span data-ttu-id="aa884-103">ページを更新する</span><span class="sxs-lookup"><span data-stu-id="aa884-103">Update page</span></span>

<span data-ttu-id="aa884-104">OneNote ページの内容を更新します。</span><span class="sxs-lookup"><span data-stu-id="aa884-104">Update the content of a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="aa884-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="aa884-105">Permissions</span></span>
<span data-ttu-id="aa884-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aa884-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa884-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="aa884-108">Permission type</span></span>      | <span data-ttu-id="aa884-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="aa884-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa884-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="aa884-110">Delegated (work or school account)</span></span> | <span data-ttu-id="aa884-111">Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa884-111">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="aa884-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="aa884-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa884-113">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aa884-113">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="aa884-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="aa884-114">Application</span></span> | <span data-ttu-id="aa884-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa884-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa884-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="aa884-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onenote/pages/{id}/content
PATCH /users/{id | userPrincipalName}/onenote/pages/{id}/content
PATCH /groups/{id}/onenote/pages/{id}/content
PATCH /sites/{id}/onenote/pages/{id}/content
```
## <a name="request-headers"></a><span data-ttu-id="aa884-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aa884-117">Request headers</span></span>
| <span data-ttu-id="aa884-118">名前</span><span class="sxs-lookup"><span data-stu-id="aa884-118">Name</span></span>       | <span data-ttu-id="aa884-119">型</span><span class="sxs-lookup"><span data-stu-id="aa884-119">Type</span></span> | <span data-ttu-id="aa884-120">説明</span><span class="sxs-lookup"><span data-stu-id="aa884-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="aa884-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa884-121">Authorization</span></span>  | <span data-ttu-id="aa884-122">string</span><span class="sxs-lookup"><span data-stu-id="aa884-122">string</span></span>  | <span data-ttu-id="aa884-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="aa884-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="aa884-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="aa884-125">Content-Type</span></span> | <span data-ttu-id="aa884-126">string</span><span class="sxs-lookup"><span data-stu-id="aa884-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="aa884-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="aa884-127">Request body</span></span>
<span data-ttu-id="aa884-p103">要求本文で、ページの変更内容を表す [patchContentCommand](../resources/patchcontentcommand.md) オブジェクトの配列を指定します。詳細と例については、「<a href="https://msdn.microsoft.com/office/office365/howto/onenote-update-page">OneNote ページ コンテンツを更新する</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aa884-p103">In the request body, supply an array of [patchContentCommand](../resources/patchcontentcommand.md) objects that represent the changes to the page. For more information and examples, see <a href="https://msdn.microsoft.com/office/office365/howto/onenote-update-page">Update OneNote pages</a>.</span></span>

## <a name="response"></a><span data-ttu-id="aa884-130">応答</span><span class="sxs-lookup"><span data-stu-id="aa884-130">Response</span></span>

<span data-ttu-id="aa884-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。PATCH 要求に対して JSON データは返されません。</span><span class="sxs-lookup"><span data-stu-id="aa884-p104">If successful, this method returns a `204 No Content` response code.  No JSON data is returned for a PATCH request.</span></span>
## <a name="example"></a><span data-ttu-id="aa884-133">例</span><span class="sxs-lookup"><span data-stu-id="aa884-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aa884-134">要求</span><span class="sxs-lookup"><span data-stu-id="aa884-134">Request</span></span>
<span data-ttu-id="aa884-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="aa884-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_page"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/content
Content-type: application/json
Content-length: 312

[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-url-or-part-name" alt="image-alt-text" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>new-page-content</li>'
  }
]
```
##### <a name="response"></a><span data-ttu-id="aa884-136">応答</span><span class="sxs-lookup"><span data-stu-id="aa884-136">Response</span></span>
<span data-ttu-id="aa884-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="aa884-137">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenotePage"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
