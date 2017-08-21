# <a name="delete-schemaextension"></a><span data-ttu-id="430f0-101">schemaExtension を削除する</span><span class="sxs-lookup"><span data-stu-id="430f0-101">Delete schemaExtension</span></span>

<span data-ttu-id="430f0-102">[スキーマ拡張機能](../resources/schemaExtension.md)の定義を削除します。</span><span class="sxs-lookup"><span data-stu-id="430f0-102">Delete the definition of a [schema extension](../resources/schemaExtension.md).</span></span>

<span data-ttu-id="430f0-p101">スキーマ拡張機能を作成したアプリ (所有者アプリ) だけが、そのスキーマ拡張機能が **InDevelopment** 状態の場合に限り、スキーマ拡張機能の定義を削除できます。スキーマ拡張機能の定義を削除しても、その定義に基づいてリソース インスタンスに追加されたカスタム データへのアクセスには影響しません。</span><span class="sxs-lookup"><span data-stu-id="430f0-p101">Only the app that created the schema extension (owner app) can delete the schema extension definition, and only when the extension is in the **InDevelopment** state. Deleting a schema extension definition does not affect accessing custom data that has been added to resource instances based on that definition.</span></span>


## <a name="prerequisites"></a><span data-ttu-id="430f0-105">前提条件</span><span class="sxs-lookup"><span data-stu-id="430f0-105">Prerequisites</span></span>
<span data-ttu-id="430f0-106">この API を実行するには、以下の**スコープ**が必要です。*Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="430f0-106">The following **scope** is required to execute this API: *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="430f0-107">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="430f0-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /schemaExtensions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="430f0-108">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="430f0-108">Request headers</span></span>
| <span data-ttu-id="430f0-109">名前</span><span class="sxs-lookup"><span data-stu-id="430f0-109">Name</span></span>      |<span data-ttu-id="430f0-110">説明</span><span class="sxs-lookup"><span data-stu-id="430f0-110">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="430f0-111">Authorization</span><span class="sxs-lookup"><span data-stu-id="430f0-111">Authorization</span></span>  | <span data-ttu-id="430f0-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="430f0-p102">Bearer {token}. Required.</span></span> |
 

## <a name="request-body"></a><span data-ttu-id="430f0-114">要求本文</span><span class="sxs-lookup"><span data-stu-id="430f0-114">Request body</span></span>
<span data-ttu-id="430f0-115">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="430f0-115">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="430f0-116">応答</span><span class="sxs-lookup"><span data-stu-id="430f0-116">Response</span></span>

<span data-ttu-id="430f0-p103">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="430f0-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="430f0-119">例</span><span class="sxs-lookup"><span data-stu-id="430f0-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="430f0-120">要求</span><span class="sxs-lookup"><span data-stu-id="430f0-120">Request</span></span>
<span data-ttu-id="430f0-121">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="430f0-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_schemaextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/schemaExtensions/{id}
```
##### <a name="response"></a><span data-ttu-id="430f0-122">応答</span><span class="sxs-lookup"><span data-stu-id="430f0-122">Response</span></span>
<span data-ttu-id="430f0-123">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="430f0-123">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="430f0-124">関連項目</span><span class="sxs-lookup"><span data-stu-id="430f0-124">See also</span></span>

- [<span data-ttu-id="430f0-125">拡張機能を使用したリソースへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="430f0-125">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="430f0-126">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="430f0-126">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->