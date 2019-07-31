---
title: デバイスを削除する
description: 登録されているデバイスを削除します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f6e11c6332ed15b53221e957a72d4e1f2de743eb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35951464"
---
# <a name="delete-device"></a><span data-ttu-id="e5b77-103">デバイスを削除する</span><span class="sxs-lookup"><span data-stu-id="e5b77-103">Delete device</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5b77-104">登録されているデバイスを削除します。</span><span class="sxs-lookup"><span data-stu-id="e5b77-104">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5b77-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e5b77-105">Permissions</span></span>
<span data-ttu-id="e5b77-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e5b77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e5b77-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e5b77-108">Permission type</span></span>      | <span data-ttu-id="e5b77-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e5b77-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5b77-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e5b77-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e5b77-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e5b77-111">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="e5b77-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e5b77-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5b77-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e5b77-113">Not supported.</span></span>    |
|<span data-ttu-id="e5b77-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e5b77-114">Application</span></span> | <span data-ttu-id="e5b77-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e5b77-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5b77-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e5b77-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}

```

> <span data-ttu-id="e5b77-117">注:要求内の"id"は、"deviceId"プロパティではなく、デバイスの id プロパティです。</span><span class="sxs-lookup"><span data-stu-id="e5b77-117">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e5b77-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e5b77-118">Request headers</span></span>
| <span data-ttu-id="e5b77-119">名前</span><span class="sxs-lookup"><span data-stu-id="e5b77-119">Name</span></span>       | <span data-ttu-id="e5b77-120">型</span><span class="sxs-lookup"><span data-stu-id="e5b77-120">Type</span></span> | <span data-ttu-id="e5b77-121">説明</span><span class="sxs-lookup"><span data-stu-id="e5b77-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e5b77-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5b77-122">Authorization</span></span>  | <span data-ttu-id="e5b77-123">string</span><span class="sxs-lookup"><span data-stu-id="e5b77-123">string</span></span>  | <span data-ttu-id="e5b77-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e5b77-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5b77-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e5b77-126">Request body</span></span>
<span data-ttu-id="e5b77-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e5b77-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5b77-128">応答</span><span class="sxs-lookup"><span data-stu-id="e5b77-128">Response</span></span>

<span data-ttu-id="e5b77-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="e5b77-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5b77-131">例</span><span class="sxs-lookup"><span data-stu-id="e5b77-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e5b77-132">要求</span><span class="sxs-lookup"><span data-stu-id="e5b77-132">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e5b77-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e5b77-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/beta/devices/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e5b77-134">C#</span><span class="sxs-lookup"><span data-stu-id="e5b77-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e5b77-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="e5b77-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e5b77-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="e5b77-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e5b77-137">Java</span><span class="sxs-lookup"><span data-stu-id="e5b77-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-device-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e5b77-138">応答</span><span class="sxs-lookup"><span data-stu-id="e5b77-138">Response</span></span>

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
  "description": "Delete device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
