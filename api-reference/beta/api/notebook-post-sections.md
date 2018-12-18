---
title: セクションを作成する
description: 指定されたノートブックに新しいセクションを作成します。
author: Jewan-microsoft
ms.openlocfilehash: 026473c7bed93fa127fd8fc4db8c27cfcb47acdc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325768"
---
# <a name="create-section"></a><span data-ttu-id="16f0e-103">セクションを作成する</span><span class="sxs-lookup"><span data-stu-id="16f0e-103">Create section</span></span>

> <span data-ttu-id="16f0e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="16f0e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16f0e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16f0e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="16f0e-106">指定されたノートブックに新しい[セクション](../resources/section.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="16f0e-106">Create a new [section](../resources/section.md) in the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="16f0e-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="16f0e-107">Permissions</span></span>
<span data-ttu-id="16f0e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="16f0e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16f0e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="16f0e-110">Permission type</span></span>      | <span data-ttu-id="16f0e-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="16f0e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16f0e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="16f0e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="16f0e-113">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16f0e-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="16f0e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="16f0e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16f0e-115">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16f0e-115">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="16f0e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="16f0e-116">Application</span></span> | <span data-ttu-id="16f0e-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16f0e-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="16f0e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="16f0e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/sections
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/sections
POST /groups/{id}/onenote/notebooks/{id}/sections
POST /sites/{id}/onenote/notebooks/{id}/sections
```
## <a name="request-headers"></a><span data-ttu-id="16f0e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="16f0e-119">Request headers</span></span>
| <span data-ttu-id="16f0e-120">名前</span><span class="sxs-lookup"><span data-stu-id="16f0e-120">Name</span></span>       | <span data-ttu-id="16f0e-121">種類</span><span class="sxs-lookup"><span data-stu-id="16f0e-121">Type</span></span> | <span data-ttu-id="16f0e-122">説明</span><span class="sxs-lookup"><span data-stu-id="16f0e-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="16f0e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="16f0e-123">Authorization</span></span>  | <span data-ttu-id="16f0e-124">string</span><span class="sxs-lookup"><span data-stu-id="16f0e-124">string</span></span>  | <span data-ttu-id="16f0e-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="16f0e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="16f0e-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="16f0e-127">Content-Type</span></span> | <span data-ttu-id="16f0e-128">string</span><span class="sxs-lookup"><span data-stu-id="16f0e-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="16f0e-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="16f0e-129">Request body</span></span>
<span data-ttu-id="16f0e-130">要求本文でセクション名を入力します。</span><span class="sxs-lookup"><span data-stu-id="16f0e-130">In the request body, supply a name for the section.</span></span>

<span data-ttu-id="16f0e-p104">同じ階層レベルでは、セクションの名前を一意にする必要があります。名前は 50 文字以内で、次の文字は使用できません: ?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="16f0e-p104">Within the same hierarchy level, section names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="16f0e-133">応答</span><span class="sxs-lookup"><span data-stu-id="16f0e-133">Response</span></span>

<span data-ttu-id="16f0e-134">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [section](../resources/section.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="16f0e-134">If successful, this method returns a `201 Created` response code and a [section](../resources/section.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16f0e-135">例</span><span class="sxs-lookup"><span data-stu-id="16f0e-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="16f0e-136">要求</span><span class="sxs-lookup"><span data-stu-id="16f0e-136">Request</span></span>
<span data-ttu-id="16f0e-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="16f0e-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_section_from_notebook"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks/{id}/sections
Content-type: application/json
Content-length: 27

{
  "displayName": "Section name"
}
```
##### <a name="response"></a><span data-ttu-id="16f0e-138">応答</span><span class="sxs-lookup"><span data-stu-id="16f0e-138">Response</span></span>
<span data-ttu-id="16f0e-p105">以下は、応答の例です。注:ここに示す応答オブジェクトは切り詰めて簡略化されています。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="16f0e-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 272

{
  "isDefault": true,
  "pagesUrl": "pagesUrl-value",
  "displayName": "name-value",
  "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
  "createdBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  },
  "lastModifiedBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Section",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
