---
title: Delete calendarGroup
description: 既定の予定表グループ以外の予定表グループを削除します。
ms.openlocfilehash: 64fa9069ba54c7549392db4fc2d3d47b4e95ebdc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021955"
---
# <a name="delete-calendargroup"></a><span data-ttu-id="c4097-103">Delete calendarGroup</span><span class="sxs-lookup"><span data-stu-id="c4097-103">Delete calendarGroup</span></span>

<span data-ttu-id="c4097-104">既定の予定表グループ以外の予定表グループを削除します。</span><span class="sxs-lookup"><span data-stu-id="c4097-104">Delete a calendar group other than the default calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4097-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c4097-105">Permissions</span></span>

<span data-ttu-id="c4097-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c4097-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c4097-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c4097-108">Permission type</span></span>                        | <span data-ttu-id="c4097-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c4097-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="c4097-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c4097-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c4097-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4097-111">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="c4097-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c4097-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4097-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4097-113">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="c4097-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c4097-114">Application</span></span>                            | <span data-ttu-id="c4097-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4097-115">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c4097-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c4097-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/calendarGroups/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c4097-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c4097-117">Request headers</span></span>

| <span data-ttu-id="c4097-118">名前</span><span class="sxs-lookup"><span data-stu-id="c4097-118">Name</span></span>          | <span data-ttu-id="c4097-119">型</span><span class="sxs-lookup"><span data-stu-id="c4097-119">Type</span></span>   | <span data-ttu-id="c4097-120">説明</span><span class="sxs-lookup"><span data-stu-id="c4097-120">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="c4097-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4097-121">Authorization</span></span> | <span data-ttu-id="c4097-122">string</span><span class="sxs-lookup"><span data-stu-id="c4097-122">string</span></span> | <span data-ttu-id="c4097-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c4097-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c4097-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="c4097-125">Request body</span></span>

<span data-ttu-id="c4097-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c4097-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4097-127">応答</span><span class="sxs-lookup"><span data-stu-id="c4097-127">Response</span></span>

<span data-ttu-id="c4097-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="c4097-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4097-130">例</span><span class="sxs-lookup"><span data-stu-id="c4097-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c4097-131">要求</span><span class="sxs-lookup"><span data-stu-id="c4097-131">Request</span></span>

<span data-ttu-id="c4097-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c4097-132">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_calendargroup"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="c4097-133">応答</span><span class="sxs-lookup"><span data-stu-id="c4097-133">Response</span></span>

<span data-ttu-id="c4097-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c4097-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "Delete calendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
