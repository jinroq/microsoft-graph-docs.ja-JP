# <a name="create-a-sharing-link-for-a-driveitem"></a><span data-ttu-id="f553b-101">DriveItem の共有リンクを作成する</span><span class="sxs-lookup"><span data-stu-id="f553b-101">Create a sharing link for a DriveItem</span></span>

<span data-ttu-id="f553b-102">**createLink** アクションを使用して、共有リンクを使って [DriveItem](../resources/driveitem.md) を共有できます。</span><span class="sxs-lookup"><span data-stu-id="f553b-102">You can use **createLink** action to share a [DriveItem](../resources/driveitem.md) via a sharing link.</span></span>

<span data-ttu-id="f553b-p101">**createLink** アクションは、呼び出し元のアプリケーションに指定されたリンクの種類が存在しない場合に、新しい共有リンクを作成します。指定された種類の共有リンクがアプリで既に存在している場合、既存の共有リンクが返されます。</span><span class="sxs-lookup"><span data-stu-id="f553b-p101">The **createLink** action will create a new sharing link if the specified link type doesn't already exist for the calling application. If a sharing link of the specified type already exists for the app, the existing sharing link will be returned.</span></span>

<span data-ttu-id="f553b-105">DriveItem リソースは、そのリソースの先祖からアクセス許可を継承します。</span><span class="sxs-lookup"><span data-stu-id="f553b-105">DriveItem resources inherit permissions from their ancestors.</span></span>

