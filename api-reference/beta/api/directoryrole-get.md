---
title: directoryRole を取得する
description: directoryRole オブジェクトのプロパティを取得します。
author: lleonard-msft
ms.openlocfilehash: efb3de57c8cc0a36a11c5af873ee1507927e2e38
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302948"
---
# <a name="get-directoryrole"></a><span data-ttu-id="7b6a1-103">directoryRole を取得する</span><span class="sxs-lookup"><span data-stu-id="7b6a1-103">Get directoryRole</span></span>

> <span data-ttu-id="7b6a1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7b6a1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7b6a1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7b6a1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7b6a1-106">directoryRole オブジェクトのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="7b6a1-106">Retrieve the properties of a directoryRole object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7b6a1-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7b6a1-107">Permissions</span></span>
<span data-ttu-id="7b6a1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7b6a1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b6a1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7b6a1-110">Permission type</span></span>      | <span data-ttu-id="7b6a1-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7b6a1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b6a1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7b6a1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7b6a1-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7b6a1-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7b6a1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7b6a1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b6a1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7b6a1-115">Not supported.</span></span>    |
|<span data-ttu-id="7b6a1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7b6a1-116">Application</span></span> | <span data-ttu-id="7b6a1-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b6a1-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b6a1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7b6a1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7b6a1-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7b6a1-119">Optional query parameters</span></span>
<span data-ttu-id="7b6a1-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポート**していません** (例: $filter はここではサポートされていません)。</span><span class="sxs-lookup"><span data-stu-id="7b6a1-120">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7b6a1-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7b6a1-121">Request headers</span></span>
| <span data-ttu-id="7b6a1-122">名前</span><span class="sxs-lookup"><span data-stu-id="7b6a1-122">Name</span></span>       | <span data-ttu-id="7b6a1-123">種類</span><span class="sxs-lookup"><span data-stu-id="7b6a1-123">Type</span></span> | <span data-ttu-id="7b6a1-124">説明</span><span class="sxs-lookup"><span data-stu-id="7b6a1-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7b6a1-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b6a1-125">Authorization</span></span>  | <span data-ttu-id="7b6a1-126">string</span><span class="sxs-lookup"><span data-stu-id="7b6a1-126">string</span></span>  | <span data-ttu-id="7b6a1-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7b6a1-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7b6a1-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="7b6a1-129">Request body</span></span>
<span data-ttu-id="7b6a1-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7b6a1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b6a1-131">応答</span><span class="sxs-lookup"><span data-stu-id="7b6a1-131">Response</span></span>

<span data-ttu-id="7b6a1-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryRole](../resources/directoryrole.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7b6a1-132">If successful, this method returns a `200 OK` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7b6a1-133">例</span><span class="sxs-lookup"><span data-stu-id="7b6a1-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7b6a1-134">要求</span><span class="sxs-lookup"><span data-stu-id="7b6a1-134">Request</span></span>
<span data-ttu-id="7b6a1-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7b6a1-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directoryrole"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoles/{id}
```
##### <a name="response"></a><span data-ttu-id="7b6a1-136">応答</span><span class="sxs-lookup"><span data-stu-id="7b6a1-136">Response</span></span>
<span data-ttu-id="7b6a1-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7b6a1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 142

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->