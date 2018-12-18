---
title: ルールを取得する
description: messageRule オブジェクトのプロパティとリレーションシップを取得します。
author: angelgolfer-ms
ms.openlocfilehash: 425b5043e1ef173ef05033862ae5e705960987f6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342330"
---
# <a name="get-rule"></a><span data-ttu-id="15156-103">ルールを取得する</span><span class="sxs-lookup"><span data-stu-id="15156-103">Get rule</span></span>

> <span data-ttu-id="15156-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="15156-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15156-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15156-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="15156-106">[messageRule](../resources/messagerule.md) オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="15156-106">Get the properties and relationships of a [messageRule](../resources/messagerule.md) object.</span></span>


## <a name="permissions"></a><span data-ttu-id="15156-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="15156-107">Permissions</span></span>
<span data-ttu-id="15156-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="15156-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15156-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="15156-110">Permission type</span></span>      | <span data-ttu-id="15156-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="15156-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15156-112">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="15156-112">Delegated (work or school account)</span></span> | <span data-ttu-id="15156-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="15156-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="15156-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="15156-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15156-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="15156-115">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="15156-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="15156-116">Application</span></span> | <span data-ttu-id="15156-117">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="15156-117">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="15156-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="15156-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messagerules/{id}
GET /users/{id | userPrincipalName}/mailFolders/inbox/messagerules/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="15156-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="15156-119">Optional query parameters</span></span>
<span data-ttu-id="15156-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="15156-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="15156-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="15156-121">Request headers</span></span>
| <span data-ttu-id="15156-122">名前</span><span class="sxs-lookup"><span data-stu-id="15156-122">Name</span></span>      |<span data-ttu-id="15156-123">説明</span><span class="sxs-lookup"><span data-stu-id="15156-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="15156-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="15156-124">Authorization</span></span>  | <span data-ttu-id="15156-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="15156-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="15156-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="15156-127">Request body</span></span>
<span data-ttu-id="15156-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="15156-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="15156-129">応答</span><span class="sxs-lookup"><span data-stu-id="15156-129">Response</span></span>
<span data-ttu-id="15156-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文に [messageRule](../resources/messagerule.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="15156-130">If successful, this method returns a `200 OK` response code and [messageRule](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="15156-131">例</span><span class="sxs-lookup"><span data-stu-id="15156-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="15156-132">要求</span><span class="sxs-lookup"><span data-stu-id="15156-132">Request</span></span>
<span data-ttu-id="15156-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="15156-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messagerule"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailfolders/inbox/messagerules('AQAAAJ5dZqA=')
```
##### <a name="response"></a><span data-ttu-id="15156-134">応答</span><span class="sxs-lookup"><span data-stu-id="15156-134">Response</span></span>
<span data-ttu-id="15156-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="15156-135">Here is an example of the response.</span></span> <span data-ttu-id="15156-136">既定では、応答に含まれる日時のプロパティは UTC 形式になります。</span><span class="sxs-lookup"><span data-stu-id="15156-136">By default, the date-time properties in the response are in UTC.</span></span> 

<span data-ttu-id="15156-p105">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="15156-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->