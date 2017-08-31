# <a name="filter-apply"></a><span data-ttu-id="84f46-101">フィルター: 適用</span><span class="sxs-lookup"><span data-stu-id="84f46-101">Filter: apply</span></span>

<span data-ttu-id="84f46-102">指定した列に指定されたフィルター条件を適用します。</span><span class="sxs-lookup"><span data-stu-id="84f46-102">Apply the given filter criteria on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="84f46-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="84f46-103">Permissions</span></span>
<span data-ttu-id="84f46-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="84f46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="84f46-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="84f46-106">Permission type</span></span>      | <span data-ttu-id="84f46-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="84f46-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84f46-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="84f46-108">Delegated (work or school account)</span></span> | <span data-ttu-id="84f46-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84f46-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="84f46-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="84f46-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84f46-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="84f46-111">Not supported.</span></span>    |
|<span data-ttu-id="84f46-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="84f46-112">Application</span></span> | <span data-ttu-id="84f46-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="84f46-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="84f46-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="84f46-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/apply

```
## <a name="request-headers"></a><span data-ttu-id="84f46-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="84f46-115">Request headers</span></span>
| <span data-ttu-id="84f46-116">名前</span><span class="sxs-lookup"><span data-stu-id="84f46-116">Name</span></span>       | <span data-ttu-id="84f46-117">説明</span><span class="sxs-lookup"><span data-stu-id="84f46-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="84f46-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="84f46-118">Authorization</span></span>  | <span data-ttu-id="84f46-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="84f46-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="84f46-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="84f46-121">Request body</span></span>
<span data-ttu-id="84f46-122">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="84f46-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="84f46-123">パラメーター</span><span class="sxs-lookup"><span data-stu-id="84f46-123">Parameter</span></span>    | <span data-ttu-id="84f46-124">型</span><span class="sxs-lookup"><span data-stu-id="84f46-124">Type</span></span>   |<span data-ttu-id="84f46-125">説明</span><span class="sxs-lookup"><span data-stu-id="84f46-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="84f46-126">criteria</span><span class="sxs-lookup"><span data-stu-id="84f46-126">criteria</span></span>|<span data-ttu-id="84f46-127">FilterCriteria</span><span class="sxs-lookup"><span data-stu-id="84f46-127">FilterCriteria</span></span>|<span data-ttu-id="84f46-128">適用する基準。</span><span class="sxs-lookup"><span data-stu-id="84f46-128">The criteria to apply.</span></span>|

## <a name="response"></a><span data-ttu-id="84f46-129">応答</span><span class="sxs-lookup"><span data-stu-id="84f46-129">Response</span></span>

<span data-ttu-id="84f46-p103">成功した場合、このメソッドは `200, OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="84f46-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84f46-132">例</span><span class="sxs-lookup"><span data-stu-id="84f46-132">Example</span></span>
<span data-ttu-id="84f46-133">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="84f46-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="84f46-134">要求</span><span class="sxs-lookup"><span data-stu-id="84f46-134">Request</span></span>
<span data-ttu-id="84f46-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="84f46-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "filter_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/apply
Content-type: application/json
Content-length: 321

{
  "criteria": {
    "criterion1": "criterion1-value",
    "criterion2": "criterion2-value",
    "color": "color-value",
    "operator": {
    },
    "icon": {
      "set": "set-value",
      "index": 99
    },
    "dynamicCriteria": "dynamicCriteria-value",
    "values": {
    },
    "filterOn": "filterOn-value"
  }
}
```

##### <a name="response"></a><span data-ttu-id="84f46-136">応答</span><span class="sxs-lookup"><span data-stu-id="84f46-136">Response</span></span>
<span data-ttu-id="84f46-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="84f46-137">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Filter: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->