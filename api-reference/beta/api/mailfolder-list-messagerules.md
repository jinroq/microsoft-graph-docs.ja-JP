---
title: ルールを一覧表示する
description: ユーザーの受信トレイに定義されているすべての messageRule オブジェクトを取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c6e800ab7a42d38b397cfcfd4426e59f4b9ae80b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35984070"
---
# <a name="list-rules"></a><span data-ttu-id="421b6-103">ルールを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="421b6-103">List rules</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="421b6-104">ユーザーの受信トレイに定義されているすべての [messageRule](../resources/messagerule.md) オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="421b6-104">Get all the [messageRule](../resources/messagerule.md) objects defined for the user's Inbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="421b6-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="421b6-105">Permissions</span></span>
<span data-ttu-id="421b6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="421b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="421b6-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="421b6-108">Permission type</span></span>      | <span data-ttu-id="421b6-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="421b6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="421b6-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="421b6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="421b6-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="421b6-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="421b6-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="421b6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="421b6-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="421b6-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="421b6-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="421b6-114">Application</span></span> | <span data-ttu-id="421b6-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="421b6-115">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="421b6-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="421b6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messagerules
GET /users/{id | userPrincipalName}/mailFolders/inbox/messagerules
```
## <a name="optional-query-parameters"></a><span data-ttu-id="421b6-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="421b6-117">Optional query parameters</span></span>
<span data-ttu-id="421b6-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="421b6-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="421b6-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="421b6-119">Request headers</span></span>
| <span data-ttu-id="421b6-120">名前</span><span class="sxs-lookup"><span data-stu-id="421b6-120">Name</span></span>       | <span data-ttu-id="421b6-121">型</span><span class="sxs-lookup"><span data-stu-id="421b6-121">Type</span></span> | <span data-ttu-id="421b6-122">説明</span><span class="sxs-lookup"><span data-stu-id="421b6-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="421b6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="421b6-123">Authorization</span></span>  | <span data-ttu-id="421b6-124">string</span><span class="sxs-lookup"><span data-stu-id="421b6-124">string</span></span>  | <span data-ttu-id="421b6-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="421b6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="421b6-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="421b6-127">Request body</span></span>
<span data-ttu-id="421b6-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="421b6-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="421b6-129">応答</span><span class="sxs-lookup"><span data-stu-id="421b6-129">Response</span></span>
<span data-ttu-id="421b6-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文に [messageRule](../resources/messagerule.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="421b6-130">If successful, this method returns a `200 OK` response code and collection of [messageRule](../resources/messagerule.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="421b6-131">例</span><span class="sxs-lookup"><span data-stu-id="421b6-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="421b6-132">要求</span><span class="sxs-lookup"><span data-stu-id="421b6-132">Request</span></span>
<span data-ttu-id="421b6-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="421b6-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="421b6-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="421b6-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messagerules"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/inbox/messagerules
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="421b6-135">C#</span><span class="sxs-lookup"><span data-stu-id="421b6-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messagerules-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="421b6-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="421b6-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messagerules-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="421b6-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="421b6-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messagerules-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="421b6-138">Java</span><span class="sxs-lookup"><span data-stu-id="421b6-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messagerules-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="421b6-139">応答</span><span class="sxs-lookup"><span data-stu-id="421b6-139">Response</span></span>
<span data-ttu-id="421b6-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="421b6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messageRule",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Me/mailFolders('inbox')/messageRules",
  "value":[
    {
      "id":"AQAAAJ5dZp8=",
      "displayName":"Remove spam",
      "sequence":1,
      "isEnabled":true,
      "hasError":false,
      "isReadOnly":false,
      "conditions":{
        "subjectContains":[
          "enter to win"
        ]
      },
      "actions":{
        "delete":true,
        "stopProcessingRules":true
      }
    },
    {
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
  ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List rules",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
