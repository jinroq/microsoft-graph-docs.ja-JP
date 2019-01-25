---
title: 契約書を取得する
description: 契約オブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6fa54d813a456cc5a29aadc84ec29f99dc475f9f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513264"
---
# <a name="get-contract"></a><span data-ttu-id="47629-103">契約書を取得する</span><span class="sxs-lookup"><span data-stu-id="47629-103">Get Contract</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47629-104">[契約](../resources/contract.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="47629-104">Retrieve the properties and relationships of [contract](../resources/contract.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="47629-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="47629-105">Permissions</span></span>

<span data-ttu-id="47629-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="47629-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="47629-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="47629-108">Permission type</span></span>      | <span data-ttu-id="47629-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="47629-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47629-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="47629-110">Delegated (work or school account)</span></span> | <span data-ttu-id="47629-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="47629-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="47629-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="47629-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47629-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="47629-113">Not supported.</span></span>    |
|<span data-ttu-id="47629-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="47629-114">Application</span></span> | <span data-ttu-id="47629-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47629-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="47629-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="47629-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contracts/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="47629-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="47629-117">Optional query parameters</span></span>

<span data-ttu-id="47629-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="47629-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="47629-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="47629-119">Request headers</span></span>

| <span data-ttu-id="47629-120">名前</span><span class="sxs-lookup"><span data-stu-id="47629-120">Name</span></span>      |<span data-ttu-id="47629-121">説明</span><span class="sxs-lookup"><span data-stu-id="47629-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="47629-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="47629-122">Authorization</span></span>  | <span data-ttu-id="47629-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="47629-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="47629-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="47629-125">Request body</span></span>

<span data-ttu-id="47629-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="47629-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47629-127">応答</span><span class="sxs-lookup"><span data-stu-id="47629-127">Response</span></span>

<span data-ttu-id="47629-128">成功した場合、このメソッドは応答本文で `200 OK` 応答コードと [Contract](../resources/contract.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="47629-128">If successful, this method returns a `200 OK` response code and [Contract](../resources/contract.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47629-129">例</span><span class="sxs-lookup"><span data-stu-id="47629-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="47629-130">要求</span><span class="sxs-lookup"><span data-stu-id="47629-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/beta/contracts/{id}
```

##### <a name="response"></a><span data-ttu-id="47629-131">応答</span><span class="sxs-lookup"><span data-stu-id="47629-131">Response</span></span>
<span data-ttu-id="47629-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="47629-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Contract"
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
<!--
{
  "type": "#page.annotation",
  "description": "Get Contract",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/contract-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
