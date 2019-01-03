---
title: 上司を割り当てる
description: この API を使用して、ユーザーの上司を割り当てます。
ms.openlocfilehash: ab48d0546b533fcc137d31cdc889072abf48fcfe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022282"
---
# <a name="assign-a-manager"></a><span data-ttu-id="777bd-103">上司を割り当てる</span><span class="sxs-lookup"><span data-stu-id="777bd-103">Assign a manager</span></span>

<span data-ttu-id="777bd-104">この API を使用して、ユーザーの上司を割り当てます。</span><span class="sxs-lookup"><span data-stu-id="777bd-104">Use this API to assign a user's manager.</span></span>
> <span data-ttu-id="777bd-105">注:直属の部下を割り当てることはできません。代わりにこの API を使用します。</span><span class="sxs-lookup"><span data-stu-id="777bd-105">Note: You cannot assign direct reports - instead use this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="777bd-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="777bd-106">Permissions</span></span>
<span data-ttu-id="777bd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="777bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="777bd-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="777bd-109">Permission type</span></span>      | <span data-ttu-id="777bd-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="777bd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="777bd-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="777bd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="777bd-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="777bd-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="777bd-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="777bd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="777bd-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="777bd-114">Not supported.</span></span>    |
|<span data-ttu-id="777bd-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="777bd-115">Application</span></span> | <span data-ttu-id="777bd-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="777bd-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="777bd-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="777bd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /users/{id}/manager/$ref
```
## <a name="request-headers"></a><span data-ttu-id="777bd-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="777bd-118">Request headers</span></span>
| <span data-ttu-id="777bd-119">名前</span><span class="sxs-lookup"><span data-stu-id="777bd-119">Name</span></span>       | <span data-ttu-id="777bd-120">型</span><span class="sxs-lookup"><span data-stu-id="777bd-120">Type</span></span> | <span data-ttu-id="777bd-121">説明</span><span class="sxs-lookup"><span data-stu-id="777bd-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="777bd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="777bd-122">Authorization</span></span>  | <span data-ttu-id="777bd-123">string</span><span class="sxs-lookup"><span data-stu-id="777bd-123">string</span></span>  | <span data-ttu-id="777bd-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="777bd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="777bd-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="777bd-126">Request body</span></span>
<span data-ttu-id="777bd-127">要求本文で、追加する [directoryObject](../resources/directoryobject.md) または[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="777bd-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="777bd-128">応答</span><span class="sxs-lookup"><span data-stu-id="777bd-128">Response</span></span>

<span data-ttu-id="777bd-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="777bd-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="777bd-131">例</span><span class="sxs-lookup"><span data-stu-id="777bd-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="777bd-132">要求</span><span class="sxs-lookup"><span data-stu-id="777bd-132">Request</span></span>
<span data-ttu-id="777bd-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="777bd-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="777bd-134">要求本文で、追加する[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="777bd-134">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>
##### <a name="response"></a><span data-ttu-id="777bd-135">応答</span><span class="sxs-lookup"><span data-stu-id="777bd-135">Response</span></span>
<span data-ttu-id="777bd-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="777bd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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