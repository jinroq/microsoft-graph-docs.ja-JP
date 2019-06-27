---
title: registeredUsers を一覧表示する
description: デバイスの登録ユーザーの一覧を取得します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 584226cd157658a8917c6059877d16b07d826f39
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276329"
---
# <a name="list-registeredusers"></a><span data-ttu-id="44d42-103">registeredUsers を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="44d42-103">List registeredUsers</span></span>

<span data-ttu-id="44d42-104">デバイスの登録ユーザーの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="44d42-104">Retrieve a list of users that are registered users of the device.</span></span>

<span data-ttu-id="44d42-105">クラウドに参加済みのデバイスと登録済みの個人用デバイスの場合、登録済みのユーザーは、登録時に登録済み所有者と同じ値に設定されます。</span><span class="sxs-lookup"><span data-stu-id="44d42-105">For cloud joined devices and registered personal devices, registered users are set to the same value as registered owners at the time of registration.</span></span>

## <a name="permissions"></a><span data-ttu-id="44d42-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="44d42-106">Permissions</span></span>
<span data-ttu-id="44d42-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="44d42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="44d42-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="44d42-109">Permission type</span></span>      | <span data-ttu-id="44d42-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="44d42-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44d42-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="44d42-111">Delegated (work or school account)</span></span> | <span data-ttu-id="44d42-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="44d42-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="44d42-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="44d42-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44d42-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="44d42-114">Not supported.</span></span>    |
|<span data-ttu-id="44d42-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="44d42-115">Application</span></span> | <span data-ttu-id="44d42-116">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44d42-116">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="44d42-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="44d42-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredUsers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="44d42-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="44d42-118">Optional query parameters</span></span>
<span data-ttu-id="44d42-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="44d42-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="44d42-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="44d42-120">Request headers</span></span>
| <span data-ttu-id="44d42-121">名前</span><span class="sxs-lookup"><span data-stu-id="44d42-121">Name</span></span>       | <span data-ttu-id="44d42-122">型</span><span class="sxs-lookup"><span data-stu-id="44d42-122">Type</span></span> | <span data-ttu-id="44d42-123">説明</span><span class="sxs-lookup"><span data-stu-id="44d42-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="44d42-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="44d42-124">Authorization</span></span>  | <span data-ttu-id="44d42-125">string</span><span class="sxs-lookup"><span data-stu-id="44d42-125">string</span></span>  | <span data-ttu-id="44d42-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="44d42-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="44d42-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="44d42-128">Request body</span></span>
<span data-ttu-id="44d42-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="44d42-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44d42-130">応答</span><span class="sxs-lookup"><span data-stu-id="44d42-130">Response</span></span>

<span data-ttu-id="44d42-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="44d42-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="44d42-132">例</span><span class="sxs-lookup"><span data-stu-id="44d42-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="44d42-133">要求</span><span class="sxs-lookup"><span data-stu-id="44d42-133">Request</span></span>
<span data-ttu-id="44d42-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="44d42-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredusers"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredUsers
```
##### <a name="response"></a><span data-ttu-id="44d42-135">応答</span><span class="sxs-lookup"><span data-stu-id="44d42-135">Response</span></span>
<span data-ttu-id="44d42-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="44d42-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="44d42-139">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="44d42-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="44d42-140">C#</span><span class="sxs-lookup"><span data-stu-id="44d42-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_registeredusers-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="44d42-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="44d42-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_registeredusers-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="44d42-142">目的-C</span><span class="sxs-lookup"><span data-stu-id="44d42-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_registeredusers-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List registeredUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/device-list-registeredusers.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/device-list-registeredusers.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/device-list-registeredusers.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
