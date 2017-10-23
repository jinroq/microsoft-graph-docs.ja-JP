# <a name="tablesort-clear"></a><span data-ttu-id="2421a-101">TableSort: clear　</span><span class="sxs-lookup"><span data-stu-id="2421a-101">TableSort: clear</span></span>

<span data-ttu-id="2421a-p101">テーブルに現在設定されている並べ替えをクリアします。これにより表の順序が変更されることはありませんが、ヘッダーのボタンの状態がクリアされます。</span><span class="sxs-lookup"><span data-stu-id="2421a-p101">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>
## <a name="permissions"></a><span data-ttu-id="2421a-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2421a-104">Permissions</span></span>
<span data-ttu-id="2421a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2421a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2421a-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2421a-107">Permission type</span></span>      | <span data-ttu-id="2421a-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2421a-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2421a-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2421a-109">Delegated (work or school account)</span></span> | <span data-ttu-id="2421a-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2421a-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2421a-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2421a-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2421a-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2421a-112">Not supported.</span></span>    |
|<span data-ttu-id="2421a-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2421a-113">Application</span></span> | <span data-ttu-id="2421a-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2421a-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2421a-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2421a-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/clear

```
## <a name="request-headers"></a><span data-ttu-id="2421a-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2421a-116">Request headers</span></span>
| <span data-ttu-id="2421a-117">名前</span><span class="sxs-lookup"><span data-stu-id="2421a-117">Name</span></span>       | <span data-ttu-id="2421a-118">説明</span><span class="sxs-lookup"><span data-stu-id="2421a-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2421a-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="2421a-119">Authorization</span></span>  | <span data-ttu-id="2421a-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2421a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2421a-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="2421a-122">Request body</span></span>

## <a name="response"></a><span data-ttu-id="2421a-123">応答</span><span class="sxs-lookup"><span data-stu-id="2421a-123">Response</span></span>

<span data-ttu-id="2421a-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="2421a-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2421a-126">例</span><span class="sxs-lookup"><span data-stu-id="2421a-126">Example</span></span>
<span data-ttu-id="2421a-127">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="2421a-127">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2421a-128">要求</span><span class="sxs-lookup"><span data-stu-id="2421a-128">Request</span></span>
<span data-ttu-id="2421a-129">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2421a-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/clear
```

##### <a name="response"></a><span data-ttu-id="2421a-130">応答</span><span class="sxs-lookup"><span data-stu-id="2421a-130">Response</span></span>
<span data-ttu-id="2421a-131">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="2421a-131">Here is an example of the response.</span></span> 
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
  "description": "TableSort: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->