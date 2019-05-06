---
title: ルールを取得する
description: messageRule オブジェクトのプロパティとリレーションシップを取得します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 06d824e8cb761b4ffadc0b95284cdfb5326a285b
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33597917"
---
# <a name="get-rule"></a><span data-ttu-id="46443-103">ルールを取得する</span><span class="sxs-lookup"><span data-stu-id="46443-103">Get rule</span></span>


<span data-ttu-id="46443-104">[messageRule](../resources/messagerule.md) オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="46443-104">Get the properties and relationships of a [messageRule](../resources/messagerule.md) object.</span></span>


## <a name="permissions"></a><span data-ttu-id="46443-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="46443-105">Permissions</span></span>
<span data-ttu-id="46443-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="46443-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46443-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="46443-108">Permission type</span></span>      | <span data-ttu-id="46443-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="46443-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46443-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="46443-110">Delegated (work or school account)</span></span> | <span data-ttu-id="46443-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="46443-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="46443-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="46443-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46443-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="46443-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="46443-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="46443-114">Application</span></span> | <span data-ttu-id="46443-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="46443-115">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="46443-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="46443-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messageRules/{id}
GET /users/{id | userPrincipalName}/mailFolders/inbox/messageRules/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="46443-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="46443-117">Optional query parameters</span></span>
<span data-ttu-id="46443-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="46443-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="46443-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="46443-119">Request headers</span></span>
| <span data-ttu-id="46443-120">名前</span><span class="sxs-lookup"><span data-stu-id="46443-120">Name</span></span>      |<span data-ttu-id="46443-121">説明</span><span class="sxs-lookup"><span data-stu-id="46443-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="46443-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="46443-122">Authorization</span></span>  | <span data-ttu-id="46443-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="46443-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="46443-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="46443-125">Request body</span></span>
<span data-ttu-id="46443-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="46443-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="46443-127">応答</span><span class="sxs-lookup"><span data-stu-id="46443-127">Response</span></span>
<span data-ttu-id="46443-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文に [messageRule](../resources/messagerule.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="46443-128">If successful, this method returns a `200 OK` response code and [messageRule](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="46443-129">例</span><span class="sxs-lookup"><span data-stu-id="46443-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="46443-130">要求</span><span class="sxs-lookup"><span data-stu-id="46443-130">Request</span></span>
<span data-ttu-id="46443-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="46443-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox", "AQAAAJ5dZqA="],
  "name": "get_messagerule"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules/AQAAAJ5dZqA=
```
##### <a name="response"></a><span data-ttu-id="46443-132">応答</span><span class="sxs-lookup"><span data-stu-id="46443-132">Response</span></span>
<span data-ttu-id="46443-133">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="46443-133">Here is an example of the response.</span></span> <span data-ttu-id="46443-134">既定では、応答に含まれる日時のプロパティは UTC 形式になります。</span><span class="sxs-lookup"><span data-stu-id="46443-134">By default, the date-time properties in the response are in UTC.</span></span> 

<span data-ttu-id="46443-p104">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="46443-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="46443-137">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="46443-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="46443-138">Visual</span><span class="sxs-lookup"><span data-stu-id="46443-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_messagerule-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="46443-139">Java</span><span class="sxs-lookup"><span data-stu-id="46443-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_messagerule-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/messagerule-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/messagerule-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
