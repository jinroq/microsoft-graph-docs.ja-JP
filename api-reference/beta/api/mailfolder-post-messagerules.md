---
title: ルールを作成する
description: '条件とアクションのセットを指定して messageRule オブジェクトを作成します。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: c21ab70c723e9a97711e87559dc06856672fee0f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970424"
---
# <a name="create-rule"></a><span data-ttu-id="a1bf0-103">ルールを作成する</span><span class="sxs-lookup"><span data-stu-id="a1bf0-103">Create rule</span></span>

> <span data-ttu-id="a1bf0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a1bf0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a1bf0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1bf0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a1bf0-106">条件とアクションのセットを指定して [messageRule](../resources/messagerule.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a1bf0-106">Create a [messageRule](../resources/messagerule.md) object by specifying a set of conditions and actions.</span></span> 

<span data-ttu-id="a1bf0-107">Outlook では、ユーザーの受信トレイで受信したメッセージが指定した条件を満たしている場合に、それらのアクションが実行されます。</span><span class="sxs-lookup"><span data-stu-id="a1bf0-107">Outlook carries out those actions if an incoming message in the user's Inbox meets the specified conditions.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1bf0-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a1bf0-108">Permissions</span></span>
<span data-ttu-id="a1bf0-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a1bf0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1bf0-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a1bf0-111">Permission type</span></span>      | <span data-ttu-id="a1bf0-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a1bf0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1bf0-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a1bf0-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a1bf0-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a1bf0-114">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="a1bf0-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a1bf0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1bf0-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a1bf0-116">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="a1bf0-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a1bf0-117">Application</span></span> | <span data-ttu-id="a1bf0-118">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a1bf0-118">MailboxSettings.ReadWrite</span></span> |


## <a name="http-request"></a><span data-ttu-id="a1bf0-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a1bf0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/inbox/messagerules
POST /users/{id | userPrincipalName}/mailFolders/inbox/messagerules
```
## <a name="request-headers"></a><span data-ttu-id="a1bf0-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a1bf0-120">Request headers</span></span>
| <span data-ttu-id="a1bf0-121">名前</span><span class="sxs-lookup"><span data-stu-id="a1bf0-121">Name</span></span>       | <span data-ttu-id="a1bf0-122">説明</span><span class="sxs-lookup"><span data-stu-id="a1bf0-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a1bf0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1bf0-123">Authorization</span></span>  | <span data-ttu-id="a1bf0-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a1bf0-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="a1bf0-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a1bf0-126">Request body</span></span>
<span data-ttu-id="a1bf0-127">要求本文に、ルールを適用するパラメーターを指定します。</span><span class="sxs-lookup"><span data-stu-id="a1bf0-127">In the request body, supply the parameters that are applicable to your rule.</span></span> <span data-ttu-id="a1bf0-128">ルールを作成する際に本文に通常指定するパラメーターは、次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="a1bf0-128">The following are body parameters that are typically used when creating rules.</span></span> <span data-ttu-id="a1bf0-129">必要に応じて、本文に他の書き込み可能な **messageRule** プロパティを指定することもできます。</span><span class="sxs-lookup"><span data-stu-id="a1bf0-129">You can specify any other writable **messageRule** properties as appropriate in the request body.</span></span>

| <span data-ttu-id="a1bf0-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="a1bf0-130">Parameter</span></span>       | <span data-ttu-id="a1bf0-131">型</span><span class="sxs-lookup"><span data-stu-id="a1bf0-131">Type</span></span>|<span data-ttu-id="a1bf0-132">説明</span><span class="sxs-lookup"><span data-stu-id="a1bf0-132">Description</span></span>|
|:--------|:-------|:----------|
|<span data-ttu-id="a1bf0-133">actions</span><span class="sxs-lookup"><span data-stu-id="a1bf0-133">actions</span></span>|[<span data-ttu-id="a1bf0-134">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="a1bf0-134">messageRuleActions</span></span>](../resources/messageruleactions.md)|<span data-ttu-id="a1bf0-p105">該当する条件があり、それが満たされる場合にメッセージに対して実行されるアクションです。必須。</span><span class="sxs-lookup"><span data-stu-id="a1bf0-p105">Actions to be taken on a message when the corresponding conditions, if any, are fulfilled. Required.</span></span>|
|<span data-ttu-id="a1bf0-137">conditions</span><span class="sxs-lookup"><span data-stu-id="a1bf0-137">conditions</span></span>|[<span data-ttu-id="a1bf0-138">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="a1bf0-138">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)|<span data-ttu-id="a1bf0-p106">満たされた場合に、そのルールに該当するアクションをトリガーする条件です。省略可能。</span><span class="sxs-lookup"><span data-stu-id="a1bf0-p106">Conditions that when fulfilled, will trigger the corresponding actions for that rule. Optional.</span></span>|
|<span data-ttu-id="a1bf0-141">displayName</span><span class="sxs-lookup"><span data-stu-id="a1bf0-141">displayName</span></span>| <span data-ttu-id="a1bf0-142">String</span><span class="sxs-lookup"><span data-stu-id="a1bf0-142">String</span></span>  | <span data-ttu-id="a1bf0-p107">ルールの表示名。必須。</span><span class="sxs-lookup"><span data-stu-id="a1bf0-p107">The display name of the rule. Required.</span></span>|
|<span data-ttu-id="a1bf0-145">exceptions</span><span class="sxs-lookup"><span data-stu-id="a1bf0-145">exceptions</span></span>| [<span data-ttu-id="a1bf0-146">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="a1bf0-146">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)| <span data-ttu-id="a1bf0-p108">ルールの例外条件を表します。省略可能。</span><span class="sxs-lookup"><span data-stu-id="a1bf0-p108">Represents exception conditions for the rule. Optional.</span></span> |
|<span data-ttu-id="a1bf0-149">isEnabled</span><span class="sxs-lookup"><span data-stu-id="a1bf0-149">isEnabled</span></span> | <span data-ttu-id="a1bf0-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1bf0-150">Boolean</span></span> | <span data-ttu-id="a1bf0-p109">メッセージに対するルールの適用が有効になっているかどうかを示します。省略可能。</span><span class="sxs-lookup"><span data-stu-id="a1bf0-p109">Indicates whether the rule is enabled to be applied to messages. Optional.</span></span> |
|<span data-ttu-id="a1bf0-153">sequence</span><span class="sxs-lookup"><span data-stu-id="a1bf0-153">sequence</span></span>| <span data-ttu-id="a1bf0-154">Int32</span><span class="sxs-lookup"><span data-stu-id="a1bf0-154">Int32</span></span> | <span data-ttu-id="a1bf0-p110">他のルールもある中で、そのルールが実行される順序を示します。必須。</span><span class="sxs-lookup"><span data-stu-id="a1bf0-p110">Indicates the order in which the rule is executed, among other rules. Required.</span></span>|

## <a name="response"></a><span data-ttu-id="a1bf0-157">応答</span><span class="sxs-lookup"><span data-stu-id="a1bf0-157">Response</span></span>
<span data-ttu-id="a1bf0-158">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文に **messageRule** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a1bf0-158">If successful, this method returns `201 Created` response code and a **messageRule** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1bf0-159">例</span><span class="sxs-lookup"><span data-stu-id="a1bf0-159">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a1bf0-160">要求</span><span class="sxs-lookup"><span data-stu-id="a1bf0-160">Request</span></span>
<span data-ttu-id="a1bf0-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a1bf0-161">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="a1bf0-162">応答</span><span class="sxs-lookup"><span data-stu-id="a1bf0-162">Response</span></span>
<span data-ttu-id="a1bf0-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a1bf0-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
