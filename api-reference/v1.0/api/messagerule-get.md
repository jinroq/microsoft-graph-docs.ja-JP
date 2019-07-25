---
title: ルールを取得する
description: messageRule オブジェクトのプロパティとリレーションシップを取得します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 839955c24d91da45c5066a4c4588d4c69ac6ba98
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890392"
---
# <a name="get-rule"></a><span data-ttu-id="40d53-103">ルールを取得する</span><span class="sxs-lookup"><span data-stu-id="40d53-103">Get rule</span></span>


<span data-ttu-id="40d53-104">[messageRule](../resources/messagerule.md) オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="40d53-104">Get the properties and relationships of a [messageRule](../resources/messagerule.md) object.</span></span>


## <a name="permissions"></a><span data-ttu-id="40d53-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="40d53-105">Permissions</span></span>
<span data-ttu-id="40d53-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="40d53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40d53-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="40d53-108">Permission type</span></span>      | <span data-ttu-id="40d53-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="40d53-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40d53-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="40d53-110">Delegated (work or school account)</span></span> | <span data-ttu-id="40d53-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="40d53-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="40d53-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="40d53-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40d53-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="40d53-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="40d53-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="40d53-114">Application</span></span> | <span data-ttu-id="40d53-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="40d53-115">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="40d53-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="40d53-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messageRules/{id}
GET /users/{id | userPrincipalName}/mailFolders/inbox/messageRules/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="40d53-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="40d53-117">Optional query parameters</span></span>
<span data-ttu-id="40d53-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="40d53-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="40d53-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="40d53-119">Request headers</span></span>
| <span data-ttu-id="40d53-120">名前</span><span class="sxs-lookup"><span data-stu-id="40d53-120">Name</span></span>      |<span data-ttu-id="40d53-121">説明</span><span class="sxs-lookup"><span data-stu-id="40d53-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="40d53-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="40d53-122">Authorization</span></span>  | <span data-ttu-id="40d53-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="40d53-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="40d53-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="40d53-125">Request body</span></span>
<span data-ttu-id="40d53-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="40d53-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="40d53-127">応答</span><span class="sxs-lookup"><span data-stu-id="40d53-127">Response</span></span>
<span data-ttu-id="40d53-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文に [messageRule](../resources/messagerule.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="40d53-128">If successful, this method returns a `200 OK` response code and [messageRule](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="40d53-129">例</span><span class="sxs-lookup"><span data-stu-id="40d53-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="40d53-130">要求</span><span class="sxs-lookup"><span data-stu-id="40d53-130">Request</span></span>
<span data-ttu-id="40d53-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="40d53-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="40d53-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="40d53-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox", "AQAAAJ5dZqA="],
  "name": "get_messagerule"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules/AQAAAJ5dZqA=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="40d53-133">C#</span><span class="sxs-lookup"><span data-stu-id="40d53-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messagerule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="40d53-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="40d53-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messagerule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="40d53-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="40d53-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messagerule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="40d53-136">Java</span><span class="sxs-lookup"><span data-stu-id="40d53-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messagerule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="40d53-137">応答</span><span class="sxs-lookup"><span data-stu-id="40d53-137">Response</span></span>
<span data-ttu-id="40d53-138">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="40d53-138">Here is an example of the response.</span></span> <span data-ttu-id="40d53-139">既定では、応答に含まれる日時のプロパティは UTC 形式になります。</span><span class="sxs-lookup"><span data-stu-id="40d53-139">By default, the date-time properties in the response are in UTC.</span></span> 

<span data-ttu-id="40d53-p104">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="40d53-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
