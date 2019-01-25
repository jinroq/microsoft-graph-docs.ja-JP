---
title: Outlook カテゴリを一覧表示する
description: ユーザーに対して定義されているすべてのカテゴリを取得します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 5a375079748be356b37cb2281f10da857cca2563
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523604"
---
# <a name="list-outlook-categories"></a><span data-ttu-id="49d06-103">Outlook カテゴリを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="49d06-103">List Outlook categories</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49d06-104">ユーザーに対して定義されているすべてのカテゴリを取得します。</span><span class="sxs-lookup"><span data-stu-id="49d06-104">Get all the categories that have been defined for the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="49d06-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="49d06-105">Permissions</span></span>
<span data-ttu-id="49d06-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="49d06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49d06-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="49d06-108">Permission type</span></span>      | <span data-ttu-id="49d06-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="49d06-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49d06-110">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="49d06-110">Delegated (work or school account)</span></span> | <span data-ttu-id="49d06-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="49d06-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="49d06-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="49d06-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49d06-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="49d06-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="49d06-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="49d06-114">Application</span></span> | <span data-ttu-id="49d06-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="49d06-115">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="49d06-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="49d06-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/masterCategories
GET /users/{id|userPrincipalName}/outlook/masterCategories
```
## <a name="optional-query-parameters"></a><span data-ttu-id="49d06-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="49d06-117">Optional query parameters</span></span>
<span data-ttu-id="49d06-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="49d06-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="49d06-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="49d06-119">Request headers</span></span>
| <span data-ttu-id="49d06-120">名前</span><span class="sxs-lookup"><span data-stu-id="49d06-120">Name</span></span>      |<span data-ttu-id="49d06-121">説明</span><span class="sxs-lookup"><span data-stu-id="49d06-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="49d06-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="49d06-122">Authorization</span></span>  | <span data-ttu-id="49d06-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="49d06-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="49d06-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="49d06-125">Request body</span></span>
<span data-ttu-id="49d06-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="49d06-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49d06-127">応答</span><span class="sxs-lookup"><span data-stu-id="49d06-127">Response</span></span>

<span data-ttu-id="49d06-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文に [outlookCategory](../resources/outlookcategory.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="49d06-128">If successful, this method returns a `200 OK` response code and collection of [outlookCategory](../resources/outlookcategory.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="49d06-129">例</span><span class="sxs-lookup"><span data-stu-id="49d06-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="49d06-130">要求</span><span class="sxs-lookup"><span data-stu-id="49d06-130">Request</span></span>
<span data-ttu-id="49d06-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="49d06-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mastercategories"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/masterCategories
```
##### <a name="response"></a><span data-ttu-id="49d06-132">応答</span><span class="sxs-lookup"><span data-stu-id="49d06-132">Response</span></span>
<span data-ttu-id="49d06-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="49d06-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 727

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories",
  "value":[
    {
      "id":"5a9a6aa8-b65f-4357-b1f9-60c6bf6330d8",
      "displayName":"Red category",
      "color":"preset0"
    },
    {
      "id":"4b1c2495-54c9-4a5e-90a2-0ab0b31987d8",
      "displayName":"Orange category",
      "color":"preset1"
    },
    {
      "id":"de912e4d-c790-4da9-949c-ccd933aaa0f7",
      "displayName":"Yellow category",
      "color":"preset3"
    },
    {
      "id":"79c8d8f8-9db1-49ec-99ce-ae25793e7232",
      "displayName":"Green category",
      "color":"preset4"
    },
    {
      "id":"626e696c-6a10-48b8-89b9-12de3160cfb9",
      "displayName":"Blue category",
      "color":"preset7"
    },
    {
      "id":"453d06d0-447d-41f7-91cd-aa0f6b190b5b",
      "displayName":"Purple category",
      "color":"preset8"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List categories",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlookuser-list-mastercategories.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
}-->
