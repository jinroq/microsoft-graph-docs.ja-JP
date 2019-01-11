---
title: アプリケーションを取得します。
description: プロパティとアプリケーションのオブジェクトの関係を取得します。
localization_priority: Normal
ms.openlocfilehash: 9226e697f3e8439740003887d8560ffaac9df2fa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864492"
---
# <a name="get-application"></a><span data-ttu-id="6a8e4-103">アプリケーションを取得します。</span><span class="sxs-lookup"><span data-stu-id="6a8e4-103">Get Application</span></span>

> <span data-ttu-id="6a8e4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6a8e4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6a8e4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a8e4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6a8e4-106">プロパティとアプリケーションのオブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="6a8e4-106">Retrieve the properties and relationships of application object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6a8e4-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6a8e4-107">Permissions</span></span>
<span data-ttu-id="6a8e4-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6a8e4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a8e4-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6a8e4-110">Permission type</span></span>      | <span data-ttu-id="6a8e4-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6a8e4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a8e4-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6a8e4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6a8e4-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a8e4-113">Not supported.</span></span>    |
|<span data-ttu-id="6a8e4-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6a8e4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a8e4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a8e4-115">Not supported.</span></span>    |
|<span data-ttu-id="6a8e4-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6a8e4-116">Application</span></span> | <span data-ttu-id="6a8e4-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a8e4-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a8e4-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6a8e4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/application
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6a8e4-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6a8e4-119">Optional query parameters</span></span>
<span data-ttu-id="6a8e4-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6a8e4-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6a8e4-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6a8e4-121">Request headers</span></span>
| <span data-ttu-id="6a8e4-122">名前</span><span class="sxs-lookup"><span data-stu-id="6a8e4-122">Name</span></span>      |<span data-ttu-id="6a8e4-123">説明</span><span class="sxs-lookup"><span data-stu-id="6a8e4-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6a8e4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a8e4-124">Authorization</span></span>  | <span data-ttu-id="6a8e4-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6a8e4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a8e4-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="6a8e4-127">Request body</span></span>
<span data-ttu-id="6a8e4-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6a8e4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a8e4-129">応答</span><span class="sxs-lookup"><span data-stu-id="6a8e4-129">Response</span></span>

<span data-ttu-id="6a8e4-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本体にある[アプリケーション](../resources/application.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="6a8e4-130">If successful, this method returns a `200 OK` response code and [Application](../resources/application.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6a8e4-131">例</span><span class="sxs-lookup"><span data-stu-id="6a8e4-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6a8e4-132">要求</span><span class="sxs-lookup"><span data-stu-id="6a8e4-132">Request</span></span>
<span data-ttu-id="6a8e4-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6a8e4-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_application"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/application
```
##### <a name="response"></a><span data-ttu-id="6a8e4-134">応答</span><span class="sxs-lookup"><span data-stu-id="6a8e4-134">Response</span></span>
<span data-ttu-id="6a8e4-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6a8e4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 48

{
  "calculationMode": "calculationMode-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Application",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
