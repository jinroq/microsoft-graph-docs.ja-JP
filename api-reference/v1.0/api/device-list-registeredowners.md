---
title: registeredOwners を一覧表示する
description: デバイスの登録済み所有者の一覧を取得します。 登録済み所有者は、デバイスがクラウドに参加済みか、または個人用デバイスが登録済みのユーザーです。 登録済み所有者は、登録時に設定されます。 現在、所有者は 1 人しかいることができません。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 023ce6a0d4d00384e4311f0454c59ca33ed368ab
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276406"
---
# <a name="list-registeredowners"></a><span data-ttu-id="1a156-106">registeredOwners を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="1a156-106">List registeredOwners</span></span>

<span data-ttu-id="1a156-107">デバイスの登録済み所有者の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="1a156-107">Retrieve a list of users that are registered owners of the device.</span></span> <span data-ttu-id="1a156-108">登録済み所有者は、デバイスがクラウドに参加済みか、または個人用デバイスが登録済みのユーザーです。</span><span class="sxs-lookup"><span data-stu-id="1a156-108">A registered owner is the user that cloud joined the device or registered their personal device.</span></span> <span data-ttu-id="1a156-109">登録済み所有者は、登録時に設定されます。</span><span class="sxs-lookup"><span data-stu-id="1a156-109">The registered owner is set at the time of registration.</span></span> <span data-ttu-id="1a156-110">現在、所有者は 1 人しかいることができません。</span><span class="sxs-lookup"><span data-stu-id="1a156-110">Currently, there can be only one owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a156-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1a156-111">Permissions</span></span>
<span data-ttu-id="1a156-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1a156-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1a156-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1a156-114">Permission type</span></span>      | <span data-ttu-id="1a156-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1a156-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a156-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1a156-116">Delegated (work or school account)</span></span> | <span data-ttu-id="1a156-117">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1a156-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1a156-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1a156-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a156-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a156-119">Not supported.</span></span>    |
|<span data-ttu-id="1a156-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1a156-120">Application</span></span> | <span data-ttu-id="1a156-121">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a156-121">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a156-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1a156-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredOwners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1a156-123">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="1a156-123">Optional query parameters</span></span>
<span data-ttu-id="1a156-124">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="1a156-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1a156-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1a156-125">Request headers</span></span>
| <span data-ttu-id="1a156-126">名前</span><span class="sxs-lookup"><span data-stu-id="1a156-126">Name</span></span>       | <span data-ttu-id="1a156-127">型</span><span class="sxs-lookup"><span data-stu-id="1a156-127">Type</span></span> | <span data-ttu-id="1a156-128">説明</span><span class="sxs-lookup"><span data-stu-id="1a156-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1a156-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a156-129">Authorization</span></span>  | <span data-ttu-id="1a156-130">string</span><span class="sxs-lookup"><span data-stu-id="1a156-130">string</span></span>  | <span data-ttu-id="1a156-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1a156-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a156-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="1a156-133">Request body</span></span>
<span data-ttu-id="1a156-134">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1a156-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a156-135">応答</span><span class="sxs-lookup"><span data-stu-id="1a156-135">Response</span></span>

<span data-ttu-id="1a156-136">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="1a156-136">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1a156-137">例</span><span class="sxs-lookup"><span data-stu-id="1a156-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1a156-138">要求</span><span class="sxs-lookup"><span data-stu-id="1a156-138">Request</span></span>
<span data-ttu-id="1a156-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1a156-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredowners"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredOwners
```
##### <a name="response"></a><span data-ttu-id="1a156-140">応答</span><span class="sxs-lookup"><span data-stu-id="1a156-140">Response</span></span>
<span data-ttu-id="1a156-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1a156-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1a156-144">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="1a156-144">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1a156-145">C#</span><span class="sxs-lookup"><span data-stu-id="1a156-145">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_registeredowners-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1a156-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="1a156-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_registeredowners-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="1a156-147">目的-C</span><span class="sxs-lookup"><span data-stu-id="1a156-147">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_registeredowners-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List registeredOwners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/device-list-registeredowners.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/device-list-registeredowners.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/device-list-registeredowners.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
