# <a name="outlookuser-supportedlanguages"></a><span data-ttu-id="1e35f-101">outlookUser: supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="1e35f-101">outlookUser: supportedLanguages</span></span>

<span data-ttu-id="1e35f-102">ユーザーに対してサポートされている (ユーザーのメールボックス サーバーで構成されている) ロケールと言語のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="1e35f-102">Get the list of locales and languages that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="1e35f-103">Outlook クライアントを設定する際は、このサポートされているリストから、優先する言語を選択します。</span><span class="sxs-lookup"><span data-stu-id="1e35f-103">When setting up an Outlook client, the user selects the preferred language from this supported list.</span></span> <span data-ttu-id="1e35f-104">これにより、[ユーザーのメールボックス設定を取得](user_get_mailboxsettings.md)することによって、優先言語を取得できるようになります。</span><span class="sxs-lookup"><span data-stu-id="1e35f-104">The user's preferred language is selected from this supported list. You can get the preferred language by [getting the user's mailbox settings](user_get_mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="1e35f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1e35f-105">Permissions</span></span>
<span data-ttu-id="1e35f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1e35f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1e35f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1e35f-108">Permission type</span></span>      | <span data-ttu-id="1e35f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1e35f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e35f-110">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="1e35f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1e35f-111">User.Read、User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="1e35f-111">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="1e35f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1e35f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e35f-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="1e35f-113">User.Read</span></span>    |
|<span data-ttu-id="1e35f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1e35f-114">Application</span></span> | <span data-ttu-id="1e35f-115">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e35f-115">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e35f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1e35f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedLanguages
GET /users/{id|userPrincipalName}/outlook/supportedLanguages
```
## <a name="request-headers"></a><span data-ttu-id="1e35f-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1e35f-117">Request headers</span></span>
| <span data-ttu-id="1e35f-118">名前</span><span class="sxs-lookup"><span data-stu-id="1e35f-118">Name</span></span>       | <span data-ttu-id="1e35f-119">型</span><span class="sxs-lookup"><span data-stu-id="1e35f-119">Type</span></span> | <span data-ttu-id="1e35f-120">説明</span><span class="sxs-lookup"><span data-stu-id="1e35f-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1e35f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e35f-121">Authorization</span></span>  | <span data-ttu-id="1e35f-122">string</span><span class="sxs-lookup"><span data-stu-id="1e35f-122">string</span></span>  | <span data-ttu-id="1e35f-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1e35f-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="1e35f-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="1e35f-125">Request body</span></span>
<span data-ttu-id="1e35f-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1e35f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e35f-127">応答</span><span class="sxs-lookup"><span data-stu-id="1e35f-127">Response</span></span>
<span data-ttu-id="1e35f-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文に [localeInfo](../resources/localeinfo.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="1e35f-128">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/localeinfo.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e35f-129">例</span><span class="sxs-lookup"><span data-stu-id="1e35f-129">Example</span></span>
<span data-ttu-id="1e35f-130">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="1e35f-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1e35f-131">要求</span><span class="sxs-lookup"><span data-stu-id="1e35f-131">Request</span></span>
<span data-ttu-id="1e35f-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1e35f-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_supportedlanguages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/outlook/supportedLanguages
```

##### <a name="response"></a><span data-ttu-id="1e35f-133">応答</span><span class="sxs-lookup"><span data-stu-id="1e35f-133">Response</span></span>
<span data-ttu-id="1e35f-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="1e35f-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.localeInfo",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.localeInfo)",
  "value":[
    {
      "locale":"af-ZA",
      "displayName":"Afrikaans (Suid-Afrika)"
    },
    {
      "locale":"en-US",
      "displayName":"English (United States)"
    },
    {
       "locale":"en-CA",
       "displayName":"English (Canada)"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: supportedLanguages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->