---
title: ルールを取得する
description: messageRule オブジェクトのプロパティとリレーションシップを取得します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: eef1f590161a600ec7852cf7af5a60ee024a3e94
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266039"
---
# <a name="get-rule"></a><span data-ttu-id="8551b-103">ルールを取得する</span><span class="sxs-lookup"><span data-stu-id="8551b-103">Get rule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8551b-104">[messageRule](../resources/messagerule.md) オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="8551b-104">Get the properties and relationships of a [messageRule](../resources/messagerule.md) object.</span></span>


## <a name="permissions"></a><span data-ttu-id="8551b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8551b-105">Permissions</span></span>
<span data-ttu-id="8551b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8551b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8551b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8551b-108">Permission type</span></span>      | <span data-ttu-id="8551b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8551b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8551b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8551b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8551b-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="8551b-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="8551b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8551b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8551b-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="8551b-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="8551b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8551b-114">Application</span></span> | <span data-ttu-id="8551b-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="8551b-115">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="8551b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8551b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messagerules/{id}
GET /users/{id | userPrincipalName}/mailFolders/inbox/messagerules/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8551b-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8551b-117">Optional query parameters</span></span>
<span data-ttu-id="8551b-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8551b-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8551b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8551b-119">Request headers</span></span>
| <span data-ttu-id="8551b-120">名前</span><span class="sxs-lookup"><span data-stu-id="8551b-120">Name</span></span>      |<span data-ttu-id="8551b-121">説明</span><span class="sxs-lookup"><span data-stu-id="8551b-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8551b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8551b-122">Authorization</span></span>  | <span data-ttu-id="8551b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8551b-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="8551b-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="8551b-125">Request body</span></span>
<span data-ttu-id="8551b-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8551b-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8551b-127">応答</span><span class="sxs-lookup"><span data-stu-id="8551b-127">Response</span></span>
<span data-ttu-id="8551b-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文に [messageRule](../resources/messagerule.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8551b-128">If successful, this method returns a `200 OK` response code and [messageRule](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8551b-129">例</span><span class="sxs-lookup"><span data-stu-id="8551b-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8551b-130">要求</span><span class="sxs-lookup"><span data-stu-id="8551b-130">Request</span></span>
<span data-ttu-id="8551b-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8551b-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messagerule"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailfolders/inbox/messagerules('AQAAAJ5dZqA=')
```
##### <a name="response"></a><span data-ttu-id="8551b-132">応答</span><span class="sxs-lookup"><span data-stu-id="8551b-132">Response</span></span>
<span data-ttu-id="8551b-133">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="8551b-133">Here is an example of the response.</span></span> <span data-ttu-id="8551b-134">既定では、応答に含まれる日時のプロパティは UTC 形式になります。</span><span class="sxs-lookup"><span data-stu-id="8551b-134">By default, the date-time properties in the response are in UTC.</span></span> 

<span data-ttu-id="8551b-p104">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8551b-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messageRule"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Me/mailFolders('inbox')/messageRules/$entity",
  "id":"AQAAAJ5dZqA=",
  "displayName":"From partner",
  "sequence":2,
  "isEnabled":true,
  "hasError":false,
  "isReadOnly":false,
  "conditions":{
    "senderContains":[
      "ADELE"
    ]
  },
  "actions":{
    "stopProcessingRules":true,
    "forwardTo":[
      {
        "emailAddress":{
          "name":"Alex Wilbur",
          "address":"AlexW@contoso.onmicrosoft.com"
        }
      }
    ]
  }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="8551b-137">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="8551b-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8551b-138">C#</span><span class="sxs-lookup"><span data-stu-id="8551b-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_messagerule-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8551b-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="8551b-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_messagerule-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="8551b-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="8551b-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_messagerule-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/messagerule-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/messagerule-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/messagerule-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
