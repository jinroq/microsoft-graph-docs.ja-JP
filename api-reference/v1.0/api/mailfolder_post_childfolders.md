# <a name="create-mailfolder"></a><span data-ttu-id="b8a3b-101">MailFolder を作成する</span><span class="sxs-lookup"><span data-stu-id="b8a3b-101">Create MailFolder</span></span>

<span data-ttu-id="b8a3b-102">この API を使用して、新しい子 mailFolder を作成します。</span><span class="sxs-lookup"><span data-stu-id="b8a3b-102">Use this API to create a new child mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8a3b-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b8a3b-103">Permissions</span></span>
<span data-ttu-id="b8a3b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b8a3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b8a3b-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b8a3b-106">Permission type</span></span>      | <span data-ttu-id="b8a3b-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b8a3b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8a3b-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b8a3b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b8a3b-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8a3b-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b8a3b-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b8a3b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8a3b-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8a3b-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b8a3b-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b8a3b-112">Application</span></span> | <span data-ttu-id="b8a3b-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8a3b-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8a3b-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b8a3b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="b8a3b-115">クエリの URL 内の親フォルダーをフォルダー ID、または `Inbox`、`Drafts`、`SentItems`、や `DeletedItems` のよく知られているフォルダー名として指定します。</span><span class="sxs-lookup"><span data-stu-id="b8a3b-115">Specify the parent folder in the query URL as a folder ID, or the `Inbox`, `Drafts`, `SentItems`, or `DeletedItems` well-known folder name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b8a3b-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b8a3b-116">Request headers</span></span>
| <span data-ttu-id="b8a3b-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b8a3b-117">Header</span></span>       | <span data-ttu-id="b8a3b-118">値</span><span class="sxs-lookup"><span data-stu-id="b8a3b-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b8a3b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8a3b-119">Authorization</span></span>  | <span data-ttu-id="b8a3b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b8a3b-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b8a3b-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b8a3b-122">Content-Type</span></span>  | <span data-ttu-id="b8a3b-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="b8a3b-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b8a3b-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="b8a3b-125">Request body</span></span>
<span data-ttu-id="b8a3b-p104">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。[MailFolder](../resources/mailfolder.md) オブジェクトに対して書き込み可能なプロパティは **displayName** のみです。</span><span class="sxs-lookup"><span data-stu-id="b8a3b-p104">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="b8a3b-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="b8a3b-128">Parameter</span></span>    | <span data-ttu-id="b8a3b-129">型</span><span class="sxs-lookup"><span data-stu-id="b8a3b-129">Type</span></span>   |<span data-ttu-id="b8a3b-130">説明</span><span class="sxs-lookup"><span data-stu-id="b8a3b-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8a3b-131">displayName</span><span class="sxs-lookup"><span data-stu-id="b8a3b-131">displayName</span></span>|<span data-ttu-id="b8a3b-132">String</span><span class="sxs-lookup"><span data-stu-id="b8a3b-132">String</span></span>|<span data-ttu-id="b8a3b-133">新しいフォルダーの表示名です。</span><span class="sxs-lookup"><span data-stu-id="b8a3b-133">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="b8a3b-134">応答</span><span class="sxs-lookup"><span data-stu-id="b8a3b-134">Response</span></span>

<span data-ttu-id="b8a3b-135">成功した場合、このメソッドは `201, Created` 応答コードと、応答本文で [MailFolder](../resources/mailfolder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b8a3b-135">If successful, this method returns `201, Created` response code and [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8a3b-136">例</span><span class="sxs-lookup"><span data-stu-id="b8a3b-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b8a3b-137">要求</span><span class="sxs-lookup"><span data-stu-id="b8a3b-137">Request</span></span>
<span data-ttu-id="b8a3b-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b8a3b-138">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="b8a3b-139">応答</span><span class="sxs-lookup"><span data-stu-id="b8a3b-139">Response</span></span>
<span data-ttu-id="b8a3b-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b8a3b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
