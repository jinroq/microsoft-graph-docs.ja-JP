# <a name="create-rule"></a><span data-ttu-id="98660-101">ルールを作成する</span><span class="sxs-lookup"><span data-stu-id="98660-101">Create rule</span></span>


<span data-ttu-id="98660-102">条件とアクションのセットを指定して [messageRule](../resources/messagerule.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="98660-102">Create a [messageRule](../resources/messagerule.md) object by specifying a set of conditions and actions.</span></span> 

<span data-ttu-id="98660-103">Outlook では、ユーザーの受信トレイで受信したメッセージが指定した条件を満たしている場合に、それらのアクションが実行されます。</span><span class="sxs-lookup"><span data-stu-id="98660-103">Outlook carries out those actions if an incoming message in the user's Inbox meets the specified conditions.</span></span>

## <a name="permissions"></a><span data-ttu-id="98660-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="98660-104">Permissions</span></span>
<span data-ttu-id="98660-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="98660-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="98660-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="98660-107">Permission type</span></span>      | <span data-ttu-id="98660-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="98660-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98660-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="98660-109">Delegated (work or school account)</span></span> | <span data-ttu-id="98660-110">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="98660-110">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="98660-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="98660-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98660-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="98660-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="98660-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="98660-113">Application</span></span> | <span data-ttu-id="98660-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="98660-114">MailboxSettings.ReadWrite</span></span> |


## <a name="http-request"></a><span data-ttu-id="98660-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="98660-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/inbox/messageRules
POST /users/{id | userPrincipalName}/mailFolders/inbox/messageRules
```
## <a name="request-headers"></a><span data-ttu-id="98660-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="98660-116">Request headers</span></span>
| <span data-ttu-id="98660-117">名前</span><span class="sxs-lookup"><span data-stu-id="98660-117">Name</span></span>       | <span data-ttu-id="98660-118">説明</span><span class="sxs-lookup"><span data-stu-id="98660-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="98660-119">承認</span><span class="sxs-lookup"><span data-stu-id="98660-119">Authorization</span></span>  | <span data-ttu-id="98660-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="98660-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="98660-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="98660-122">Request body</span></span>
<span data-ttu-id="98660-123">要求本文に、ルールを適用するパラメーターを指定します。</span><span class="sxs-lookup"><span data-stu-id="98660-123">In the request body, supply the parameters that are applicable to your rule.</span></span> <span data-ttu-id="98660-124">ルールを作成する際に本文に通常指定するパラメーターは、次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="98660-124">The following are body parameters that are typically used when creating rules.</span></span> <span data-ttu-id="98660-125">必要に応じて、本文に他の書き込み可能な **messageRule** プロパティを指定することもできます。</span><span class="sxs-lookup"><span data-stu-id="98660-125">You can specify any other writable **messageRule** properties as appropriate in the request body.</span></span>

| <span data-ttu-id="98660-126">名前</span><span class="sxs-lookup"><span data-stu-id="98660-126">Name</span></span>       | <span data-ttu-id="98660-127">型</span><span class="sxs-lookup"><span data-stu-id="98660-127">Type</span></span>|<span data-ttu-id="98660-128">説明</span><span class="sxs-lookup"><span data-stu-id="98660-128">Description</span></span>|
|:--------|:-------|:----------|
|<span data-ttu-id="98660-129">actions</span><span class="sxs-lookup"><span data-stu-id="98660-129">actions</span></span>|[<span data-ttu-id="98660-130">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="98660-130">messageRuleActions</span></span>](../resources/messageruleactions.md)|<span data-ttu-id="98660-p104">該当する条件があり、それが満たされる場合にメッセージに対して実行されるアクションです。必須。</span><span class="sxs-lookup"><span data-stu-id="98660-p104">Actions to be taken on a message when the corresponding conditions, if any, are fulfilled. Required.</span></span>|
|<span data-ttu-id="98660-133">conditions</span><span class="sxs-lookup"><span data-stu-id="98660-133">conditions</span></span>|[<span data-ttu-id="98660-134">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="98660-134">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)|<span data-ttu-id="98660-p105">満たされた場合に、そのルールに該当するアクションをトリガーする条件です。省略可能。</span><span class="sxs-lookup"><span data-stu-id="98660-p105">Conditions that when fulfilled, will trigger the corresponding actions for that rule. Optional.</span></span>|
|<span data-ttu-id="98660-137">displayName</span><span class="sxs-lookup"><span data-stu-id="98660-137">displayName</span></span>| <span data-ttu-id="98660-138">文字列</span><span class="sxs-lookup"><span data-stu-id="98660-138">String</span></span>  | <span data-ttu-id="98660-p106">ルールの表示名。必須。</span><span class="sxs-lookup"><span data-stu-id="98660-p106">The display name of the rule. Required.</span></span>|
|<span data-ttu-id="98660-141">exceptions</span><span class="sxs-lookup"><span data-stu-id="98660-141">exceptions</span></span>| [<span data-ttu-id="98660-142">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="98660-142">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)| <span data-ttu-id="98660-p107">ルールの例外条件を表します。省略可能。</span><span class="sxs-lookup"><span data-stu-id="98660-p107">Represents exception conditions for the rule. Optional.</span></span> |
|<span data-ttu-id="98660-145">isEnabled</span><span class="sxs-lookup"><span data-stu-id="98660-145">isEnabled</span></span> | <span data-ttu-id="98660-146">ブール値</span><span class="sxs-lookup"><span data-stu-id="98660-146">Boolean</span></span> | <span data-ttu-id="98660-p108">メッセージに対するルールの適用が有効になっているかどうかを示します。省略可能。</span><span class="sxs-lookup"><span data-stu-id="98660-p108">Indicates whether the rule is enabled to be applied to messages. Optional.</span></span> |
|<span data-ttu-id="98660-149">sequence</span><span class="sxs-lookup"><span data-stu-id="98660-149">sequence</span></span>| <span data-ttu-id="98660-150">Int32</span><span class="sxs-lookup"><span data-stu-id="98660-150">Int32</span></span> | <span data-ttu-id="98660-p109">他のルールもある中で、そのルールが実行される順序を示します。必須。</span><span class="sxs-lookup"><span data-stu-id="98660-p109">Indicates the order in which the rule is executed, among other rules. Required.</span></span>|

## <a name="response"></a><span data-ttu-id="98660-153">応答</span><span class="sxs-lookup"><span data-stu-id="98660-153">Response</span></span>
<span data-ttu-id="98660-154">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文に **messageRule** オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="98660-154">If successful, this method returns `201 Created` response code and a **messageRule** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98660-155">例</span><span class="sxs-lookup"><span data-stu-id="98660-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="98660-156">要求</span><span class="sxs-lookup"><span data-stu-id="98660-156">Request</span></span>
<span data-ttu-id="98660-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="98660-157">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="98660-158">応答</span><span class="sxs-lookup"><span data-stu-id="98660-158">Response</span></span>
<span data-ttu-id="98660-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="98660-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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