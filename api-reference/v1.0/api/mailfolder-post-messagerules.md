---
title: ルールを作成する
description: '条件とアクションのセットを指定して messageRule オブジェクトを作成します。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: c1c8470e7d82f6898fc4895d9ddb27eef254638a
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33612279"
---
# <a name="create-rule"></a><span data-ttu-id="f673d-103">ルールを作成する</span><span class="sxs-lookup"><span data-stu-id="f673d-103">Create rule</span></span>


<span data-ttu-id="f673d-104">条件とアクションのセットを指定して [messageRule](../resources/messagerule.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f673d-104">Create a [messageRule](../resources/messagerule.md) object by specifying a set of conditions and actions.</span></span> 

<span data-ttu-id="f673d-105">Outlook では、ユーザーの受信トレイで受信したメッセージが指定した条件を満たしている場合に、それらのアクションが実行されます。</span><span class="sxs-lookup"><span data-stu-id="f673d-105">Outlook carries out those actions if an incoming message in the user's Inbox meets the specified conditions.</span></span>

## <a name="permissions"></a><span data-ttu-id="f673d-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f673d-106">Permissions</span></span>
<span data-ttu-id="f673d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f673d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f673d-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f673d-109">Permission type</span></span>      | <span data-ttu-id="f673d-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f673d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f673d-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f673d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f673d-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f673d-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="f673d-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f673d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f673d-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f673d-114">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="f673d-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f673d-115">Application</span></span> | <span data-ttu-id="f673d-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f673d-116">MailboxSettings.ReadWrite</span></span> |


## <a name="http-request"></a><span data-ttu-id="f673d-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f673d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/inbox/messageRules
POST /users/{id | userPrincipalName}/mailFolders/inbox/messageRules
```
## <a name="request-headers"></a><span data-ttu-id="f673d-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f673d-118">Request headers</span></span>
| <span data-ttu-id="f673d-119">名前</span><span class="sxs-lookup"><span data-stu-id="f673d-119">Name</span></span>       | <span data-ttu-id="f673d-120">説明</span><span class="sxs-lookup"><span data-stu-id="f673d-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f673d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f673d-121">Authorization</span></span>  | <span data-ttu-id="f673d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f673d-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="f673d-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="f673d-124">Request body</span></span>
<span data-ttu-id="f673d-125">要求本文に、ルールを適用するパラメーターを指定します。</span><span class="sxs-lookup"><span data-stu-id="f673d-125">In the request body, supply the parameters that are applicable to your rule.</span></span> <span data-ttu-id="f673d-126">ルールを作成する際に本文に通常指定するパラメーターは、次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="f673d-126">The following are body parameters that are typically used when creating rules.</span></span> <span data-ttu-id="f673d-127">必要に応じて、本文に他の書き込み可能な **messageRule** プロパティを指定することもできます。</span><span class="sxs-lookup"><span data-stu-id="f673d-127">You can specify any other writable **messageRule** properties as appropriate in the request body.</span></span>

| <span data-ttu-id="f673d-128">名前</span><span class="sxs-lookup"><span data-stu-id="f673d-128">Name</span></span>       | <span data-ttu-id="f673d-129">型</span><span class="sxs-lookup"><span data-stu-id="f673d-129">Type</span></span>|<span data-ttu-id="f673d-130">説明</span><span class="sxs-lookup"><span data-stu-id="f673d-130">Description</span></span>|
|:--------|:-------|:----------|
|<span data-ttu-id="f673d-131">actions</span><span class="sxs-lookup"><span data-stu-id="f673d-131">actions</span></span>|[<span data-ttu-id="f673d-132">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="f673d-132">messageRuleActions</span></span>](../resources/messageruleactions.md)|<span data-ttu-id="f673d-p104">該当する条件があり、それが満たされる場合にメッセージに対して実行されるアクションです。必須。</span><span class="sxs-lookup"><span data-stu-id="f673d-p104">Actions to be taken on a message when the corresponding conditions, if any, are fulfilled. Required.</span></span>|
|<span data-ttu-id="f673d-135">conditions</span><span class="sxs-lookup"><span data-stu-id="f673d-135">conditions</span></span>|[<span data-ttu-id="f673d-136">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="f673d-136">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)|<span data-ttu-id="f673d-p105">満たされた場合に、そのルールに該当するアクションをトリガーする条件です。省略可能。</span><span class="sxs-lookup"><span data-stu-id="f673d-p105">Conditions that when fulfilled, will trigger the corresponding actions for that rule. Optional.</span></span>|
|<span data-ttu-id="f673d-139">displayName</span><span class="sxs-lookup"><span data-stu-id="f673d-139">displayName</span></span>| <span data-ttu-id="f673d-140">String</span><span class="sxs-lookup"><span data-stu-id="f673d-140">String</span></span>  | <span data-ttu-id="f673d-p106">ルールの表示名。必須。</span><span class="sxs-lookup"><span data-stu-id="f673d-p106">The display name of the rule. Required.</span></span>|
|<span data-ttu-id="f673d-143">exceptions</span><span class="sxs-lookup"><span data-stu-id="f673d-143">exceptions</span></span>| [<span data-ttu-id="f673d-144">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="f673d-144">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)| <span data-ttu-id="f673d-p107">ルールの例外条件を表します。省略可能。</span><span class="sxs-lookup"><span data-stu-id="f673d-p107">Represents exception conditions for the rule. Optional.</span></span> |
|<span data-ttu-id="f673d-147">isEnabled</span><span class="sxs-lookup"><span data-stu-id="f673d-147">isEnabled</span></span> | <span data-ttu-id="f673d-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="f673d-148">Boolean</span></span> | <span data-ttu-id="f673d-p108">メッセージに対するルールの適用が有効になっているかどうかを示します。省略可能。</span><span class="sxs-lookup"><span data-stu-id="f673d-p108">Indicates whether the rule is enabled to be applied to messages. Optional.</span></span> |
|<span data-ttu-id="f673d-151">sequence</span><span class="sxs-lookup"><span data-stu-id="f673d-151">sequence</span></span>| <span data-ttu-id="f673d-152">Int32</span><span class="sxs-lookup"><span data-stu-id="f673d-152">Int32</span></span> | <span data-ttu-id="f673d-p109">他のルールもある中で、そのルールが実行される順序を示します。必須。</span><span class="sxs-lookup"><span data-stu-id="f673d-p109">Indicates the order in which the rule is executed, among other rules. Required.</span></span>|

## <a name="response"></a><span data-ttu-id="f673d-155">応答</span><span class="sxs-lookup"><span data-stu-id="f673d-155">Response</span></span>
<span data-ttu-id="f673d-156">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文に **messageRule** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f673d-156">If successful, this method returns `201 Created` response code and a **messageRule** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f673d-157">例</span><span class="sxs-lookup"><span data-stu-id="f673d-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f673d-158">要求</span><span class="sxs-lookup"><span data-stu-id="f673d-158">Request</span></span>
<span data-ttu-id="f673d-159">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f673d-159">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox"],
  "name": "create_messagerule_from_mailfolder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules
Content-type: application/json

{      
    "displayName": "From partner",      
    "sequence": 2,      
    "isEnabled": true,          
    "conditions": {
        "senderContains": [
          "adele"       
        ]
     },
     "actions": {
        "forwardTo": [
          {
             "emailAddress": {
                "name": "Alex Wilbur",
                "address": "AlexW@contoso.onmicrosoft.com"
              }
           }
        ],
        "stopProcessingRules": true
     }    
}

```
##### <a name="response"></a><span data-ttu-id="f673d-160">応答</span><span class="sxs-lookup"><span data-stu-id="f673d-160">Response</span></span>
<span data-ttu-id="f673d-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f673d-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messageRule"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

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

```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f673d-164">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="f673d-164">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f673d-165">Visual</span><span class="sxs-lookup"><span data-stu-id="f673d-165">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_messagerule_from_mailfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f673d-166">Java</span><span class="sxs-lookup"><span data-stu-id="f673d-166">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_messagerule_from_mailfolder-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/mailfolder-post-messagerules.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/mailfolder-post-messagerules.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
