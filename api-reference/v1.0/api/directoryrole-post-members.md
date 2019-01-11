---
title: ディレクトリ ロールのメンバーを追加する
description: この API を使用して、新しいディレクトリ ロールのメンバーを作成します。
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 11b06eac57d0850e8df5233bba47966f6b7932d8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886640"
---
# <a name="add-directory-role-member"></a><span data-ttu-id="7194a-103">ディレクトリ ロールのメンバーを追加する</span><span class="sxs-lookup"><span data-stu-id="7194a-103">Add directory role member</span></span>

<span data-ttu-id="7194a-104">この API を使用して、新しいディレクトリ ロールのメンバーを作成します。</span><span class="sxs-lookup"><span data-stu-id="7194a-104">Use this API to create a new directory role member.</span></span>

## <a name="permissions"></a><span data-ttu-id="7194a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7194a-105">Permissions</span></span>
<span data-ttu-id="7194a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7194a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7194a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7194a-108">Permission type</span></span>      | <span data-ttu-id="7194a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7194a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7194a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7194a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7194a-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7194a-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7194a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7194a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7194a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7194a-113">Not supported.</span></span>    |
|<span data-ttu-id="7194a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7194a-114">Application</span></span> | <span data-ttu-id="7194a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7194a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7194a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7194a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{id}/members/$ref

```
## <a name="request-headers"></a><span data-ttu-id="7194a-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7194a-117">Request headers</span></span>
| <span data-ttu-id="7194a-118">名前</span><span class="sxs-lookup"><span data-stu-id="7194a-118">Name</span></span>       | <span data-ttu-id="7194a-119">種類</span><span class="sxs-lookup"><span data-stu-id="7194a-119">Type</span></span> | <span data-ttu-id="7194a-120">説明</span><span class="sxs-lookup"><span data-stu-id="7194a-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7194a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7194a-121">Authorization</span></span>  | <span data-ttu-id="7194a-122">string</span><span class="sxs-lookup"><span data-stu-id="7194a-122">string</span></span>  | <span data-ttu-id="7194a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7194a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7194a-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7194a-125">Content-Type</span></span>  | <span data-ttu-id="7194a-126">string</span><span class="sxs-lookup"><span data-stu-id="7194a-126">string</span></span>  | <span data-ttu-id="7194a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7194a-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7194a-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="7194a-128">Request body</span></span>
<span data-ttu-id="7194a-129">要求本文で、追加する [directoryObject](../resources/directoryobject.md) または[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7194a-129">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="7194a-130">応答</span><span class="sxs-lookup"><span data-stu-id="7194a-130">Response</span></span>

<span data-ttu-id="7194a-131">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="7194a-131">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7194a-132">例</span><span class="sxs-lookup"><span data-stu-id="7194a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7194a-133">要求</span><span class="sxs-lookup"><span data-stu-id="7194a-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles/{id}/members/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```

##### <a name="response"></a><span data-ttu-id="7194a-134">応答</span><span class="sxs-lookup"><span data-stu-id="7194a-134">Response</span></span>
<span data-ttu-id="7194a-135">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="7194a-135">Note: The response object shown here may be truncated for brevity.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
Content-type: text/plain

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
