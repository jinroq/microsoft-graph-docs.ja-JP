---
title: ポリシーを取得する
description: ポリシーのプロパティを取得します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 435e711c711675b94b089d818b7451b551f8b5ac
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35978883"
---
# <a name="get-policy"></a><span data-ttu-id="f6ce0-103">ポリシーを取得する</span><span class="sxs-lookup"><span data-stu-id="f6ce0-103">Get Policy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6ce0-104">[ポリシー](../resources/policy.md)のプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="f6ce0-104">Retrieve the properties of a [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f6ce0-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f6ce0-105">Permissions</span></span>
<span data-ttu-id="f6ce0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f6ce0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6ce0-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f6ce0-108">Permission type</span></span>      | <span data-ttu-id="f6ce0-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f6ce0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6ce0-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f6ce0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f6ce0-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f6ce0-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f6ce0-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f6ce0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6ce0-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f6ce0-113">Not supported.</span></span>    |
|<span data-ttu-id="f6ce0-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f6ce0-114">Application</span></span> | <span data-ttu-id="f6ce0-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f6ce0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6ce0-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f6ce0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f6ce0-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f6ce0-117">Request headers</span></span>
| <span data-ttu-id="f6ce0-118">名前</span><span class="sxs-lookup"><span data-stu-id="f6ce0-118">Name</span></span>       | <span data-ttu-id="f6ce0-119">型</span><span class="sxs-lookup"><span data-stu-id="f6ce0-119">Type</span></span> | <span data-ttu-id="f6ce0-120">説明</span><span class="sxs-lookup"><span data-stu-id="f6ce0-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f6ce0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6ce0-121">Authorization</span></span>  | <span data-ttu-id="f6ce0-122">string</span><span class="sxs-lookup"><span data-stu-id="f6ce0-122">string</span></span>  | <span data-ttu-id="f6ce0-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f6ce0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f6ce0-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="f6ce0-125">Request body</span></span>
<span data-ttu-id="f6ce0-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f6ce0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6ce0-127">応答</span><span class="sxs-lookup"><span data-stu-id="f6ce0-127">Response</span></span>

<span data-ttu-id="f6ce0-128">成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[ポリシー](../resources/policy.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f6ce0-128">If successful, this method returns `200 OK` response code and a [policy](../resources/policy.md) object in the response body.</span></span> <span data-ttu-id="f6ce0-129">Unsucccessful</span><span class="sxs-lookup"><span data-stu-id="f6ce0-129">If unsucccessful...</span></span>

## <a name="example"></a><span data-ttu-id="f6ce0-130">例</span><span class="sxs-lookup"><span data-stu-id="f6ce0-130">Example</span></span>
<span data-ttu-id="f6ce0-131">次の例では、特定のポリシーを取得します。</span><span class="sxs-lookup"><span data-stu-id="f6ce0-131">The following example retrieves a specific policy.</span></span>

##### <a name="request"></a><span data-ttu-id="f6ce0-132">要求</span><span class="sxs-lookup"><span data-stu-id="f6ce0-132">Request</span></span>
<span data-ttu-id="f6ce0-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f6ce0-133">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies/{id}
```

##### <a name="response"></a><span data-ttu-id="f6ce0-134">応答</span><span class="sxs-lookup"><span data-stu-id="f6ce0-134">Response</span></span>
<span data-ttu-id="f6ce0-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f6ce0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#policies/$entity",
    "id":"id-value",
    "alternativeIdentifier":null,
    "definition":["policy-definition"],
    "displayName":"name-value",
    "isOrganizationDefault":boolean-value,
    "keyCredentials":[key-credentials],
    "type":"type-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
