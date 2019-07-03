---
title: ルールを作成する
description: '条件とアクションのセットを指定して messageRule オブジェクトを作成します。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 6bfc4c9b31513b0ca549a4c0c4b5963a5dc734de
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35449527"
---
# <a name="create-rule"></a><span data-ttu-id="295ab-103">ルールを作成する</span><span class="sxs-lookup"><span data-stu-id="295ab-103">Create rule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="295ab-104">条件とアクションのセットを指定して [messageRule](../resources/messagerule.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="295ab-104">Create a [messageRule](../resources/messagerule.md) object by specifying a set of conditions and actions.</span></span> 

<span data-ttu-id="295ab-105">Outlook では、ユーザーの受信トレイで受信したメッセージが指定した条件を満たしている場合に、それらのアクションが実行されます。</span><span class="sxs-lookup"><span data-stu-id="295ab-105">Outlook carries out those actions if an incoming message in the user's Inbox meets the specified conditions.</span></span>

## <a name="permissions"></a><span data-ttu-id="295ab-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="295ab-106">Permissions</span></span>
<span data-ttu-id="295ab-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="295ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="295ab-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="295ab-109">Permission type</span></span>      | <span data-ttu-id="295ab-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="295ab-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="295ab-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="295ab-111">Delegated (work or school account)</span></span> | <span data-ttu-id="295ab-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="295ab-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="295ab-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="295ab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="295ab-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="295ab-114">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="295ab-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="295ab-115">Application</span></span> | <span data-ttu-id="295ab-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="295ab-116">MailboxSettings.ReadWrite</span></span> |


