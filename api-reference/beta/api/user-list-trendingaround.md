---
title: リスト trendingAround
description: ユーザーの周囲でのアイテムのリストを返す、計算された洞察。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 625ae9d66ce1b891ebdba3209d92bd0e88b06a94
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544205"
---
# <a name="list-trendingaround"></a><span data-ttu-id="d4c69-103">リスト trendingAround</span><span class="sxs-lookup"><span data-stu-id="d4c69-103">List trendingAround</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4c69-104">ユーザーの周囲でのアイテムのリストを返す、計算された洞察。</span><span class="sxs-lookup"><span data-stu-id="d4c69-104">Calculated insight that returns the list of items trending around a user.</span></span>

<span data-ttu-id="d4c69-105">**注:** この api は非推奨になり、[トレンド api](../resources/insights-trending.md)に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="d4c69-105">**Note:** This API will be deprecated and replaced by the [Trending API](../resources/insights-trending.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d4c69-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d4c69-106">Permissions</span></span>
<span data-ttu-id="d4c69-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d4c69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4c69-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d4c69-109">Permission type</span></span>      | <span data-ttu-id="d4c69-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d4c69-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d4c69-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d4c69-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d4c69-112">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4c69-112">Sites.Read.All</span></span>    |
|<span data-ttu-id="d4c69-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d4c69-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4c69-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d4c69-114">Not supported.</span></span>    |
|<span data-ttu-id="d4c69-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d4c69-115">Application</span></span> | <span data-ttu-id="d4c69-116">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4c69-116">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4c69-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d4c69-117">HTTP request</span></span>
```http
GET /me/trendingAround
GET /users/{id | userPrincipalName}/trendingAround
GET /drive/root/createdByUser/trendingAround
GET /drive/root/lastModifiedByUser/trendingAround
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d4c69-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d4c69-118">Optional query parameters</span></span>
<span data-ttu-id="d4c69-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d4c69-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d4c69-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d4c69-120">Request headers</span></span>
| <span data-ttu-id="d4c69-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d4c69-121">Header</span></span>         | <span data-ttu-id="d4c69-122">値</span><span class="sxs-lookup"><span data-stu-id="d4c69-122">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="d4c69-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4c69-123">Authorization</span></span>  | <span data-ttu-id="d4c69-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d4c69-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d4c69-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d4c69-126">Content-Type</span></span>   | <span data-ttu-id="d4c69-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d4c69-127">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="d4c69-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="d4c69-128">Request body</span></span>
<span data-ttu-id="d4c69-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d4c69-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4c69-130">応答</span><span class="sxs-lookup"><span data-stu-id="d4c69-130">Response</span></span>

<span data-ttu-id="d4c69-131">成功した場合、このメソッドは、応答本文で 200 OK 応答コードと、[ハードアイテム](../resources/driveitem.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="d4c69-131">If successful, this method returns a 200 OK response code and collection of [driveItem](../resources/driveitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4c69-132">例</span><span class="sxs-lookup"><span data-stu-id="d4c69-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d4c69-133">要求</span><span class="sxs-lookup"><span data-stu-id="d4c69-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/me/trendingAround
```
##### <a name="response"></a><span data-ttu-id="d4c69-134">応答</span><span class="sxs-lookup"><span data-stu-id="d4c69-134">Response</span></span>
<span data-ttu-id="d4c69-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d4c69-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 226

{
  "id": "id-value",
  "name": "name-value",
  "DateTimeCreated": "DateTimeCreated-value",
  "DateTimeLastModified": "DateTimeLastModified-value",
  "webUrl": "webUrl-value",
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-trendingaround.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
