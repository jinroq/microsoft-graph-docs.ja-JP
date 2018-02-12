# <a name="delete-domain"></a><span data-ttu-id="15723-101">ドメインを削除する</span><span class="sxs-lookup"><span data-stu-id="15723-101">Delete domain</span></span>

<span data-ttu-id="15723-102">テナントからドメインを削除します。</span><span class="sxs-lookup"><span data-stu-id="15723-102">Deletes a domain from a tenant.</span></span>

> <span data-ttu-id="15723-103">**重要:**</span><span class="sxs-lookup"><span data-stu-id="15723-103">**Important:**</span></span>
> - <span data-ttu-id="15723-104">削除されたドメインは回復できません。</span><span class="sxs-lookup"><span data-stu-id="15723-104">Deleted domains are not recoverable.</span></span><br />
> - <span data-ttu-id="15723-p101">ドメインにまだ依存しているリソースまたはオブジェクトがある場合、削除の試行は失敗します。[List domainNameReferences](domain_list_domainnamereferences.md) API を使用して、すべての依存リソースを探すことができます。</span><span class="sxs-lookup"><span data-stu-id="15723-p101">Attempts to delete will fail if there are any resources or objects still dependent on the domain. You can find all dependent resources by using the [List domainNameReferences](domain_list_domainnamereferences.md) API.</span></span>

## <a name="permissions"></a><span data-ttu-id="15723-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="15723-107">Permissions</span></span>

<span data-ttu-id="15723-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="15723-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="15723-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="15723-110">Permission type</span></span>      | <span data-ttu-id="15723-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="15723-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15723-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="15723-112">Delegated (work or school account)</span></span> | <span data-ttu-id="15723-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="15723-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="15723-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="15723-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15723-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15723-115">Not supported.</span></span>    |
|<span data-ttu-id="15723-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="15723-116">Application</span></span> | <span data-ttu-id="15723-117">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15723-117">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="15723-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="15723-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> <span data-ttu-id="15723-119">{Id} には、ドメインを完全修飾ドメイン名で指定します。</span><span class="sxs-lookup"><span data-stu-id="15723-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="15723-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="15723-120">Request headers</span></span>

| <span data-ttu-id="15723-121">名前</span><span class="sxs-lookup"><span data-stu-id="15723-121">Name</span></span>       | <span data-ttu-id="15723-122">説明</span><span class="sxs-lookup"><span data-stu-id="15723-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="15723-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="15723-123">Authorization</span></span>  | <span data-ttu-id="15723-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="15723-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="15723-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="15723-126">Content-Type</span></span>  | <span data-ttu-id="15723-127">application/json</span><span class="sxs-lookup"><span data-stu-id="15723-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="15723-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="15723-128">Request body</span></span>

<span data-ttu-id="15723-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="15723-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15723-130">応答</span><span class="sxs-lookup"><span data-stu-id="15723-130">Response</span></span>

<span data-ttu-id="15723-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文は返されません。</span><span class="sxs-lookup"><span data-stu-id="15723-p104">If successful, this method returns `204 No Content` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="15723-133">例</span><span class="sxs-lookup"><span data-stu-id="15723-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="15723-134">要求</span><span class="sxs-lookup"><span data-stu-id="15723-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/domains/contoso.com
```

##### <a name="response"></a><span data-ttu-id="15723-135">応答</span><span class="sxs-lookup"><span data-stu-id="15723-135">Response</span></span>

<span data-ttu-id="15723-p105">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="15723-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->