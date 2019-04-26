---
title: デバイスを削除する
description: 登録されているデバイスを削除します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ee9bcfe46e0a931e47b4b4cbe0925fedf6bec7c3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33326110"
---
# <a name="delete-device"></a><span data-ttu-id="ba600-103">デバイスを削除する</span><span class="sxs-lookup"><span data-stu-id="ba600-103">Delete device</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba600-104">登録されているデバイスを削除します。</span><span class="sxs-lookup"><span data-stu-id="ba600-104">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba600-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ba600-105">Permissions</span></span>
<span data-ttu-id="ba600-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ba600-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ba600-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ba600-108">Permission type</span></span>      | <span data-ttu-id="ba600-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ba600-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba600-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ba600-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ba600-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ba600-111">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="ba600-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ba600-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba600-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ba600-113">Not supported.</span></span>    |
|<span data-ttu-id="ba600-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ba600-114">Application</span></span> | <span data-ttu-id="ba600-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ba600-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba600-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ba600-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}

```

> <span data-ttu-id="ba600-117">注:要求内の"id"は、"deviceId"プロパティではなく、デバイスの id プロパティです。</span><span class="sxs-lookup"><span data-stu-id="ba600-117">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ba600-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ba600-118">Request headers</span></span>
| <span data-ttu-id="ba600-119">名前</span><span class="sxs-lookup"><span data-stu-id="ba600-119">Name</span></span>       | <span data-ttu-id="ba600-120">型</span><span class="sxs-lookup"><span data-stu-id="ba600-120">Type</span></span> | <span data-ttu-id="ba600-121">説明</span><span class="sxs-lookup"><span data-stu-id="ba600-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ba600-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba600-122">Authorization</span></span>  | <span data-ttu-id="ba600-123">string</span><span class="sxs-lookup"><span data-stu-id="ba600-123">string</span></span>  | <span data-ttu-id="ba600-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ba600-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba600-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ba600-126">Request body</span></span>
<span data-ttu-id="ba600-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ba600-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba600-128">応答</span><span class="sxs-lookup"><span data-stu-id="ba600-128">Response</span></span>

<span data-ttu-id="ba600-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="ba600-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba600-131">例</span><span class="sxs-lookup"><span data-stu-id="ba600-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ba600-132">要求</span><span class="sxs-lookup"><span data-stu-id="ba600-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/beta/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="ba600-133">応答</span><span class="sxs-lookup"><span data-stu-id="ba600-133">Response</span></span>

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
  "suppressions": []
}
-->