## <a name="permissions"></a><span data-ttu-id="f553b-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f553b-106">Permissions</span></span>
<span data-ttu-id="f553b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f553b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f553b-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f553b-109">Permission type</span></span>      | <span data-ttu-id="f553b-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f553b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f553b-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f553b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f553b-112">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f553b-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f553b-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f553b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f553b-114">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f553b-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="f553b-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f553b-115">Application</span></span> | <span data-ttu-id="f553b-116">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f553b-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f553b-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f553b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{item-id}/createLink
POST /me/drive/root:/{item-path}:/createLink
POST /groups/{group-id}/drive/items/{item-id}/createLink
POST /drives/{drive-id}/items/{item-id}/createLink
```

## <a name="request-body"></a><span data-ttu-id="f553b-118">要求本文</span><span class="sxs-lookup"><span data-stu-id="f553b-118">Request body</span></span>
<span data-ttu-id="f553b-p103">要求本文はアプリが検索する共有リンクの種類を定義します。要求は、次のプロパティを持つ JSON オブジェクトである必要があります。</span><span class="sxs-lookup"><span data-stu-id="f553b-p103">The body of the request defines the type of sharing link your application is looking for. The request should be a JSON object with this property.</span></span>

| <span data-ttu-id="f553b-121">名前</span><span class="sxs-lookup"><span data-stu-id="f553b-121">Name</span></span>      | <span data-ttu-id="f553b-122">型</span><span class="sxs-lookup"><span data-stu-id="f553b-122">Type</span></span>   | <span data-ttu-id="f553b-123">説明</span><span class="sxs-lookup"><span data-stu-id="f553b-123">Description</span></span>                                                                  |
|:----------|:-------|:-----------------------------------------------------------------------------|
| <span data-ttu-id="f553b-124">**type**</span><span class="sxs-lookup"><span data-stu-id="f553b-124">**type**</span></span>  | <span data-ttu-id="f553b-125">string</span><span class="sxs-lookup"><span data-stu-id="f553b-125">string</span></span> | <span data-ttu-id="f553b-p104">作成する共有リンクの種類。`view`、`edit`、または `embed` です。</span><span class="sxs-lookup"><span data-stu-id="f553b-p104">The type of sharing link to create. Either `view`, `edit`, or `embed`.</span></span>       |
| <span data-ttu-id="f553b-128">**scope**</span><span class="sxs-lookup"><span data-stu-id="f553b-128">**scope**</span></span> | <span data-ttu-id="f553b-129">string</span><span class="sxs-lookup"><span data-stu-id="f553b-129">string</span></span> | <span data-ttu-id="f553b-p105">作成するリンクのスコープ。`anonymous` または `organization` です。省略可能。</span><span class="sxs-lookup"><span data-stu-id="f553b-p105">The scope of link to create. Either `anonymous` or `organization`. Optional.</span></span> |

## <a name="link-types"></a><span data-ttu-id="f553b-133">リンクの種類</span><span class="sxs-lookup"><span data-stu-id="f553b-133">Link types</span></span>
<span data-ttu-id="f553b-134">**type** パラメーターには次の値を使用できます。</span><span class="sxs-lookup"><span data-stu-id="f553b-134">The following values are allowed for the **type** parameter.</span></span>

| <span data-ttu-id="f553b-135">種類の値</span><span class="sxs-lookup"><span data-stu-id="f553b-135">Type value</span></span> | <span data-ttu-id="f553b-136">説明</span><span class="sxs-lookup"><span data-stu-id="f553b-136">Description</span></span>                                                                                  |
|:-----------|:---------------------------------------------------------------------------------------------|
| `view`     | <span data-ttu-id="f553b-137">そのアイテムへの読み取り専用リンクを作成します。</span><span class="sxs-lookup"><span data-stu-id="f553b-137">Creates a read-only link to the item.</span></span>                                                        |
| `edit`     | <span data-ttu-id="f553b-138">そのアイテムへの読み取り/書き込みリンクを作成します。</span><span class="sxs-lookup"><span data-stu-id="f553b-138">Creates a read-write link to the item.</span></span>                                                       |
| `embed`    | <span data-ttu-id="f553b-p106">そのアイテムへの埋め込み可能なリンクを作成します。このオプションは OneDrive 個人用でのみ選択可能です。</span><span class="sxs-lookup"><span data-stu-id="f553b-p106">Creates an embeddable link to the item. This option is only available for OneDrive Personal.</span></span> |

## <a name="scope-types"></a><span data-ttu-id="f553b-141">スコープの種類</span><span class="sxs-lookup"><span data-stu-id="f553b-141">Scope types</span></span>
<span data-ttu-id="f553b-p107">**scope** パラメーターには次の値を使用できます。このパラメーターは省略可能です。**scope** パラメーターを指定しない場合、最も制限の少ないリンクが作成されます。</span><span class="sxs-lookup"><span data-stu-id="f553b-p107">The following values are allowed for the **scope** parameter. This is an optional parameter. If the **scope** parameter is not specified, the most permissive link available will be created.</span></span>

| <span data-ttu-id="f553b-145">種類の値</span><span class="sxs-lookup"><span data-stu-id="f553b-145">Type value</span></span>     | <span data-ttu-id="f553b-146">説明</span><span class="sxs-lookup"><span data-stu-id="f553b-146">Description</span></span>                                                                                                                   |
|:---------------|:------------------------------------------------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="f553b-p108">そのアイテムへの、すべてのユーザーがアクセス可能なリンクを作成します。匿名リンクはテナント管理者により無効にされることがあります。</span><span class="sxs-lookup"><span data-stu-id="f553b-p108">Creates a link to the item accessible to anyone. Anonymous links may be disabled by the tenant administrator.</span></span>                 |
| `organization` | <span data-ttu-id="f553b-p109">そのアイテムへの、組織内でアクセス可能なリンクを作成します。組織のリンク スコープは、OneDrive 個人用では使用できません。</span><span class="sxs-lookup"><span data-stu-id="f553b-p109">Creates a link to the item accessible within an organization. Organization link scope is not available for OneDrive Personal.</span></span> |

## <a name="response"></a><span data-ttu-id="f553b-151">応答</span><span class="sxs-lookup"><span data-stu-id="f553b-151">Response</span></span>

<span data-ttu-id="f553b-152">正常に実行されると、このメソッドは要求された共有リンクのアクセス許可を表す応答本文で、単一の[アクセス許可](../resources/permission.md)リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="f553b-152">If successful, this method returns a single [Permission](../resources/permission.md) resource in the response body that represents the requested sharing link permission.</span></span>

<span data-ttu-id="f553b-153">サービスはまず、現在のアクセス許可を調べ、呼び出し元アプリケーションで同じ **型**を持つアクセス許可があるかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="f553b-153">The service will first look at the current permissions and check if one already exists that has the same **type** for the calling application.</span></span>

<span data-ttu-id="f553b-154">応答は、アイテムに新しい共有リンクが作成される場合は `201 Created`、既存のリンクが返される場合は `200 OK` となります。</span><span class="sxs-lookup"><span data-stu-id="f553b-154">The response will be `201 Created` if a new sharing link is created for the item or `200 OK` if an existing link is returned.</span></span>

## <a name="example"></a><span data-ttu-id="f553b-155">例</span><span class="sxs-lookup"><span data-stu-id="f553b-155">Example</span></span>
<span data-ttu-id="f553b-156">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="f553b-156">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="f553b-157">要求</span><span class="sxs-lookup"><span data-stu-id="f553b-157">Request</span></span>
<span data-ttu-id="f553b-158">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f553b-158">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "item_createlink"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root:/{item-path}:/createLink
Content-type: application/json

{
  "type": "view",
  "scope": "anonymous"
}
```

