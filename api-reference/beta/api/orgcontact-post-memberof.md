---
title: 所属するグループを作成します。
description: 新しいへの後方リンクを作成するのにには、この API を使用します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ca5aa856f1f2e64f3a3b73ccff15f686c048cfda
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970004"
---
# <a name="create-memberof"></a><span data-ttu-id="3f001-103">所属するグループを作成します。</span><span class="sxs-lookup"><span data-stu-id="3f001-103">Create memberOf</span></span>

> <span data-ttu-id="3f001-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3f001-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3f001-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3f001-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3f001-106">新しいへの後方リンクを作成するのにには、この API を使用します。</span><span class="sxs-lookup"><span data-stu-id="3f001-106">Use this API to create a new memberOf.</span></span>
## <a name="permissions"></a><span data-ttu-id="3f001-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3f001-107">Permissions</span></span>
<span data-ttu-id="3f001-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3f001-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f001-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3f001-110">Permission type</span></span>      | <span data-ttu-id="3f001-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3f001-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3f001-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3f001-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3f001-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3f001-113">Not supported.</span></span>    |
|<span data-ttu-id="3f001-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3f001-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f001-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3f001-115">Not supported.</span></span>    |
|<span data-ttu-id="3f001-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3f001-116">Application</span></span> | <span data-ttu-id="3f001-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3f001-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3f001-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3f001-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/memberOf

```
## <a name="request-headers"></a><span data-ttu-id="3f001-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3f001-119">Request headers</span></span>
| <span data-ttu-id="3f001-120">名前</span><span class="sxs-lookup"><span data-stu-id="3f001-120">Name</span></span>       | <span data-ttu-id="3f001-121">種類</span><span class="sxs-lookup"><span data-stu-id="3f001-121">Type</span></span> | <span data-ttu-id="3f001-122">説明</span><span class="sxs-lookup"><span data-stu-id="3f001-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3f001-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f001-123">Authorization</span></span>  | <span data-ttu-id="3f001-124">string</span><span class="sxs-lookup"><span data-stu-id="3f001-124">string</span></span>  | <span data-ttu-id="3f001-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3f001-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3f001-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="3f001-127">Request body</span></span>
<span data-ttu-id="3f001-128">要求本文で、[directoryObject](../resources/directoryobject.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3f001-128">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3f001-129">応答</span><span class="sxs-lookup"><span data-stu-id="3f001-129">Response</span></span>

<span data-ttu-id="3f001-130">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3f001-130">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f001-131">例</span><span class="sxs-lookup"><span data-stu-id="3f001-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3f001-132">要求</span><span class="sxs-lookup"><span data-stu-id="3f001-132">Request</span></span>
<span data-ttu-id="3f001-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3f001-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_orgcontact"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/memberOf
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
<span data-ttu-id="3f001-134">要求本文で、[directoryObject](../resources/directoryobject.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3f001-134">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="3f001-135">応答</span><span class="sxs-lookup"><span data-stu-id="3f001-135">Response</span></span>
<span data-ttu-id="3f001-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3f001-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 51

{
  "directoryObject": {
    "id": "id-value"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
