# <a name="update-domain"></a><span data-ttu-id="19783-101">ドメインを更新する</span><span class="sxs-lookup"><span data-stu-id="19783-101">Update domain</span></span>

<span data-ttu-id="19783-102">ドメイン オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="19783-102">Update the properties of domain object.</span></span>

> <span data-ttu-id="19783-103">**重要:** 検証済みのドメインのみを更新できます。</span><span class="sxs-lookup"><span data-stu-id="19783-103">**Important:** Only verified domains can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="19783-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="19783-104">Permissions</span></span>

<span data-ttu-id="19783-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="19783-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="19783-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="19783-107">Permission type</span></span>      | <span data-ttu-id="19783-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="19783-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19783-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="19783-109">Delegated (work or school account)</span></span> | <span data-ttu-id="19783-110">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="19783-110">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="19783-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="19783-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19783-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="19783-112">Not supported.</span></span>    |
|<span data-ttu-id="19783-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="19783-113">Application</span></span> | <span data-ttu-id="19783-114">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19783-114">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="19783-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="19783-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /domains/{id}
```

> <span data-ttu-id="19783-116">{Id} には、ドメインを完全修飾ドメイン名で指定します。</span><span class="sxs-lookup"><span data-stu-id="19783-116">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="19783-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="19783-117">Request headers</span></span>

| <span data-ttu-id="19783-118">名前</span><span class="sxs-lookup"><span data-stu-id="19783-118">Name</span></span>       | <span data-ttu-id="19783-119">説明</span><span class="sxs-lookup"><span data-stu-id="19783-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="19783-120">承認</span><span class="sxs-lookup"><span data-stu-id="19783-120">Authorization</span></span>  | <span data-ttu-id="19783-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="19783-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="19783-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="19783-123">Content-Type</span></span>  | <span data-ttu-id="19783-124">アプリケーション /json</span><span class="sxs-lookup"><span data-stu-id="19783-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="19783-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="19783-125">Request body</span></span>

<span data-ttu-id="19783-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るには、変更する値のみを含めます。</span><span class="sxs-lookup"><span data-stu-id="19783-p103">In the request body, supply the values for relevant fields to be updated. Existing properties not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance, only include changed values.</span></span>

## <a name="response"></a><span data-ttu-id="19783-129">応答</span><span class="sxs-lookup"><span data-stu-id="19783-129">Response</span></span>

<span data-ttu-id="19783-130">成功した場合、このメソッドは `204 No Content` 応答コードを返しますが、応答本文は返しません。</span><span class="sxs-lookup"><span data-stu-id="19783-130">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="19783-131">例</span><span class="sxs-lookup"><span data-stu-id="19783-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="19783-132">要求</span><span class="sxs-lookup"><span data-stu-id="19783-132">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["contoso.com"],
  "name": "update_domain"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/domains/contoso.com
Content-type: application/json

{
  "isDefault": true,
  "supportedServices": [
    "Email",
    "OfficeCommunicationsOnline"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="19783-133">応答</span><span class="sxs-lookup"><span data-stu-id="19783-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->