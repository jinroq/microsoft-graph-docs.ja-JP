---
title: Outlook カテゴリを取得する
description: 指定した outlookCategory オブジェクトのプロパティとリレーションシップを取得します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ab2d536dac104665ba17f07a4282905412b2fad7
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36414190"
---
# <a name="get-outlook-category"></a><span data-ttu-id="6ccb1-103">Outlook カテゴリを取得する</span><span class="sxs-lookup"><span data-stu-id="6ccb1-103">Get Outlook category</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ccb1-104">指定した [outlookCategory](../resources/outlookcategory.md) オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="6ccb1-104">Get the properties and relationships of the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ccb1-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6ccb1-105">Permissions</span></span>
<span data-ttu-id="6ccb1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6ccb1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ccb1-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6ccb1-108">Permission type</span></span>      | <span data-ttu-id="6ccb1-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6ccb1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ccb1-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6ccb1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6ccb1-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="6ccb1-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="6ccb1-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6ccb1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ccb1-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="6ccb1-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="6ccb1-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6ccb1-114">Application</span></span> | <span data-ttu-id="6ccb1-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="6ccb1-115">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ccb1-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6ccb1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/masterCategories/{id}
GET /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6ccb1-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6ccb1-117">Optional query parameters</span></span>
<span data-ttu-id="6ccb1-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6ccb1-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6ccb1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6ccb1-119">Request headers</span></span>
| <span data-ttu-id="6ccb1-120">名前</span><span class="sxs-lookup"><span data-stu-id="6ccb1-120">Name</span></span>      |<span data-ttu-id="6ccb1-121">説明</span><span class="sxs-lookup"><span data-stu-id="6ccb1-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6ccb1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ccb1-122">Authorization</span></span>  | <span data-ttu-id="6ccb1-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6ccb1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6ccb1-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="6ccb1-125">Request body</span></span>
<span data-ttu-id="6ccb1-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6ccb1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ccb1-127">応答</span><span class="sxs-lookup"><span data-stu-id="6ccb1-127">Response</span></span>

<span data-ttu-id="6ccb1-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文に [outlookCategory](../resources/outlookcategory.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6ccb1-128">If successful, this method returns a `200 OK` response code and [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6ccb1-129">例</span><span class="sxs-lookup"><span data-stu-id="6ccb1-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6ccb1-130">要求</span><span class="sxs-lookup"><span data-stu-id="6ccb1-130">Request</span></span>
<span data-ttu-id="6ccb1-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6ccb1-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6ccb1-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="6ccb1-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outlookcategory"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/masterCategories/de912e4d-c790-4da9-949c-ccd933aaa0f7
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6ccb1-133">C#</span><span class="sxs-lookup"><span data-stu-id="6ccb1-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outlookcategory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6ccb1-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6ccb1-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outlookcategory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6ccb1-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="6ccb1-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outlookcategory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6ccb1-136">応答</span><span class="sxs-lookup"><span data-stu-id="6ccb1-136">Response</span></span>
<span data-ttu-id="6ccb1-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6ccb1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 249

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"de912e4d-c790-4da9-949c-ccd933aaa0f7",
  "displayName":"Yellow category",
  "color":"preset3"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