## <a name="http-request"></a><span data-ttu-id="295ab-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="295ab-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/inbox/messagerules
POST /users/{id | userPrincipalName}/mailFolders/inbox/messagerules
```
## <a name="request-headers"></a><span data-ttu-id="295ab-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="295ab-118">Request headers</span></span>
| <span data-ttu-id="295ab-119">名前</span><span class="sxs-lookup"><span data-stu-id="295ab-119">Name</span></span>       | <span data-ttu-id="295ab-120">説明</span><span class="sxs-lookup"><span data-stu-id="295ab-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="295ab-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="295ab-121">Authorization</span></span>  | <span data-ttu-id="295ab-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="295ab-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="295ab-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="295ab-124">Request body</span></span>
<span data-ttu-id="295ab-125">要求本文に、ルールを適用するパラメーターを指定します。</span><span class="sxs-lookup"><span data-stu-id="295ab-125">In the request body, supply the parameters that are applicable to your rule.</span></span> <span data-ttu-id="295ab-126">ルールを作成する際に本文に通常指定するパラメーターは、次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="295ab-126">The following are body parameters that are typically used when creating rules.</span></span> <span data-ttu-id="295ab-127">必要に応じて、本文に他の書き込み可能な **messageRule** プロパティを指定することもできます。</span><span class="sxs-lookup"><span data-stu-id="295ab-127">You can specify any other writable **messageRule** properties as appropriate in the request body.</span></span>

| <span data-ttu-id="295ab-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="295ab-128">Parameter</span></span>       | <span data-ttu-id="295ab-129">型</span><span class="sxs-lookup"><span data-stu-id="295ab-129">Type</span></span>|<span data-ttu-id="295ab-130">説明</span><span class="sxs-lookup"><span data-stu-id="295ab-130">Description</span></span>|
|:--------|:-------|:----------|
|<span data-ttu-id="295ab-131">actions</span><span class="sxs-lookup"><span data-stu-id="295ab-131">actions</span></span>|[<span data-ttu-id="295ab-132">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="295ab-132">messageRuleActions</span></span>](../resources/messageruleactions.md)|<span data-ttu-id="295ab-p104">該当する条件があり、それが満たされる場合にメッセージに対して実行されるアクションです。必須。</span><span class="sxs-lookup"><span data-stu-id="295ab-p104">Actions to be taken on a message when the corresponding conditions, if any, are fulfilled. Required.</span></span>|
|<span data-ttu-id="295ab-135">conditions</span><span class="sxs-lookup"><span data-stu-id="295ab-135">conditions</span></span>|[<span data-ttu-id="295ab-136">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="295ab-136">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)|<span data-ttu-id="295ab-p105">満たされた場合に、そのルールに該当するアクションをトリガーする条件です。省略可能。</span><span class="sxs-lookup"><span data-stu-id="295ab-p105">Conditions that when fulfilled, will trigger the corresponding actions for that rule. Optional.</span></span>|
|<span data-ttu-id="295ab-139">displayName</span><span class="sxs-lookup"><span data-stu-id="295ab-139">displayName</span></span>| <span data-ttu-id="295ab-140">String</span><span class="sxs-lookup"><span data-stu-id="295ab-140">String</span></span>  | <span data-ttu-id="295ab-p106">ルールの表示名。必須。</span><span class="sxs-lookup"><span data-stu-id="295ab-p106">The display name of the rule. Required.</span></span>|
|<span data-ttu-id="295ab-143">exceptions</span><span class="sxs-lookup"><span data-stu-id="295ab-143">exceptions</span></span>| [<span data-ttu-id="295ab-144">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="295ab-144">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)| <span data-ttu-id="295ab-p107">ルールの例外条件を表します。省略可能。</span><span class="sxs-lookup"><span data-stu-id="295ab-p107">Represents exception conditions for the rule. Optional.</span></span> |
|<span data-ttu-id="295ab-147">isEnabled</span><span class="sxs-lookup"><span data-stu-id="295ab-147">isEnabled</span></span> | <span data-ttu-id="295ab-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="295ab-148">Boolean</span></span> | <span data-ttu-id="295ab-p108">メッセージに対するルールの適用が有効になっているかどうかを示します。省略可能。</span><span class="sxs-lookup"><span data-stu-id="295ab-p108">Indicates whether the rule is enabled to be applied to messages. Optional.</span></span> |
|<span data-ttu-id="295ab-151">sequence</span><span class="sxs-lookup"><span data-stu-id="295ab-151">sequence</span></span>| <span data-ttu-id="295ab-152">Int32</span><span class="sxs-lookup"><span data-stu-id="295ab-152">Int32</span></span> | <span data-ttu-id="295ab-p109">他のルールもある中で、そのルールが実行される順序を示します。必須。</span><span class="sxs-lookup"><span data-stu-id="295ab-p109">Indicates the order in which the rule is executed, among other rules. Required.</span></span>|

## <a name="response"></a><span data-ttu-id="295ab-155">応答</span><span class="sxs-lookup"><span data-stu-id="295ab-155">Response</span></span>
<span data-ttu-id="295ab-156">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文に **messageRule** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="295ab-156">If successful, this method returns `201 Created` response code and a **messageRule** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="295ab-157">例</span><span class="sxs-lookup"><span data-stu-id="295ab-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="295ab-158">要求</span><span class="sxs-lookup"><span data-stu-id="295ab-158">Request</span></span>
<span data-ttu-id="295ab-159">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="295ab-159">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="295ab-160">プロトコル</span><span class="sxs-lookup"><span data-stu-id="295ab-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_messagerule_from_mailfolder"
}-->
```http
POST https://graph.microsoft.com/beta/me/mailFolders/inbox/messagerules
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="295ab-161">C#</span><span class="sxs-lookup"><span data-stu-id="295ab-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-messagerule-from-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="295ab-162">Javascript</span><span class="sxs-lookup"><span data-stu-id="295ab-162">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-messagerule-from-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="295ab-163">目的-C</span><span class="sxs-lookup"><span data-stu-id="295ab-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-messagerule-from-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="295ab-164">応答</span><span class="sxs-lookup"><span data-stu-id="295ab-164">Response</span></span>
<span data-ttu-id="295ab-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="295ab-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
