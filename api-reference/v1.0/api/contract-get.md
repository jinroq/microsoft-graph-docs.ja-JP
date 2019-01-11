---
title: 契約書を取得する
description: 契約オブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
ms.openlocfilehash: dd379286e161cc68e33af49bec20bb580512ef0b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805776"
---
# <a name="get-contract"></a><span data-ttu-id="b345c-103">契約書を取得する</span><span class="sxs-lookup"><span data-stu-id="b345c-103">Get Contract</span></span>

<span data-ttu-id="b345c-104">[契約](../resources/contract.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="b345c-104">Retrieve the properties and relationships of [contract](../resources/contract.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b345c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b345c-105">Permissions</span></span>

<span data-ttu-id="b345c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b345c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b345c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b345c-108">Permission type</span></span>      | <span data-ttu-id="b345c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b345c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b345c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b345c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b345c-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b345c-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b345c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b345c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b345c-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b345c-113">Not supported.</span></span>    |
|<span data-ttu-id="b345c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b345c-114">Application</span></span> | <span data-ttu-id="b345c-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b345c-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b345c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b345c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contracts/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b345c-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b345c-117">Optional query parameters</span></span>

<span data-ttu-id="b345c-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b345c-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b345c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b345c-119">Request headers</span></span>

| <span data-ttu-id="b345c-120">名前</span><span class="sxs-lookup"><span data-stu-id="b345c-120">Name</span></span>      |<span data-ttu-id="b345c-121">説明</span><span class="sxs-lookup"><span data-stu-id="b345c-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b345c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b345c-122">Authorization</span></span>  | <span data-ttu-id="b345c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b345c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b345c-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="b345c-125">Request body</span></span>

<span data-ttu-id="b345c-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b345c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b345c-127">応答</span><span class="sxs-lookup"><span data-stu-id="b345c-127">Response</span></span>

<span data-ttu-id="b345c-128">成功した場合、このメソッドは応答本文で `200 OK` 応答コードと [Contract](../resources/contract.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b345c-128">If successful, this method returns a `200 OK` response code and [Contract](../resources/contract.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b345c-129">例</span><span class="sxs-lookup"><span data-stu-id="b345c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b345c-130">要求</span><span class="sxs-lookup"><span data-stu-id="b345c-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/v1.0/contracts/{id}
```

##### <a name="response"></a><span data-ttu-id="b345c-131">応答</span><span class="sxs-lookup"><span data-stu-id="b345c-131">Response</span></span>
<span data-ttu-id="b345c-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b345c-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contract"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 186

{
  "contractType": "contractType-value",
  "customerId": "customerId-value",
  "defaultDomainName": "defaultDomainName-value",
  "displayName": "displayName-value",
  "id": "id-value"
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
