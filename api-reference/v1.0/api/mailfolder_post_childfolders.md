# <a name="create-mailfolder"></a><span data-ttu-id="ca807-101">MailFolder を作成する</span><span class="sxs-lookup"><span data-stu-id="ca807-101">Create MailFolder</span></span>

<span data-ttu-id="ca807-102">この API を使用して、新しい子 mailFolder を作成します。</span><span class="sxs-lookup"><span data-stu-id="ca807-102">Use this API to create a new child mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="ca807-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ca807-103">Permissions</span></span>

<span data-ttu-id="ca807-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ca807-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="ca807-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ca807-106">Permission type</span></span> | <span data-ttu-id="ca807-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ca807-107">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="ca807-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ca807-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ca807-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca807-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ca807-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ca807-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca807-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca807-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ca807-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ca807-112">Application</span></span> | <span data-ttu-id="ca807-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca807-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca807-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ca807-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="ca807-115">クエリの URL の親フォルダーを、フォルダー ID またはよく知られているフォルダー名として指定します。</span><span class="sxs-lookup"><span data-stu-id="ca807-115">Specify the parent folder in the query URL as a folder ID, or the , , , or  well-known folder name.</span></span> <span data-ttu-id="ca807-116">サポートされている既知のフォルダー名の一覧については、「[mailFolder リソースの種類](../resources/mailfolder.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ca807-116">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ca807-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ca807-117">Request headers</span></span>

| <span data-ttu-id="ca807-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ca807-118">Header</span></span> | <span data-ttu-id="ca807-119">値</span><span class="sxs-lookup"><span data-stu-id="ca807-119">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="ca807-120">承認</span><span class="sxs-lookup"><span data-stu-id="ca807-120">Authorization</span></span> | <span data-ttu-id="ca807-121">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="ca807-121"></span></span> <span data-ttu-id="ca807-122">必須。</span><span class="sxs-lookup"><span data-stu-id="ca807-122">Required.</span></span> |
| <span data-ttu-id="ca807-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ca807-123">Content-Type</span></span> | <span data-ttu-id="ca807-124">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="ca807-124"></span></span> <span data-ttu-id="ca807-125">必須。</span><span class="sxs-lookup"><span data-stu-id="ca807-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ca807-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ca807-126">Request body</span></span>

<span data-ttu-id="ca807-127">要求本文で、次のパラメータを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="ca807-127">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="ca807-128">**displayName** は、 [mailFolder](../resources/mailfolder.md) オブジェクトに唯一書き込み可能なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="ca807-128">**displayName** is the only writable property for a [mailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="ca807-129">パラメータ</span><span class="sxs-lookup"><span data-stu-id="ca807-129">Parameter</span></span> | <span data-ttu-id="ca807-130">型</span><span class="sxs-lookup"><span data-stu-id="ca807-130">Type</span></span> | <span data-ttu-id="ca807-131">説明</span><span class="sxs-lookup"><span data-stu-id="ca807-131">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="ca807-132">displayName</span><span class="sxs-lookup"><span data-stu-id="ca807-132">displayName</span></span>|<span data-ttu-id="ca807-133">文字列</span><span class="sxs-lookup"><span data-stu-id="ca807-133">String</span></span>|<span data-ttu-id="ca807-134">新しいフォルダーの表示名です。</span><span class="sxs-lookup"><span data-stu-id="ca807-134">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="ca807-135">応答</span><span class="sxs-lookup"><span data-stu-id="ca807-135">Response</span></span>

<span data-ttu-id="ca807-136">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文の [mailFolder](../resources/mailfolder.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="ca807-136">If successful, this method returns a `201 Created` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca807-137">例</span><span class="sxs-lookup"><span data-stu-id="ca807-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ca807-138">要求</span><span class="sxs-lookup"><span data-stu-id="ca807-138">Request</span></span>

<span data-ttu-id="ca807-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ca807-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_mailfolder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```

##### <a name="response"></a><span data-ttu-id="ca807-140">応答</span><span class="sxs-lookup"><span data-stu-id="ca807-140">Response</span></span>
<span data-ttu-id="ca807-141">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="ca807-141">Here is an example of the response.</span></span>

> <span data-ttu-id="ca807-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="ca807-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create MailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
