---
title: 契約書を一覧表示する
description: パートナーテナントに関連付けられている契約オブジェクトの一覧を取得します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b4003bf2aaa910d3ad33e299a9fdb01f47229d1a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566186"
---
# <a name="list-contracts"></a><span data-ttu-id="e011b-103">契約書を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e011b-103">List contracts</span></span>

<span data-ttu-id="e011b-104">パートナーテナントに関連付けられている[契約](../resources/contract.md)オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="e011b-104">Retrieve a list of [contract](../resources/contract.md) objects associated to a partner tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="e011b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e011b-105">Permissions</span></span>

<span data-ttu-id="e011b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e011b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e011b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e011b-108">Permission type</span></span>      | <span data-ttu-id="e011b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e011b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e011b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e011b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e011b-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e011b-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e011b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e011b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e011b-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e011b-113">Not supported.</span></span>    |
|<span data-ttu-id="e011b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e011b-114">Application</span></span> | <span data-ttu-id="e011b-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e011b-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e011b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e011b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /contracts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e011b-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e011b-117">Optional query parameters</span></span>

<span data-ttu-id="e011b-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e011b-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> 

> <span data-ttu-id="e011b-119">フィルター処理は、customerId、defaultdomainname、および displayName でサポートされています。</span><span class="sxs-lookup"><span data-stu-id="e011b-119">Filtering is supported for customerId, defaultDomainName, and displayName.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e011b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e011b-120">Request headers</span></span>

| <span data-ttu-id="e011b-121">名前</span><span class="sxs-lookup"><span data-stu-id="e011b-121">Name</span></span>      |<span data-ttu-id="e011b-122">説明</span><span class="sxs-lookup"><span data-stu-id="e011b-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e011b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e011b-123">Authorization</span></span>  | <span data-ttu-id="e011b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e011b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e011b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e011b-126">Request body</span></span>

<span data-ttu-id="e011b-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e011b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e011b-128">応答</span><span class="sxs-lookup"><span data-stu-id="e011b-128">Response</span></span>

<span data-ttu-id="e011b-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[Contract](../resources/contract.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="e011b-129">If successful, this method returns a `200 OK` response code and a collection of [Contract](../resources/contract.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e011b-130">例</span><span class="sxs-lookup"><span data-stu-id="e011b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e011b-131">要求</span><span class="sxs-lookup"><span data-stu-id="e011b-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/v1.0/contracts
```

##### <a name="response"></a><span data-ttu-id="e011b-132">応答</span><span class="sxs-lookup"><span data-stu-id="e011b-132">Response</span></span>

<span data-ttu-id="e011b-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e011b-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contract",
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
