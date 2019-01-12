---
title: Outlook カテゴリを取得する
description: 指定した outlookCategory オブジェクトのプロパティとリレーションシップを取得します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: c296aea62fec7090cb76607911f6be178f1ebdbb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949718"
---
# <a name="get-outlook-category"></a><span data-ttu-id="4615a-103">Outlook カテゴリを取得する</span><span class="sxs-lookup"><span data-stu-id="4615a-103">Get Outlook category</span></span>

> <span data-ttu-id="4615a-104">**重要**: [Microsoft Graph で/beta のバージョンの Api を選択し、プレビューでは、変更されることができます。</span><span class="sxs-lookup"><span data-stu-id="4615a-104">**Important**: APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4615a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4615a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4615a-106">指定した [outlookCategory](../resources/outlookcategory.md) オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="4615a-106">Get the properties and relationships of the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4615a-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4615a-107">Permissions</span></span>
<span data-ttu-id="4615a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4615a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4615a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4615a-110">Permission type</span></span>      | <span data-ttu-id="4615a-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4615a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4615a-112">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="4615a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4615a-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="4615a-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="4615a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4615a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4615a-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="4615a-115">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="4615a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4615a-116">Application</span></span> | <span data-ttu-id="4615a-117">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="4615a-117">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="4615a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4615a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/masterCategories/{id}
GET /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4615a-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="4615a-119">Optional query parameters</span></span>
<span data-ttu-id="4615a-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="4615a-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4615a-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4615a-121">Request headers</span></span>
| <span data-ttu-id="4615a-122">名前</span><span class="sxs-lookup"><span data-stu-id="4615a-122">Name</span></span>      |<span data-ttu-id="4615a-123">説明</span><span class="sxs-lookup"><span data-stu-id="4615a-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4615a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4615a-124">Authorization</span></span>  | <span data-ttu-id="4615a-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4615a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4615a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="4615a-127">Request body</span></span>
<span data-ttu-id="4615a-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4615a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4615a-129">応答</span><span class="sxs-lookup"><span data-stu-id="4615a-129">Response</span></span>

<span data-ttu-id="4615a-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文に [outlookCategory](../resources/outlookcategory.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4615a-130">If successful, this method returns a `200 OK` response code and [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4615a-131">例</span><span class="sxs-lookup"><span data-stu-id="4615a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4615a-132">要求</span><span class="sxs-lookup"><span data-stu-id="4615a-132">Request</span></span>
<span data-ttu-id="4615a-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4615a-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlookcategory"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/masterCategories('de912e4d-c790-4da9-949c-ccd933aaa0f7')
```
##### <a name="response"></a><span data-ttu-id="4615a-134">応答</span><span class="sxs-lookup"><span data-stu-id="4615a-134">Response</span></span>
<span data-ttu-id="4615a-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4615a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
