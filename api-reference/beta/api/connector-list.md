---
title: コネクタの一覧表示
description: コネクタオブジェクトの一覧を取得します。
localization_priority: Normal
ms.openlocfilehash: 69e70bbf0f247b4d702f9cea2e69e2cddcce6272
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33327675"
---
# <a name="list-connectors"></a><span data-ttu-id="d5b24-103">コネクタの一覧表示</span><span class="sxs-lookup"><span data-stu-id="d5b24-103">List connectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5b24-104">コネクタオブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="d5b24-104">Retrieve a list of connector objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="d5b24-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d5b24-105">Permissions</span></span>
<span data-ttu-id="d5b24-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d5b24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5b24-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d5b24-108">Permission type</span></span>      | <span data-ttu-id="d5b24-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d5b24-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5b24-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d5b24-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d5b24-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d5b24-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d5b24-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d5b24-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5b24-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5b24-113">Not supported.</span></span>    |
|<span data-ttu-id="d5b24-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d5b24-114">Application</span></span> | <span data-ttu-id="d5b24-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5b24-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5b24-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d5b24-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /connectors
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d5b24-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d5b24-117">Optional query parameters</span></span>
<span data-ttu-id="d5b24-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d5b24-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d5b24-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d5b24-119">Request headers</span></span>
| <span data-ttu-id="d5b24-120">名前</span><span class="sxs-lookup"><span data-stu-id="d5b24-120">Name</span></span>      |<span data-ttu-id="d5b24-121">説明</span><span class="sxs-lookup"><span data-stu-id="d5b24-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d5b24-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5b24-122">Authorization</span></span>  | <span data-ttu-id="d5b24-123">ベアラー.</span><span class="sxs-lookup"><span data-stu-id="d5b24-123">Bearer.</span></span> <span data-ttu-id="d5b24-124">必須</span><span class="sxs-lookup"><span data-stu-id="d5b24-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5b24-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="d5b24-125">Request body</span></span>
<span data-ttu-id="d5b24-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d5b24-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5b24-127">応答</span><span class="sxs-lookup"><span data-stu-id="d5b24-127">Response</span></span>

<span data-ttu-id="d5b24-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[connector](../resources/connector.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="d5b24-128">If successful, this method returns a `200 OK` response code and collection of [connector](../resources/connector.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d5b24-129">例</span><span class="sxs-lookup"><span data-stu-id="d5b24-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d5b24-130">要求</span><span class="sxs-lookup"><span data-stu-id="d5b24-130">Request</span></span>
<span data-ttu-id="d5b24-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d5b24-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_connectors"
}-->
```http
GET https://graph.microsoft.com/{ver}/connectors
```
##### <a name="response"></a><span data-ttu-id="d5b24-132">応答</span><span class="sxs-lookup"><span data-stu-id="d5b24-132">Response</span></span>
<span data-ttu-id="d5b24-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d5b24-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connector",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "value": [
    {
      "id": "id-value",
      "machineName": "machineName-value",
      "externalIp": "externalIp-value",
      "status": "status-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List connectors",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
