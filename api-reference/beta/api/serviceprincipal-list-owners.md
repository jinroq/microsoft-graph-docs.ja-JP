---
title: 'serviceprincipals: リストの所有者'
description: serviceprincipal の所有者の一覧を取得します。
localization_priority: Normal
ms.openlocfilehash: 162df83524d5c26d6e95112d30f91c7d0bc27596
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331364"
---
# <a name="serviceprincipals-list-owners"></a><span data-ttu-id="68e72-103">serviceprincipals: リストの所有者</span><span class="sxs-lookup"><span data-stu-id="68e72-103">servicePrincipals: List owners</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68e72-104">serviceprincipal の所有者の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="68e72-104">Retrieve a list of owners of the servicePrincipal.</span></span>

## <a name="permissions"></a><span data-ttu-id="68e72-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="68e72-105">Permissions</span></span>
<span data-ttu-id="68e72-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="68e72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68e72-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="68e72-108">Permission type</span></span>      | <span data-ttu-id="68e72-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="68e72-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68e72-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="68e72-110">Delegated (work or school account)</span></span> | <span data-ttu-id="68e72-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="68e72-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="68e72-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="68e72-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68e72-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="68e72-113">Not supported.</span></span>    |
|<span data-ttu-id="68e72-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="68e72-114">Application</span></span> | <span data-ttu-id="68e72-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68e72-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="68e72-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="68e72-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/owners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="68e72-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="68e72-117">Optional query parameters</span></span>
<span data-ttu-id="68e72-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="68e72-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="68e72-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="68e72-119">Request headers</span></span>
| <span data-ttu-id="68e72-120">名前</span><span class="sxs-lookup"><span data-stu-id="68e72-120">Name</span></span>       | <span data-ttu-id="68e72-121">型</span><span class="sxs-lookup"><span data-stu-id="68e72-121">Type</span></span> | <span data-ttu-id="68e72-122">説明</span><span class="sxs-lookup"><span data-stu-id="68e72-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="68e72-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="68e72-123">Authorization</span></span>  | <span data-ttu-id="68e72-124">string</span><span class="sxs-lookup"><span data-stu-id="68e72-124">string</span></span>  | <span data-ttu-id="68e72-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="68e72-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="68e72-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="68e72-127">Request body</span></span>
<span data-ttu-id="68e72-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="68e72-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68e72-129">応答</span><span class="sxs-lookup"><span data-stu-id="68e72-129">Response</span></span>

<span data-ttu-id="68e72-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="68e72-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="68e72-131">例</span><span class="sxs-lookup"><span data-stu-id="68e72-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="68e72-132">要求</span><span class="sxs-lookup"><span data-stu-id="68e72-132">Request</span></span>
<span data-ttu-id="68e72-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="68e72-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/owners
```
##### <a name="response"></a><span data-ttu-id="68e72-134">応答</span><span class="sxs-lookup"><span data-stu-id="68e72-134">Response</span></span>
<span data-ttu-id="68e72-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="68e72-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
