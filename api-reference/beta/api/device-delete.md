---
title: デバイスを削除する
description: 登録されているデバイスを削除します。
author: tfitzmac
ms.openlocfilehash: e171656e0d4ab32f140c1b53f5ea42e8424cb2e9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311523"
---
# <a name="delete-device"></a><span data-ttu-id="2f642-103">デバイスを削除する</span><span class="sxs-lookup"><span data-stu-id="2f642-103">Delete device</span></span>

> <span data-ttu-id="2f642-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2f642-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2f642-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2f642-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2f642-106">登録されているデバイスを削除します。</span><span class="sxs-lookup"><span data-stu-id="2f642-106">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f642-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2f642-107">Permissions</span></span>
<span data-ttu-id="2f642-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2f642-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2f642-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2f642-110">Permission type</span></span>      | <span data-ttu-id="2f642-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2f642-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f642-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2f642-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2f642-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2f642-113">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="2f642-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2f642-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f642-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2f642-115">Not supported.</span></span>    |
|<span data-ttu-id="2f642-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2f642-116">Application</span></span> | <span data-ttu-id="2f642-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2f642-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f642-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2f642-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}

```

> <span data-ttu-id="2f642-119">注:要求内の"id"は、"deviceId"プロパティではなく、デバイスの id プロパティです。</span><span class="sxs-lookup"><span data-stu-id="2f642-119">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2f642-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2f642-120">Request headers</span></span>
| <span data-ttu-id="2f642-121">名前</span><span class="sxs-lookup"><span data-stu-id="2f642-121">Name</span></span>       | <span data-ttu-id="2f642-122">種類</span><span class="sxs-lookup"><span data-stu-id="2f642-122">Type</span></span> | <span data-ttu-id="2f642-123">説明</span><span class="sxs-lookup"><span data-stu-id="2f642-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2f642-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f642-124">Authorization</span></span>  | <span data-ttu-id="2f642-125">string</span><span class="sxs-lookup"><span data-stu-id="2f642-125">string</span></span>  | <span data-ttu-id="2f642-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2f642-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2f642-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="2f642-128">Request body</span></span>
<span data-ttu-id="2f642-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2f642-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f642-130">応答</span><span class="sxs-lookup"><span data-stu-id="2f642-130">Response</span></span>

<span data-ttu-id="2f642-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="2f642-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f642-133">例</span><span class="sxs-lookup"><span data-stu-id="2f642-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2f642-134">要求</span><span class="sxs-lookup"><span data-stu-id="2f642-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/beta/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="2f642-135">応答</span><span class="sxs-lookup"><span data-stu-id="2f642-135">Response</span></span>

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
  "description": "Delete device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->