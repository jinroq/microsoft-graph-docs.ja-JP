# <a name="get-rule"></a><span data-ttu-id="02231-101">ルールを取得する</span><span class="sxs-lookup"><span data-stu-id="02231-101">Get rule</span></span>


<span data-ttu-id="02231-102">[messageRule](../resources/messagerule.md) オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="02231-102">Get the properties and relationships of a [messageRule](../resources/messagerule.md) object.</span></span>


## <a name="permissions"></a><span data-ttu-id="02231-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="02231-103">Permissions</span></span>
<span data-ttu-id="02231-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="02231-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="02231-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="02231-106">Permission type</span></span>      | <span data-ttu-id="02231-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="02231-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02231-108">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="02231-108">Delegated (work or school account)</span></span> | <span data-ttu-id="02231-109">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="02231-109">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="02231-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="02231-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02231-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="02231-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="02231-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="02231-112">Application</span></span> | <span data-ttu-id="02231-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="02231-113">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="02231-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="02231-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messageRules/{id}
GET /users/{id | userPrincipalName}/mailFolders/inbox/messageRules/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="02231-115">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="02231-115">Optional query parameters</span></span>
<span data-ttu-id="02231-116">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://graph.microsoft.io/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="02231-116">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="02231-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="02231-117">Request headers</span></span>
| <span data-ttu-id="02231-118">名前</span><span class="sxs-lookup"><span data-stu-id="02231-118">Name</span></span>      |<span data-ttu-id="02231-119">説明</span><span class="sxs-lookup"><span data-stu-id="02231-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="02231-120">承認</span><span class="sxs-lookup"><span data-stu-id="02231-120">Authorization</span></span>  | <span data-ttu-id="02231-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="02231-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="02231-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="02231-123">Request body</span></span>
<span data-ttu-id="02231-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="02231-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="02231-125">応答</span><span class="sxs-lookup"><span data-stu-id="02231-125">Response</span></span>
<span data-ttu-id="02231-126">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文に [messageRule](../resources/messagerule.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="02231-126">If successful, this method returns a `200 OK` response code and [messageRule](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="02231-127">例</span><span class="sxs-lookup"><span data-stu-id="02231-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="02231-128">要求</span><span class="sxs-lookup"><span data-stu-id="02231-128">Request</span></span>
<span data-ttu-id="02231-129">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="02231-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox", "AQAAAJ5dZqA="],
  "name": "get_messagerule"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules/AQAAAJ5dZqA=
```
##### <a name="response"></a><span data-ttu-id="02231-130">応答</span><span class="sxs-lookup"><span data-stu-id="02231-130">Response</span></span>
<span data-ttu-id="02231-131">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="02231-131">Here is an example of the response.</span></span> <span data-ttu-id="02231-132">既定では、応答に含まれる日時のプロパティは UTC 形式になります。</span><span class="sxs-lookup"><span data-stu-id="02231-132">By default, the date-time properties in the response are in UTC.</span></span> 

<span data-ttu-id="02231-p104">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="02231-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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