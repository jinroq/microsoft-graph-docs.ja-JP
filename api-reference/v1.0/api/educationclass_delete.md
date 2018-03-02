# <a name="delete-educationclass"></a><span data-ttu-id="adf4f-101">educationClass を削除する</span><span class="sxs-lookup"><span data-stu-id="adf4f-101">Delete educationClass</span></span>

<span data-ttu-id="adf4f-102">クラスを削除します。</span><span class="sxs-lookup"><span data-stu-id="adf4f-102">Delete a class notebook</span></span> <span data-ttu-id="adf4f-103">クラスもユニバーサル グループなので、クラスを削除するとグループも削除されます。</span><span class="sxs-lookup"><span data-stu-id="adf4f-103">Because a class is also a universal group, deleting a class deletes the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="adf4f-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="adf4f-104">Permissions</span></span>
<span data-ttu-id="adf4f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="adf4f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="adf4f-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="adf4f-107">Permission type</span></span>      | <span data-ttu-id="adf4f-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="adf4f-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="adf4f-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="adf4f-109">Delegated (work or school account)</span></span> |  <span data-ttu-id="adf4f-110">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="adf4f-110">Not supported.</span></span>  |
|<span data-ttu-id="adf4f-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="adf4f-111">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="adf4f-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="adf4f-112">Not supported.</span></span>  |
|<span data-ttu-id="adf4f-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="adf4f-113">Application</span></span> | <span data-ttu-id="adf4f-114">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adf4f-114">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="adf4f-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="adf4f-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}

```
## <a name="request-headers"></a><span data-ttu-id="adf4f-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="adf4f-116">Request headers</span></span>
| <span data-ttu-id="adf4f-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="adf4f-117">Header</span></span>       | <span data-ttu-id="adf4f-118">値</span><span class="sxs-lookup"><span data-stu-id="adf4f-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="adf4f-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="adf4f-119">Authorization</span></span>  | <span data-ttu-id="adf4f-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="adf4f-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="adf4f-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="adf4f-122">Request body</span></span>
<span data-ttu-id="adf4f-123">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="adf4f-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="adf4f-124">応答</span><span class="sxs-lookup"><span data-stu-id="adf4f-124">Response</span></span>
<span data-ttu-id="adf4f-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="adf4f-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="adf4f-127">例</span><span class="sxs-lookup"><span data-stu-id="adf4f-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="adf4f-128">要求</span><span class="sxs-lookup"><span data-stu-id="adf4f-128">Request</span></span>
<span data-ttu-id="adf4f-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="adf4f-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationclass"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/11022
```
##### <a name="response"></a><span data-ttu-id="adf4f-130">応答</span><span class="sxs-lookup"><span data-stu-id="adf4f-130">Response</span></span>
<span data-ttu-id="adf4f-131">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="adf4f-131">The following is an example of the response.</span></span> 

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
  "description": "Delete educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->