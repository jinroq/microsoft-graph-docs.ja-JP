# <a name="outlookuser-supportedtimezones"></a><span data-ttu-id="75043-101">outlookUser: supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="75043-101">outlookUser: supportedTimeZones</span></span>

<span data-ttu-id="75043-102">ユーザーに対してサポートされている (ユーザーのメールボックス サーバーで構成されている) タイム ゾーンのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="75043-102">Get the list of time zones that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="75043-103">Windows のタイム ゾーン形式または [Internet Assigned Numbers Authority (IANA) のタイム ゾーン](http://www.iana.org/time-zones) (別称: Olson タイム ゾーン) 形式でタイム ゾーンが返されるよう、明示的に指定できます。</span><span class="sxs-lookup"><span data-stu-id="75043-103">You can explicitly specify to have time zones returned in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](http://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="75043-104">既定値は Windows 形式です。</span><span class="sxs-lookup"><span data-stu-id="75043-104">The Windows format is the default.</span></span>

<span data-ttu-id="75043-105">Outlook クライアントを設定する際は、このサポートされているリストから、優先するタイム ゾーンを選択します。</span><span class="sxs-lookup"><span data-stu-id="75043-105">When setting up an Outlook client, the user selects the preferred time zone from this supported list.</span></span> <span data-ttu-id="75043-106">これにより、[ユーザーのメールボックス設定を取得](user_get_mailboxsettings.md)することによって、優先タイム ゾーンを取得できるようになります。</span><span class="sxs-lookup"><span data-stu-id="75043-106">You can subsequently get the preferred time zone by [getting the user's mailbox settings](user_get_mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="75043-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="75043-107">Permissions</span></span>
<span data-ttu-id="75043-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="75043-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="75043-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="75043-110">Permission type</span></span>      | <span data-ttu-id="75043-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="75043-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75043-112">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="75043-112">Delegated (work or school account)</span></span> | <span data-ttu-id="75043-113">User.Read、User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="75043-113">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="75043-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="75043-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75043-115">User.Read</span><span class="sxs-lookup"><span data-stu-id="75043-115">User.Read</span></span>    |
|<span data-ttu-id="75043-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="75043-116">Application</span></span> | <span data-ttu-id="75043-117">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="75043-117">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="75043-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="75043-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedTimeZones
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones

GET /me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
```

## <a name="function-parameters"></a><span data-ttu-id="75043-119">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="75043-119">Function parameters</span></span>
| <span data-ttu-id="75043-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="75043-120">Parameter</span></span>       | <span data-ttu-id="75043-121">型</span><span class="sxs-lookup"><span data-stu-id="75043-121">Type</span></span> | <span data-ttu-id="75043-122">説明</span><span class="sxs-lookup"><span data-stu-id="75043-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="75043-123">TimeZoneStandard</span><span class="sxs-lookup"><span data-stu-id="75043-123">TimeZoneStandard</span></span>  | <span data-ttu-id="75043-124">TimeZoneStandard</span><span class="sxs-lookup"><span data-stu-id="75043-124">TimeZoneStandard</span></span>  | <span data-ttu-id="75043-125">タイム ゾーンの形式。</span><span class="sxs-lookup"><span data-stu-id="75043-125">A time zone format.</span></span> <span data-ttu-id="75043-126">サポートされている値は `Windows` および `Iana` です。</span><span class="sxs-lookup"><span data-stu-id="75043-126">Supported values are: `Windows`, and `Iana`.</span></span> <span data-ttu-id="75043-127">省略可能。</span><span class="sxs-lookup"><span data-stu-id="75043-127">Optional.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="75043-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="75043-128">Request headers</span></span>
| <span data-ttu-id="75043-129">名前</span><span class="sxs-lookup"><span data-stu-id="75043-129">Name</span></span>       | <span data-ttu-id="75043-130">型</span><span class="sxs-lookup"><span data-stu-id="75043-130">Type</span></span> | <span data-ttu-id="75043-131">説明</span><span class="sxs-lookup"><span data-stu-id="75043-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="75043-132">承認</span><span class="sxs-lookup"><span data-stu-id="75043-132">Authorization</span></span>  | <span data-ttu-id="75043-133">string</span><span class="sxs-lookup"><span data-stu-id="75043-133">string</span></span>  | <span data-ttu-id="75043-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="75043-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="75043-136">要求本文</span><span class="sxs-lookup"><span data-stu-id="75043-136">Request body</span></span>
<span data-ttu-id="75043-137">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="75043-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75043-138">応答</span><span class="sxs-lookup"><span data-stu-id="75043-138">Response</span></span>
<span data-ttu-id="75043-139">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文に [timeZoneInformation](../resources/timezoneinformation.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="75043-139">If successful, this method returns `200 OK` response code and a collection of [timeZoneInformation](../resources/timezoneinformation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75043-140">例</span><span class="sxs-lookup"><span data-stu-id="75043-140">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="75043-141">要求 1</span><span class="sxs-lookup"><span data-stu-id="75043-141">Request 1</span></span>
<span data-ttu-id="75043-142">次の例では、`timeZoneStandard` パラメーターを指定せずに、Windows のタイム ゾーン形式で表記されたサポート対象タイム ゾーンのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="75043-142">The following example does not specify the `timeZoneStandard` parameter, and gets the list of supported time zones represented in the Windows time zone format.</span></span> 
<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_default"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/outlook/supportedTimeZones
```

##### <a name="response-1"></a><span data-ttu-id="75043-143">応答 1</span><span class="sxs-lookup"><span data-stu-id="75043-143">Response 1</span></span>
<span data-ttu-id="75043-144">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="75043-144">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "name": "user_supportedtimezones_default",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeZoneInformation",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.timeZoneInformation)",
  "value":[
    {
      "alias":"Dateline Standard Time",
      "displayName":"(UTC-12:00) International Date Line West"
    },
    {
      "alias":"Samoa Standard Time",
      "displayName":"(UTC+13:00) Samoa"
    },
    {
       "alias":"UTC-11",
       "displayName":"(UTC-11:00) Coordinated Universal Time-11"
    },
    {
      "alias":"Aleutian Standard Time",
      "displayName":"(UTC-10:00) Aleutian Islands"
    }
  ]
}
```

##### <a name="request-2"></a><span data-ttu-id="75043-145">要求 2</span><span class="sxs-lookup"><span data-stu-id="75043-145">Request 2</span></span>
<span data-ttu-id="75043-146">次の例では、`TimeZoneStandard` パラメーターに `Iana` を指定して、IANA 形式で表記されたサポート対象タイム ゾーンのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="75043-146">The following example specifies `Iana` for the `TimeZoneStandard` parameter, and gets the list of supported time zones represented in IANA format.</span></span> 

<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_iana"
} -->

```http
GET https://graph.microsoft.com/v1.0/me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'Iana')
```

##### <a name="response-2"></a><span data-ttu-id="75043-147">応答 2</span><span class="sxs-lookup"><span data-stu-id="75043-147">Response 2</span></span>
<span data-ttu-id="75043-148">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="75043-148">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "name": "user_supportedtimezones_iana",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeZoneInformation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.timeZoneInformation)",
  "value":[
    {
      "alias":"Etc/GMT+12",
      "displayName":"Etc/GMT+12"
    },
    {
      "alias":"US/Samoa",
      "displayName":"US/Samoa"
    },
    {
      "alias":"Etc/GMT+11",
      "displayName":"Etc/GMT+11"
    },
    {
      "alias":"US/Aleutian",
      "displayName":"US/Aleutian"
    }
  ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: supportedTimeZones",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->