---
title: 契約書を一覧表示する
description: パートナー テナントに関連付けられている 契約オブジェクトの一覧を取得します。
ms.openlocfilehash: 41e30880bded985695581e7d1402a24d2353e07e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067915"
---
# <a name="list-contracts"></a><span data-ttu-id="a9ffe-103">契約書を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="a9ffe-103">List contracts</span></span>

> <span data-ttu-id="a9ffe-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a9ffe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a9ffe-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a9ffe-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a9ffe-106">パートナー テナントに関連付けられている [契約](../resources/contract.md)オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="a9ffe-106">Retrieve a list of [contract](../resources/contract.md) objects associated to a partner tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="a9ffe-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a9ffe-107">Permissions</span></span>

<span data-ttu-id="a9ffe-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a9ffe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a9ffe-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a9ffe-110">Permission type</span></span>      | <span data-ttu-id="a9ffe-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a9ffe-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9ffe-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a9ffe-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a9ffe-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a9ffe-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a9ffe-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a9ffe-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9ffe-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a9ffe-115">Not supported.</span></span>    |
|<span data-ttu-id="a9ffe-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a9ffe-116">Application</span></span> | <span data-ttu-id="a9ffe-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9ffe-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9ffe-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a9ffe-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /contracts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a9ffe-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a9ffe-119">Optional query parameters</span></span>

<span data-ttu-id="a9ffe-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a9ffe-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> 

> <span data-ttu-id="a9ffe-121">customerId、defaultDomainName、displayName によるフィルタリングがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="a9ffe-121">Filtering is supported for customerId, defaultDomainName, and displayName.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a9ffe-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a9ffe-122">Request headers</span></span>

| <span data-ttu-id="a9ffe-123">名前</span><span class="sxs-lookup"><span data-stu-id="a9ffe-123">Name</span></span>      |<span data-ttu-id="a9ffe-124">説明</span><span class="sxs-lookup"><span data-stu-id="a9ffe-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a9ffe-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9ffe-125">Authorization</span></span>  | <span data-ttu-id="a9ffe-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a9ffe-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a9ffe-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="a9ffe-128">Request body</span></span>

<span data-ttu-id="a9ffe-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a9ffe-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9ffe-130">応答</span><span class="sxs-lookup"><span data-stu-id="a9ffe-130">Response</span></span>

<span data-ttu-id="a9ffe-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Contract](../resources/contract.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="a9ffe-131">If successful, this method returns a `200 OK` response code and a collection of [Contract](../resources/contract.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9ffe-132">例</span><span class="sxs-lookup"><span data-stu-id="a9ffe-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a9ffe-133">要求</span><span class="sxs-lookup"><span data-stu-id="a9ffe-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/beta/contracts
```

##### <a name="response"></a><span data-ttu-id="a9ffe-134">応答</span><span class="sxs-lookup"><span data-stu-id="a9ffe-134">Response</span></span>

<span data-ttu-id="a9ffe-p104">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a9ffe-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Contract",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
    {
      "contractType": "contractType-value",
      "customerId": "customerId-value",
      "defaultDomainName": "defaultDomainName-value",
      "displayName": "displayName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Contract",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->