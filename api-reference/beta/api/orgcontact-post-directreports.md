---
title: DirectReport の作成
description: この API を使用して、新しい directReport を作成します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5f3b37931e62aa9add5ac408fe574909e67b5155
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36346507"
---
# <a name="create-directreport"></a><span data-ttu-id="a6efb-103">DirectReport の作成</span><span class="sxs-lookup"><span data-stu-id="a6efb-103">Create directReport</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6efb-104">この API を使用して、新しい directReport を作成します。</span><span class="sxs-lookup"><span data-stu-id="a6efb-104">Use this API to create a new directReport.</span></span>
## <a name="permissions"></a><span data-ttu-id="a6efb-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a6efb-105">Permissions</span></span>
<span data-ttu-id="a6efb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a6efb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6efb-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a6efb-108">Permission type</span></span>      | <span data-ttu-id="a6efb-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a6efb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6efb-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a6efb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a6efb-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6efb-111">Not supported.</span></span>    |
|<span data-ttu-id="a6efb-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a6efb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6efb-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6efb-113">Not supported.</span></span>    |
|<span data-ttu-id="a6efb-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a6efb-114">Application</span></span> | <span data-ttu-id="a6efb-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6efb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6efb-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a6efb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/directReports

```
## <a name="request-headers"></a><span data-ttu-id="a6efb-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a6efb-117">Request headers</span></span>
| <span data-ttu-id="a6efb-118">名前</span><span class="sxs-lookup"><span data-stu-id="a6efb-118">Name</span></span>       | <span data-ttu-id="a6efb-119">型</span><span class="sxs-lookup"><span data-stu-id="a6efb-119">Type</span></span> | <span data-ttu-id="a6efb-120">説明</span><span class="sxs-lookup"><span data-stu-id="a6efb-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a6efb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6efb-121">Authorization</span></span>  | <span data-ttu-id="a6efb-122">string</span><span class="sxs-lookup"><span data-stu-id="a6efb-122">string</span></span>  | <span data-ttu-id="a6efb-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a6efb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6efb-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a6efb-125">Request body</span></span>
<span data-ttu-id="a6efb-126">要求本文で、[directoryObject](../resources/directoryobject.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a6efb-126">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a6efb-127">応答</span><span class="sxs-lookup"><span data-stu-id="a6efb-127">Response</span></span>

<span data-ttu-id="a6efb-128">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a6efb-128">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6efb-129">例</span><span class="sxs-lookup"><span data-stu-id="a6efb-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a6efb-130">要求</span><span class="sxs-lookup"><span data-stu-id="a6efb-130">Request</span></span>
<span data-ttu-id="a6efb-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a6efb-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a6efb-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="a6efb-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_orgcontact"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/directReports
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a6efb-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a6efb-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="a6efb-134">要求本文に、[directoryObject](../resources/directoryobject.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a6efb-134">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a6efb-135">応答</span><span class="sxs-lookup"><span data-stu-id="a6efb-135">Response</span></span>
<span data-ttu-id="a6efb-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a6efb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create directReport",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
