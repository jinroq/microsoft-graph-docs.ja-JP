# <a name="list-verificationdnsrecords"></a><span data-ttu-id="38697-101">verificationDnsRecords を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="38697-101">List verificationDnsRecords</span></span>

<span data-ttu-id="38697-102">[domainDnsRecord](../resources/domaindnsrecord.md) オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="38697-102">Retrieve a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects.</span></span>

<span data-ttu-id="38697-p101">所有権を検証しないと、関連するドメインを Azure AD テナントで使用することはできません。ドメインの所有権を検証するには、ドメイン検証レコードを取得し、ドメインのゾーン ファイルに詳細を追加します。この作業は、ドメイン レジストラーによって、または DNS サーバーの構成で行えます。</span><span class="sxs-lookup"><span data-stu-id="38697-p101">You cannot use an associated domain with your Azure AD tenant until ownership is verified. To verify the ownership of the domain, retrieve the domain verification records and add the details to the zone file of the domain. This can be done through the domain registrar or DNS server configuration.</span></span>

<span data-ttu-id="38697-p102">ルート ドメインには検証が必要です。たとえば、contoso.com には検証が必要です。ルート ドメインが検証されると、ルート ドメインのサブドメインが自動的に検証されます。たとえば、contoso.com が検証されると、subdomain.contoso.com が自動的に検証されます。</span><span class="sxs-lookup"><span data-stu-id="38697-p102">Root domains require verification. For example, contoso.com requires verification. If a root domain is verified, subdomains of the root domain are automatically verified. For example, subdomain.contoso.com is automatically be verified if contoso.com has been verified.</span></span>

## <a name="permissions"></a><span data-ttu-id="38697-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="38697-110">Permissions</span></span>

<span data-ttu-id="38697-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="38697-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="38697-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="38697-113">Permission type</span></span>      | <span data-ttu-id="38697-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="38697-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38697-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="38697-115">Delegated (work or school account)</span></span> | <span data-ttu-id="38697-116">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="38697-116">Directory.Read.All</span></span>    |
|<span data-ttu-id="38697-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="38697-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38697-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="38697-118">Not supported.</span></span>    |
|<span data-ttu-id="38697-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="38697-119">Application</span></span> | <span data-ttu-id="38697-120">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38697-120">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="38697-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="38697-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/verificationDnsRecords
```

> <span data-ttu-id="38697-122">{Id} には、ドメインを完全修飾ドメイン名で指定します。</span><span class="sxs-lookup"><span data-stu-id="38697-122">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="38697-123">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="38697-123">Optional query parameters</span></span>

<span data-ttu-id="38697-124">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://graph.microsoft.io/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="38697-124">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="38697-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="38697-125">Request headers</span></span>

| <span data-ttu-id="38697-126">名前</span><span class="sxs-lookup"><span data-stu-id="38697-126">Name</span></span>      |<span data-ttu-id="38697-127">説明</span><span class="sxs-lookup"><span data-stu-id="38697-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="38697-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="38697-128">Authorization</span></span>  | <span data-ttu-id="38697-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="38697-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="38697-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="38697-131">Content-Type</span></span>  | <span data-ttu-id="38697-132">application/json</span><span class="sxs-lookup"><span data-stu-id="38697-132">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="38697-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="38697-133">Request body</span></span>

<span data-ttu-id="38697-134">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="38697-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38697-135">応答</span><span class="sxs-lookup"><span data-stu-id="38697-135">Response</span></span>

<span data-ttu-id="38697-136">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [domainDnsRecord](../resources/domaindnsrecord.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="38697-136">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38697-137">例</span><span class="sxs-lookup"><span data-stu-id="38697-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="38697-138">要求</span><span class="sxs-lookup"><span data-stu-id="38697-138">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_verificationdnsrecords"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains/contoso.com/verificationDnsRecords
```

##### <a name="response"></a><span data-ttu-id="38697-139">応答</span><span class="sxs-lookup"><span data-stu-id="38697-139">Response</span></span>

<span data-ttu-id="38697-p105">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="38697-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domainDnsRecord",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 220

{
  "value": [
    {
      "isOptional": false,
      "label": "contoso.com",
      "recordType": "Mx",
      "supportedService": "Email",
      "ttl": 3600,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List verificationDnsRecords",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->