##### <a name="response"></a><span data-ttu-id="f553b-159">応答</span><span class="sxs-lookup"><span data-stu-id="f553b-159">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "view",
    "scope": "anonymous",
    "webUrl": "https://1drv.ms/A6913278E564460AA616C71B28AD6EB6",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="creating-company-sharable-links"></a><span data-ttu-id="f553b-160">会社の共有可能リンクを作成する</span><span class="sxs-lookup"><span data-stu-id="f553b-160">Creating company sharable links</span></span>

<span data-ttu-id="f553b-p110">OneDrive for Business および SharePoint は、会社の共有可能リンクをサポートしています。これらは匿名リンクに似ていますが、所有テナントのメンバーだけが使用できる点が異なります。会社の共有可能リンクを作成するには、**scope** パラメーターで値 `organization` を指定して使用します。</span><span class="sxs-lookup"><span data-stu-id="f553b-p110">OneDrive for Business and SharePoint support company sharable links. These are similar to anonymous links, except they only work for members of the owning tenant. To create a company sharable link, use the **scope** parameter with a value of `organization`.</span></span>

## <a name="http-request"></a><span data-ttu-id="f553b-164">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f553b-164">HTTP request</span></span>

<!-- { "blockType": "request", "name": "create-link-scoped", "scopes": "files.readwrite service.sharepoint" } -->
```
POST https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "edit",
  "scope": "organization"
}
```

## <a name="http-response"></a><span data-ttu-id="f553b-165">HTTP 応答</span><span class="sxs-lookup"><span data-stu-id="f553b-165">HTTP response</span></span>

<span data-ttu-id="f553b-166">応答は、アイテムに新しい共有リンクが作成される場合は `201 Created`、既存のリンクが返される場合は `200 OK` となります。</span><span class="sxs-lookup"><span data-stu-id="f553b-166">The response will be `201 Created` if a new sharing link is created for the item or `200 OK` if an existing link is returned.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "view",
    "scope": "organization",
    "webUrl": "https://contoso-my.sharepoint.com/personal/ellen_contoso_com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="embeddable-links"></a><span data-ttu-id="f553b-167">埋め込み可能なリンク</span><span class="sxs-lookup"><span data-stu-id="f553b-167">Embeddable links</span></span>

<span data-ttu-id="f553b-p111">リンクの種類で `embed` を使用する場合、返される webUrl は `<iframe>` HTML 要素に埋め込むことができます。埋め込みリンクが作成されると、`webHtml` プロパティに `<iframe>` がコンテンツをホストするための HTML コードが含まれます。</span><span class="sxs-lookup"><span data-stu-id="f553b-p111">When using the `embed` link type, the webUrl returned can be embedded in an `<iframe>` HTML element. When an embed link is created the `webHtml` property contains the HTML code for an `<iframe>` to host the content.</span></span>

<span data-ttu-id="f553b-170">**注:**埋め込みリンクは **driveType** が `personal` である[ドライブ](../resources/drive.md)でのみ、サポートされます。</span><span class="sxs-lookup"><span data-stu-id="f553b-170">**Note:** Embed links are only supported in [Drives](../resources/drive.md) where the **driveType** is `personal`.</span></span>

## <a name="remarks"></a><span data-ttu-id="f553b-171">注釈</span><span class="sxs-lookup"><span data-stu-id="f553b-171">Remarks</span></span>

* <span data-ttu-id="f553b-172">組織に既定の有効期限ポリシーが適用されている場合を除き、このアクションを使用して作成されたリンクに期限はありません。</span><span class="sxs-lookup"><span data-stu-id="f553b-172">Links created using this action do not expire unless a default expiration policy is enforced for the organization.</span></span>
* <span data-ttu-id="f553b-173">リンクはそのアイテムの共有アクセス許可に表示され、アイテムの所有者はそれを削除できます。</span><span class="sxs-lookup"><span data-stu-id="f553b-173">Links are visible in the sharing permissions for the item and can be removed by an owner of the item.</span></span>
* <span data-ttu-id="f553b-174">リンクは、そのアイテムがチェックアウトされない限り、常にアイテムの現在のバージョンをポイントします (SharePoint の場合のみ)。</span><span class="sxs-lookup"><span data-stu-id="f553b-174">Links always point to the current version of a item unless the item is checked out (SharePoint only).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "item: createLink",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Create sharing link"
} -->
