---
title: 契約書を一覧表示する
description: パートナー テナントに関連付けられている 契約オブジェクトの一覧を取得します。
ms.openlocfilehash: ed2e7ea7c422372adc8377863713982cc3c688aa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022718"
---
# <a name="list-contracts"></a><span data-ttu-id="9d045-103">契約書を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="9d045-103">List contracts</span></span>

<span data-ttu-id="9d045-104">パートナー テナントに関連付けられている [契約](../resources/contract.md)オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="9d045-104">Retrieve a list of [contract](../resources/contract.md) objects associated to a partner tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d045-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9d045-105">Permissions</span></span>

<span data-ttu-id="9d045-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9d045-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9d045-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9d045-108">Permission type</span></span>      | <span data-ttu-id="9d045-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9d045-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d045-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9d045-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9d045-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9d045-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9d045-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9d045-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d045-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9d045-113">Not supported.</span></span>    |
|<span data-ttu-id="9d045-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9d045-114">Application</span></span> | <span data-ttu-id="9d045-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d045-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d045-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9d045-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /contracts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9d045-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="9d045-117">Optional query parameters</span></span>

<span data-ttu-id="9d045-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="9d045-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> 

> <span data-ttu-id="9d045-119">customerId、defaultDomainName、displayName によるフィルタリングがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="9d045-119">Filtering is supported for customerId, defaultDomainName, and displayName.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9d045-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9d045-120">Request headers</span></span>

| <span data-ttu-id="9d045-121">名前</span><span class="sxs-lookup"><span data-stu-id="9d045-121">Name</span></span>      |<span data-ttu-id="9d045-122">説明</span><span class="sxs-lookup"><span data-stu-id="9d045-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9d045-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d045-123">Authorization</span></span>  | <span data-ttu-id="9d045-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9d045-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9d045-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="9d045-126">Request body</span></span>

<span data-ttu-id="9d045-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9d045-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d045-128">応答</span><span class="sxs-lookup"><span data-stu-id="9d045-128">Response</span></span>

<span data-ttu-id="9d045-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Contract](../resources/contract.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="9d045-129">If successful, this method returns a `200 OK` response code and a collection of [Contract](../resources/contract.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d045-130">例</span><span class="sxs-lookup"><span data-stu-id="9d045-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9d045-131">要求</span><span class="sxs-lookup"><span data-stu-id="9d045-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/v1.0/contracts
```

##### <a name="response"></a><span data-ttu-id="9d045-132">応答</span><span class="sxs-lookup"><span data-stu-id="9d045-132">Response</span></span>

<span data-ttu-id="9d045-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9d045-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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