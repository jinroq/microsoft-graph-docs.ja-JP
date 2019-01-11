---
title: 所有者を一覧表示する
description: DirectoryObject オブジェクトのリストを取得します。
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 37bdd7088460ae5d4ff70f3bbde271778c922115
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814239"
---
# <a name="list-owners"></a><span data-ttu-id="769be-103">所有者を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="769be-103">List owners</span></span>

> <span data-ttu-id="769be-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="769be-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="769be-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="769be-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="769be-106">DirectoryObject オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="769be-106">Retrieve a list of directoryObject objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="769be-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="769be-107">Permissions</span></span>
<span data-ttu-id="769be-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="769be-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="769be-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="769be-110">Permission type</span></span>      | <span data-ttu-id="769be-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="769be-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="769be-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="769be-112">Delegated (work or school account)</span></span> | <span data-ttu-id="769be-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="769be-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="769be-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="769be-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="769be-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="769be-115">Not supported.</span></span>    |
|<span data-ttu-id="769be-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="769be-116">Application</span></span> | <span data-ttu-id="769be-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="769be-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="769be-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="769be-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}/owners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="769be-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="769be-119">Optional query parameters</span></span>
<span data-ttu-id="769be-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="769be-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="769be-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="769be-121">Request headers</span></span>
| <span data-ttu-id="769be-122">名前</span><span class="sxs-lookup"><span data-stu-id="769be-122">Name</span></span>       | <span data-ttu-id="769be-123">種類</span><span class="sxs-lookup"><span data-stu-id="769be-123">Type</span></span> | <span data-ttu-id="769be-124">説明</span><span class="sxs-lookup"><span data-stu-id="769be-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="769be-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="769be-125">Authorization</span></span>  | <span data-ttu-id="769be-126">string</span><span class="sxs-lookup"><span data-stu-id="769be-126">string</span></span>  | <span data-ttu-id="769be-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="769be-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="769be-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="769be-129">Request body</span></span>
<span data-ttu-id="769be-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="769be-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="769be-131">応答</span><span class="sxs-lookup"><span data-stu-id="769be-131">Response</span></span>

<span data-ttu-id="769be-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="769be-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="769be-133">例</span><span class="sxs-lookup"><span data-stu-id="769be-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="769be-134">要求</span><span class="sxs-lookup"><span data-stu-id="769be-134">Request</span></span>
<span data-ttu-id="769be-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="769be-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->
```http
GET https://graph.microsoft.com/beta/applications/{id}/owners
```
##### <a name="response"></a><span data-ttu-id="769be-136">応答</span><span class="sxs-lookup"><span data-stu-id="769be-136">Response</span></span>
<span data-ttu-id="769be-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="769be-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
