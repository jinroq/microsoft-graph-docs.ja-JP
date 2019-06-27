---
title: デバイスを削除する
description: 登録されているデバイスを削除します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 51adc59b901a2a639360fe12c8a80e2fe6114808
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276385"
---
# <a name="delete-device"></a><span data-ttu-id="a3e0e-103">デバイスを削除する</span><span class="sxs-lookup"><span data-stu-id="a3e0e-103">Delete device</span></span>

<span data-ttu-id="a3e0e-104">登録されているデバイスを削除します。</span><span class="sxs-lookup"><span data-stu-id="a3e0e-104">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3e0e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a3e0e-105">Permissions</span></span>
<span data-ttu-id="a3e0e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a3e0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a3e0e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a3e0e-108">Permission type</span></span>      | <span data-ttu-id="a3e0e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a3e0e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3e0e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a3e0e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a3e0e-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a3e0e-111">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="a3e0e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a3e0e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3e0e-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3e0e-113">Not supported.</span></span>    |
|<span data-ttu-id="a3e0e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a3e0e-114">Application</span></span> | <span data-ttu-id="a3e0e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3e0e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3e0e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a3e0e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}
```
> <span data-ttu-id="a3e0e-117">注:要求内の"id"は、"deviceId"プロパティではなく、デバイスの id プロパティです。</span><span class="sxs-lookup"><span data-stu-id="a3e0e-117">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a3e0e-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a3e0e-118">Request headers</span></span>
| <span data-ttu-id="a3e0e-119">名前</span><span class="sxs-lookup"><span data-stu-id="a3e0e-119">Name</span></span>       | <span data-ttu-id="a3e0e-120">型</span><span class="sxs-lookup"><span data-stu-id="a3e0e-120">Type</span></span> | <span data-ttu-id="a3e0e-121">説明</span><span class="sxs-lookup"><span data-stu-id="a3e0e-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a3e0e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3e0e-122">Authorization</span></span>  | <span data-ttu-id="a3e0e-123">string</span><span class="sxs-lookup"><span data-stu-id="a3e0e-123">string</span></span>  | <span data-ttu-id="a3e0e-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a3e0e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a3e0e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a3e0e-126">Request body</span></span>
<span data-ttu-id="a3e0e-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a3e0e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3e0e-128">応答</span><span class="sxs-lookup"><span data-stu-id="a3e0e-128">Response</span></span>

<span data-ttu-id="a3e0e-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="a3e0e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3e0e-131">例</span><span class="sxs-lookup"><span data-stu-id="a3e0e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a3e0e-132">要求</span><span class="sxs-lookup"><span data-stu-id="a3e0e-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="a3e0e-133">応答</span><span class="sxs-lookup"><span data-stu-id="a3e0e-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a3e0e-134">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="a3e0e-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a3e0e-135">C#</span><span class="sxs-lookup"><span data-stu-id="a3e0e-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_device-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a3e0e-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="a3e0e-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_device-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a3e0e-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="a3e0e-137">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_device-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/device-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/device-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/device-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
