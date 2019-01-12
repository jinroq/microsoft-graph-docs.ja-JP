---
title: 上司を割り当てる
description: この API を使用して、ユーザーの上司を割り当てます。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 770fad522e505abbd9f689540e6a28e875ba063d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912072"
---
# <a name="assign-a-manager"></a><span data-ttu-id="246d9-103">上司を割り当てる</span><span class="sxs-lookup"><span data-stu-id="246d9-103">Assign a manager</span></span>

> <span data-ttu-id="246d9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="246d9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="246d9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="246d9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="246d9-106">この API を使用して、ユーザーの上司を割り当てます。</span><span class="sxs-lookup"><span data-stu-id="246d9-106">Use this API to assign a user's manager.</span></span>
> <span data-ttu-id="246d9-107">注:直属の部下を割り当てることはできません。代わりにこの API を使用します。</span><span class="sxs-lookup"><span data-stu-id="246d9-107">Note: You cannot assign direct reports - instead use this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="246d9-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="246d9-108">Permissions</span></span>
<span data-ttu-id="246d9-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="246d9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="246d9-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="246d9-111">Permission type</span></span>      | <span data-ttu-id="246d9-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="246d9-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="246d9-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="246d9-113">Delegated (work or school account)</span></span> | <span data-ttu-id="246d9-114">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="246d9-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="246d9-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="246d9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="246d9-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="246d9-116">Not supported.</span></span>    |
|<span data-ttu-id="246d9-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="246d9-117">Application</span></span> | <span data-ttu-id="246d9-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="246d9-118">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="246d9-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="246d9-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /users/{id}/manager/$ref
```
## <a name="request-headers"></a><span data-ttu-id="246d9-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="246d9-120">Request headers</span></span>
| <span data-ttu-id="246d9-121">名前</span><span class="sxs-lookup"><span data-stu-id="246d9-121">Name</span></span>       | <span data-ttu-id="246d9-122">型</span><span class="sxs-lookup"><span data-stu-id="246d9-122">Type</span></span> | <span data-ttu-id="246d9-123">説明</span><span class="sxs-lookup"><span data-stu-id="246d9-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="246d9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="246d9-124">Authorization</span></span>  | <span data-ttu-id="246d9-125">string</span><span class="sxs-lookup"><span data-stu-id="246d9-125">string</span></span>  | <span data-ttu-id="246d9-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="246d9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="246d9-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="246d9-128">Request body</span></span>
<span data-ttu-id="246d9-129">要求本文で、追加する [directoryObject](../resources/directoryobject.md) または[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="246d9-129">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="246d9-130">応答</span><span class="sxs-lookup"><span data-stu-id="246d9-130">Response</span></span>

<span data-ttu-id="246d9-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="246d9-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="246d9-133">例</span><span class="sxs-lookup"><span data-stu-id="246d9-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="246d9-134">要求</span><span class="sxs-lookup"><span data-stu-id="246d9-134">Request</span></span>
<span data-ttu-id="246d9-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="246d9-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
PUT https://graph.microsoft.com/v1.0/users/{id}/manager/$ref
Content-type: application/json
Content-length: xxx

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
<span data-ttu-id="246d9-136">要求本文で、追加する[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="246d9-136">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>
##### <a name="response"></a><span data-ttu-id="246d9-137">応答</span><span class="sxs-lookup"><span data-stu-id="246d9-137">Response</span></span>
<span data-ttu-id="246d9-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="246d9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
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
