---
title: デバイスの推移性のグループを一覧表示する
description: デバイスがメンバーであるグループを取得します。 この API 要求は推移的なので、デバイスがのネストされたメンバーであるすべてのグループも返します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 93d27fcfc4163afbe5b833a2f510365d8093fbc3
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34656315"
---
# <a name="list-device-transitive-groups"></a><span data-ttu-id="ac923-104">デバイスの推移性のグループを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ac923-104">List device transitive groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac923-105">デバイスがメンバーであるグループを取得します。</span><span class="sxs-lookup"><span data-stu-id="ac923-105">Get groups that the device is a member of.</span></span> <span data-ttu-id="ac923-106">この API 要求は推移的なので、デバイスがのネストされたメンバーであるすべてのグループも返します。</span><span class="sxs-lookup"><span data-stu-id="ac923-106">This API request is transitive, and will also return all groups the device is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac923-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ac923-107">Permissions</span></span>

<span data-ttu-id="ac923-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ac923-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac923-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ac923-110">Permission type</span></span>      | <span data-ttu-id="ac923-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ac923-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac923-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ac923-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ac923-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ac923-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ac923-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ac923-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac923-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ac923-115">Not supported.</span></span>    |
|<span data-ttu-id="ac923-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ac923-116">Application</span></span> | <span data-ttu-id="ac923-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac923-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac923-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ac923-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /devices/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ac923-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ac923-119">Optional query parameters</span></span>

<span data-ttu-id="ac923-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ac923-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ac923-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ac923-121">Request headers</span></span>

| <span data-ttu-id="ac923-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ac923-122">Header</span></span>       | <span data-ttu-id="ac923-123">値</span><span class="sxs-lookup"><span data-stu-id="ac923-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ac923-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac923-124">Authorization</span></span>  | <span data-ttu-id="ac923-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ac923-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ac923-127">承諾</span><span class="sxs-lookup"><span data-stu-id="ac923-127">Accept</span></span>  | <span data-ttu-id="ac923-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ac923-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac923-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="ac923-129">Request body</span></span>

<span data-ttu-id="ac923-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ac923-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac923-131">応答</span><span class="sxs-lookup"><span data-stu-id="ac923-131">Response</span></span>

<span data-ttu-id="ac923-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="ac923-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac923-133">例</span><span class="sxs-lookup"><span data-stu-id="ac923-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="ac923-134">要求</span><span class="sxs-lookup"><span data-stu-id="ac923-134">Request</span></span>

<span data-ttu-id="ac923-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ac923-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_devices_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/beta/devices/{id}/transitiveMemberOf
```

### <a name="response"></a><span data-ttu-id="ac923-136">応答</span><span class="sxs-lookup"><span data-stu-id="ac923-136">Response</span></span>

<span data-ttu-id="ac923-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ac923-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ac923-140">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="ac923-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ac923-141">C#</span><span class="sxs-lookup"><span data-stu-id="ac923-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_devices_transitivememberof-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ac923-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="ac923-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_devices_transitivememberof-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List devices transitiveMsemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/device-list-transitivememberof.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/device-list-transitivememberof.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
