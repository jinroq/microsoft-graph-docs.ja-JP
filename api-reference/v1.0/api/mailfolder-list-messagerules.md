---
title: ルールを一覧表示する
description: ユーザーの受信トレイに定義されているすべての messageRule オブジェクトを取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 1026f66efc6e20881be0daac3f419d5a8258051e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565570"
---
# <a name="list-rules"></a><span data-ttu-id="04f88-103">ルールを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="04f88-103">List rules</span></span>

<span data-ttu-id="04f88-104">ユーザーの受信トレイに定義されているすべての [messageRule](../resources/messagerule.md) オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="04f88-104">Get all the [messageRule](../resources/messagerule.md) objects defined for the user's Inbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="04f88-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="04f88-105">Permissions</span></span>
<span data-ttu-id="04f88-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="04f88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04f88-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="04f88-108">Permission type</span></span>      | <span data-ttu-id="04f88-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="04f88-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04f88-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="04f88-110">Delegated (work or school account)</span></span> | <span data-ttu-id="04f88-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="04f88-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="04f88-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="04f88-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04f88-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="04f88-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="04f88-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="04f88-114">Application</span></span> | <span data-ttu-id="04f88-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="04f88-115">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="04f88-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="04f88-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messageRules
GET /users/{id | userPrincipalName}/mailFolders/inbox/messageRules
```
## <a name="optional-query-parameters"></a><span data-ttu-id="04f88-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="04f88-117">Optional query parameters</span></span>
<span data-ttu-id="04f88-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="04f88-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="04f88-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="04f88-119">Request headers</span></span>
| <span data-ttu-id="04f88-120">名前</span><span class="sxs-lookup"><span data-stu-id="04f88-120">Name</span></span>       | <span data-ttu-id="04f88-121">型</span><span class="sxs-lookup"><span data-stu-id="04f88-121">Type</span></span> | <span data-ttu-id="04f88-122">説明</span><span class="sxs-lookup"><span data-stu-id="04f88-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="04f88-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="04f88-123">Authorization</span></span>  | <span data-ttu-id="04f88-124">string</span><span class="sxs-lookup"><span data-stu-id="04f88-124">string</span></span>  | <span data-ttu-id="04f88-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="04f88-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="04f88-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="04f88-127">Request body</span></span>
<span data-ttu-id="04f88-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="04f88-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="04f88-129">応答</span><span class="sxs-lookup"><span data-stu-id="04f88-129">Response</span></span>
<span data-ttu-id="04f88-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文に [messageRule](../resources/messagerule.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="04f88-130">If successful, this method returns a `200 OK` response code and collection of [messageRule](../resources/messagerule.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="04f88-131">例</span><span class="sxs-lookup"><span data-stu-id="04f88-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="04f88-132">要求</span><span class="sxs-lookup"><span data-stu-id="04f88-132">Request</span></span>
<span data-ttu-id="04f88-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="04f88-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox"],
  "name": "get_messagerules"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules
```
##### <a name="response"></a><span data-ttu-id="04f88-134">応答</span><span class="sxs-lookup"><span data-stu-id="04f88-134">Response</span></span>
<span data-ttu-id="04f88-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="04f88-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Me/mailFolders('inbox')/messageRules",
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
<!-- {
  "type": "#page.annotation",
  "description": "List rules",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
