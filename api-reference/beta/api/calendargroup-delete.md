---
title: Delete calendarGroup
description: 既定の予定表グループ以外の予定表グループを削除します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e1e6b1d82778cba84dde0006772b3e9bf7ad1269
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36317838"
---
# <a name="delete-calendargroup"></a><span data-ttu-id="790d7-103">Delete calendarGroup</span><span class="sxs-lookup"><span data-stu-id="790d7-103">Delete calendarGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="790d7-104">既定の予定表グループ以外の予定表グループを削除します。</span><span class="sxs-lookup"><span data-stu-id="790d7-104">Delete a calendar group other than the default calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="790d7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="790d7-105">Permissions</span></span>

<span data-ttu-id="790d7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="790d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="790d7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="790d7-108">Permission type</span></span>                        | <span data-ttu-id="790d7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="790d7-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="790d7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="790d7-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="790d7-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="790d7-111">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="790d7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="790d7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="790d7-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="790d7-113">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="790d7-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="790d7-114">Application</span></span>                            | <span data-ttu-id="790d7-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="790d7-115">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="790d7-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="790d7-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/calendarGroups/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="790d7-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="790d7-117">Request headers</span></span>

| <span data-ttu-id="790d7-118">名前</span><span class="sxs-lookup"><span data-stu-id="790d7-118">Name</span></span>          | <span data-ttu-id="790d7-119">型</span><span class="sxs-lookup"><span data-stu-id="790d7-119">Type</span></span>   | <span data-ttu-id="790d7-120">説明</span><span class="sxs-lookup"><span data-stu-id="790d7-120">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="790d7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="790d7-121">Authorization</span></span> | <span data-ttu-id="790d7-122">string</span><span class="sxs-lookup"><span data-stu-id="790d7-122">string</span></span> | <span data-ttu-id="790d7-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="790d7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="790d7-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="790d7-125">Request body</span></span>

<span data-ttu-id="790d7-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="790d7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="790d7-127">応答</span><span class="sxs-lookup"><span data-stu-id="790d7-127">Response</span></span>

<span data-ttu-id="790d7-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="790d7-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="790d7-130">例</span><span class="sxs-lookup"><span data-stu-id="790d7-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="790d7-131">要求</span><span class="sxs-lookup"><span data-stu-id="790d7-131">Request</span></span>

<span data-ttu-id="790d7-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="790d7-132">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="790d7-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="790d7-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_calendargroup"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/calendarGroups/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="790d7-134">C#</span><span class="sxs-lookup"><span data-stu-id="790d7-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-calendargroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="790d7-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="790d7-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-calendargroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="790d7-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="790d7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-calendargroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="790d7-137">Java</span><span class="sxs-lookup"><span data-stu-id="790d7-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-calendargroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="790d7-138">応答</span><span class="sxs-lookup"><span data-stu-id="790d7-138">Response</span></span>

<span data-ttu-id="790d7-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="790d7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "Delete calendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
