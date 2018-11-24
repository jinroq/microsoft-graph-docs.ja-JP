# <a name="delete-outlook-category"></a><span data-ttu-id="02a5e-101">Outlook カテゴリを削除する</span><span class="sxs-lookup"><span data-stu-id="02a5e-101">Delete Outlook category</span></span>


<span data-ttu-id="02a5e-102">指定した [outlookCategory](../resources/outlookCategory.md) オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="02a5e-102">Delete the specified [outlookCategory](../resources/outlookCategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="02a5e-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="02a5e-103">Permissions</span></span>
<span data-ttu-id="02a5e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="02a5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="02a5e-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="02a5e-106">Permission type</span></span>      | <span data-ttu-id="02a5e-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="02a5e-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02a5e-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="02a5e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="02a5e-109">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="02a5e-109">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="02a5e-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="02a5e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02a5e-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="02a5e-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="02a5e-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="02a5e-112">Application</span></span> | <span data-ttu-id="02a5e-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="02a5e-113">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="02a5e-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="02a5e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/masterCategories/{id}
DELETE /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="02a5e-115">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="02a5e-115">Optional query parameters</span></span>
<span data-ttu-id="02a5e-116">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="02a5e-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="02a5e-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="02a5e-117">Request headers</span></span>
| <span data-ttu-id="02a5e-118">名前</span><span class="sxs-lookup"><span data-stu-id="02a5e-118">Name</span></span>      |<span data-ttu-id="02a5e-119">説明</span><span class="sxs-lookup"><span data-stu-id="02a5e-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="02a5e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="02a5e-120">Authorization</span></span>  | <span data-ttu-id="02a5e-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="02a5e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="02a5e-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="02a5e-123">Request body</span></span>
<span data-ttu-id="02a5e-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="02a5e-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02a5e-125">応答</span><span class="sxs-lookup"><span data-stu-id="02a5e-125">Response</span></span>

<span data-ttu-id="02a5e-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="02a5e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02a5e-128">例</span><span class="sxs-lookup"><span data-stu-id="02a5e-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="02a5e-129">要求</span><span class="sxs-lookup"><span data-stu-id="02a5e-129">Request</span></span>
<span data-ttu-id="02a5e-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="02a5e-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["4b1c2495-54c9-4a5e-90a2-0ab0b31987d8"],
  "name": "delete_outlookcategory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/outlook/masterCategories/4b1c2495-54c9-4a5e-90a2-0ab0b31987d8
```
##### <a name="response"></a><span data-ttu-id="02a5e-131">応答</span><span class="sxs-lookup"><span data-stu-id="02a5e-131">Response</span></span>
<span data-ttu-id="02a5e-132">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="02a5e-132">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "name": "delete_outlookcategory",
  "isEmpty": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->