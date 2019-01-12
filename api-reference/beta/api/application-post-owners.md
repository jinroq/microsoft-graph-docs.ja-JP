---
title: 所有者を作成します。
description: この API を使用すると、新しい所有者を作成します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d3bb4ae2e944ae9a292545bba462381fd7212130
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922312"
---
# <a name="create-owner"></a><span data-ttu-id="a6f3e-103">所有者を作成します。</span><span class="sxs-lookup"><span data-stu-id="a6f3e-103">Create owner</span></span>

> <span data-ttu-id="a6f3e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a6f3e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a6f3e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6f3e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a6f3e-106">この API を使用すると、新しい所有者を作成します。</span><span class="sxs-lookup"><span data-stu-id="a6f3e-106">Use this API to create a new owner.</span></span>
## <a name="permissions"></a><span data-ttu-id="a6f3e-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a6f3e-107">Permissions</span></span>
<span data-ttu-id="a6f3e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a6f3e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6f3e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a6f3e-110">Permission type</span></span>      | <span data-ttu-id="a6f3e-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a6f3e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6f3e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a6f3e-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="a6f3e-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a6f3e-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a6f3e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a6f3e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6f3e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6f3e-115">Not supported.</span></span>    |
|<span data-ttu-id="a6f3e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a6f3e-116">Application</span></span> | <span data-ttu-id="a6f3e-117">Application.ReadWrite.OwnedBy と Directory.Read.All、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a6f3e-117">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6f3e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a6f3e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/owners

```
## <a name="request-headers"></a><span data-ttu-id="a6f3e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a6f3e-119">Request headers</span></span>
| <span data-ttu-id="a6f3e-120">名前</span><span class="sxs-lookup"><span data-stu-id="a6f3e-120">Name</span></span>       | <span data-ttu-id="a6f3e-121">型</span><span class="sxs-lookup"><span data-stu-id="a6f3e-121">Type</span></span> | <span data-ttu-id="a6f3e-122">説明</span><span class="sxs-lookup"><span data-stu-id="a6f3e-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a6f3e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6f3e-123">Authorization</span></span>  | <span data-ttu-id="a6f3e-124">string</span><span class="sxs-lookup"><span data-stu-id="a6f3e-124">string</span></span>  | <span data-ttu-id="a6f3e-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a6f3e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a6f3e-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a6f3e-127">Request body</span></span>
<span data-ttu-id="a6f3e-128">要求本文で、[directoryObject](../resources/directoryobject.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a6f3e-128">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a6f3e-129">応答</span><span class="sxs-lookup"><span data-stu-id="a6f3e-129">Response</span></span>

<span data-ttu-id="a6f3e-130">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a6f3e-130">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6f3e-131">例</span><span class="sxs-lookup"><span data-stu-id="a6f3e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a6f3e-132">要求</span><span class="sxs-lookup"><span data-stu-id="a6f3e-132">Request</span></span>
<span data-ttu-id="a6f3e-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a6f3e-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_application"
}-->
```http
POST https://graph.microsoft.com/beta/applications/{id}/owners
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
<span data-ttu-id="a6f3e-134">要求本文で、[directoryObject](../resources/directoryobject.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a6f3e-134">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a6f3e-135">応答</span><span class="sxs-lookup"><span data-stu-id="a6f3e-135">Response</span></span>
<span data-ttu-id="a6f3e-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a6f3e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
