---
title: Delete calendarGroup
description: 既定の予定表グループ以外の予定表グループを削除します。
ms.openlocfilehash: e71d05a8a0205b10d8735ea0e7baf32f201c7e15
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069604"
---
# <a name="delete-calendargroup"></a><span data-ttu-id="83333-103">Delete calendarGroup</span><span class="sxs-lookup"><span data-stu-id="83333-103">Delete calendarGroup</span></span>

> <span data-ttu-id="83333-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="83333-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="83333-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83333-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="83333-106">既定の予定表グループ以外の予定表グループを削除します。</span><span class="sxs-lookup"><span data-stu-id="83333-106">Delete a calendar group other than the default calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="83333-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="83333-107">Permissions</span></span>

<span data-ttu-id="83333-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="83333-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="83333-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="83333-110">Permission type</span></span>                        | <span data-ttu-id="83333-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="83333-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="83333-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="83333-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="83333-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="83333-113">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="83333-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="83333-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83333-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="83333-115">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="83333-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="83333-116">Application</span></span>                            | <span data-ttu-id="83333-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="83333-117">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="83333-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="83333-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/calendarGroups/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="83333-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="83333-119">Request headers</span></span>

| <span data-ttu-id="83333-120">名前</span><span class="sxs-lookup"><span data-stu-id="83333-120">Name</span></span>          | <span data-ttu-id="83333-121">型</span><span class="sxs-lookup"><span data-stu-id="83333-121">Type</span></span>   | <span data-ttu-id="83333-122">説明</span><span class="sxs-lookup"><span data-stu-id="83333-122">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="83333-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="83333-123">Authorization</span></span> | <span data-ttu-id="83333-124">string</span><span class="sxs-lookup"><span data-stu-id="83333-124">string</span></span> | <span data-ttu-id="83333-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="83333-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="83333-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="83333-127">Request body</span></span>

<span data-ttu-id="83333-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="83333-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83333-129">応答</span><span class="sxs-lookup"><span data-stu-id="83333-129">Response</span></span>

<span data-ttu-id="83333-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="83333-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83333-132">例</span><span class="sxs-lookup"><span data-stu-id="83333-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="83333-133">要求</span><span class="sxs-lookup"><span data-stu-id="83333-133">Request</span></span>

<span data-ttu-id="83333-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="83333-134">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_calendargroup"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/calendarGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="83333-135">応答</span><span class="sxs-lookup"><span data-stu-id="83333-135">Response</span></span>

<span data-ttu-id="83333-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="83333-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
