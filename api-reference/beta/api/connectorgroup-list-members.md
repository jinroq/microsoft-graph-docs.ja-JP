---
title: メンバーを一覧表示する
description: ConnectorGroup に関連付けられているコネクタ オブジェクトのリストを取得します。
ms.openlocfilehash: 504cba20c0d93db9f0c0333dcf7578e051b3009f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071013"
---
# <a name="list-members"></a><span data-ttu-id="33161-103">メンバーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="33161-103">List members</span></span>

> <span data-ttu-id="33161-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="33161-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="33161-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="33161-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="33161-106">ConnectorGroup に関連付けられているコネクタ オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="33161-106">Retrieve a list of connector objects associated with a connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="33161-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="33161-107">Permissions</span></span>
<span data-ttu-id="33161-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="33161-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33161-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="33161-110">Permission type</span></span>      | <span data-ttu-id="33161-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="33161-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33161-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="33161-112">Delegated (work or school account)</span></span> | <span data-ttu-id="33161-113">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="33161-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="33161-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="33161-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33161-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="33161-115">Not supported.</span></span>    |
|<span data-ttu-id="33161-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="33161-116">Application</span></span> | <span data-ttu-id="33161-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33161-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="33161-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="33161-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /connectorGroups/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="33161-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="33161-119">Optional query parameters</span></span>
<span data-ttu-id="33161-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="33161-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="33161-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="33161-121">Request headers</span></span>
| <span data-ttu-id="33161-122">名前</span><span class="sxs-lookup"><span data-stu-id="33161-122">Name</span></span>      |<span data-ttu-id="33161-123">説明</span><span class="sxs-lookup"><span data-stu-id="33161-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="33161-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="33161-124">Authorization</span></span>  | <span data-ttu-id="33161-125">ベアラーです。</span><span class="sxs-lookup"><span data-stu-id="33161-125">Bearer.</span></span> <span data-ttu-id="33161-126">必須</span><span class="sxs-lookup"><span data-stu-id="33161-126">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="33161-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="33161-127">Request body</span></span>
<span data-ttu-id="33161-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="33161-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33161-129">応答</span><span class="sxs-lookup"><span data-stu-id="33161-129">Response</span></span>

<span data-ttu-id="33161-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[コネクタ](../resources/connector.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="33161-130">If successful, this method returns a `200 OK` response code and collection of [connector](../resources/connector.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="33161-131">例</span><span class="sxs-lookup"><span data-stu-id="33161-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="33161-132">要求</span><span class="sxs-lookup"><span data-stu-id="33161-132">Request</span></span>
<span data-ttu-id="33161-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="33161-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/{ver}/connectorGroups/{id}/members
```
##### <a name="response"></a><span data-ttu-id="33161-134">応答</span><span class="sxs-lookup"><span data-stu-id="33161-134">Response</span></span>
<span data-ttu-id="33161-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="33161-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->