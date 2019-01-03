---
title: リスト trendingAround
description: ユーザーの周りのトレンド分析項目の一覧を返す計算の把握。
author: dkershaw10
ms.openlocfilehash: 2f2595cbaacc74053b23d6b26b64fb9a17e2924a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333832"
---
# <a name="list-trendingaround"></a><span data-ttu-id="3e552-103">リスト trendingAround</span><span class="sxs-lookup"><span data-stu-id="3e552-103">List trendingAround</span></span>

> <span data-ttu-id="3e552-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3e552-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3e552-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3e552-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3e552-106">ユーザーの周りのトレンド分析項目の一覧を返す計算の把握。</span><span class="sxs-lookup"><span data-stu-id="3e552-106">Calculated insight that returns the list of items trending around a user.</span></span>

<span data-ttu-id="3e552-107">**注:** この API は廃止し、[トレンド分析の API](../resources/insights-trending.md)に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="3e552-107">**Note:** This API will be deprecated and replaced by the [Trending API](../resources/insights-trending.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3e552-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3e552-108">Permissions</span></span>
<span data-ttu-id="3e552-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3e552-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e552-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3e552-111">Permission type</span></span>      | <span data-ttu-id="3e552-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3e552-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e552-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3e552-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3e552-114">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="3e552-114">Sites.Read.All</span></span>    |
|<span data-ttu-id="3e552-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3e552-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e552-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3e552-116">Not supported.</span></span>    |
|<span data-ttu-id="3e552-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3e552-117">Application</span></span> | <span data-ttu-id="3e552-118">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="3e552-118">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e552-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3e552-119">HTTP request</span></span>
```http
GET /me/trendingAround
GET /users/{id | userPrincipalName}/trendingAround
GET /drive/root/createdByUser/trendingAround
GET /drive/root/lastModifiedByUser/trendingAround
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3e552-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="3e552-120">Optional query parameters</span></span>
<span data-ttu-id="3e552-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="3e552-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3e552-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3e552-122">Request headers</span></span>
| <span data-ttu-id="3e552-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3e552-123">Header</span></span>         | <span data-ttu-id="3e552-124">値</span><span class="sxs-lookup"><span data-stu-id="3e552-124">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="3e552-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e552-125">Authorization</span></span>  | <span data-ttu-id="3e552-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3e552-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3e552-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3e552-128">Content-Type</span></span>   | <span data-ttu-id="3e552-129">application/json</span><span class="sxs-lookup"><span data-stu-id="3e552-129">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="3e552-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="3e552-130">Request body</span></span>
<span data-ttu-id="3e552-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3e552-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e552-132">応答</span><span class="sxs-lookup"><span data-stu-id="3e552-132">Response</span></span>

<span data-ttu-id="3e552-133">成功した場合、このメソッドは、応答の本体で、200 OK 応答コードと[driveItem](../resources/driveitem.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="3e552-133">If successful, this method returns a 200 OK response code and collection of [driveItem](../resources/driveitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e552-134">例</span><span class="sxs-lookup"><span data-stu-id="3e552-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3e552-135">要求</span><span class="sxs-lookup"><span data-stu-id="3e552-135">Request</span></span>
```http
GET https://graph.microsoft.com/beta/me/trendingAround
```
##### <a name="response"></a><span data-ttu-id="3e552-136">応答</span><span class="sxs-lookup"><span data-stu-id="3e552-136">Response</span></span>
<span data-ttu-id="3e552-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3e552-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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