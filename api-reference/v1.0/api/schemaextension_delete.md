# <a name="delete-schemaextension"></a><span data-ttu-id="3f613-101">schemaExtension を削除する</span><span class="sxs-lookup"><span data-stu-id="3f613-101">Delete schemaExtension</span></span>

<span data-ttu-id="3f613-102">[スキーマ拡張機能](../resources/schemaExtension.md)の定義を削除します。</span><span class="sxs-lookup"><span data-stu-id="3f613-102">Delete the definition of a [schema extension](../resources/schemaExtension.md).</span></span>

<span data-ttu-id="3f613-p101">スキーマ拡張機能を作成したアプリ (所有者アプリ) だけが、そのスキーマ拡張機能が **InDevelopment** 状態の場合に限り、スキーマ拡張機能の定義を削除できます。スキーマ拡張機能の定義を削除しても、その定義に基づいてリソース インスタンスに追加されたカスタム データへのアクセスには影響しません。</span><span class="sxs-lookup"><span data-stu-id="3f613-p101">Only the app that created the schema extension (owner app) can delete the schema extension definition, and only when the extension is in the **InDevelopment** state. Deleting a schema extension definition does not affect accessing custom data that has been added to resource instances based on that definition.</span></span>


## <a name="permissions"></a><span data-ttu-id="3f613-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3f613-105">Permissions</span></span>
<span data-ttu-id="3f613-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3f613-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="3f613-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3f613-108">Permission type</span></span>      | <span data-ttu-id="3f613-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3f613-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3f613-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3f613-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3f613-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3f613-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3f613-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3f613-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f613-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3f613-113">Not supported.</span></span>    |
|<span data-ttu-id="3f613-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3f613-114">Application</span></span> | <span data-ttu-id="3f613-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3f613-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3f613-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3f613-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /schemaExtensions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3f613-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3f613-117">Request headers</span></span>
| <span data-ttu-id="3f613-118">名前</span><span class="sxs-lookup"><span data-stu-id="3f613-118">Name</span></span>      |<span data-ttu-id="3f613-119">説明</span><span class="sxs-lookup"><span data-stu-id="3f613-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3f613-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f613-120">Authorization</span></span>  | <span data-ttu-id="3f613-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3f613-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3f613-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="3f613-123">Request body</span></span>
<span data-ttu-id="3f613-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3f613-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3f613-125">応答</span><span class="sxs-lookup"><span data-stu-id="3f613-125">Response</span></span>

<span data-ttu-id="3f613-p104">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="3f613-p104">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f613-128">例</span><span class="sxs-lookup"><span data-stu-id="3f613-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3f613-129">要求</span><span class="sxs-lookup"><span data-stu-id="3f613-129">Request</span></span>
<span data-ttu-id="3f613-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3f613-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_schemaextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/schemaExtensions/{id}
```
##### <a name="response"></a><span data-ttu-id="3f613-131">応答</span><span class="sxs-lookup"><span data-stu-id="3f613-131">Response</span></span>
<span data-ttu-id="3f613-132">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="3f613-132">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="3f613-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="3f613-133">See also</span></span>

- [<span data-ttu-id="3f613-134">拡張機能を使用したリソースへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="3f613-134">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="3f613-135">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="3f613-135">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->