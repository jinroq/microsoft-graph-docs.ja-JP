# <a name="upload-or-replace-the-contents-of-a-driveitem"></a><span data-ttu-id="16244-101">driveItem の内容をアップロードまたは置換する</span><span class="sxs-lookup"><span data-stu-id="16244-101">Upload or replace the contents of a driveItem</span></span>

<span data-ttu-id="16244-p101">簡単なアップロード API を使用すると、新しいファイルの内容を提供したり、単一の API 呼び出しで既存のファイルの内容を更新したりすることができます。このメソッドは、サイズが 4MB までのファイルのみをサポートしています。</span><span class="sxs-lookup"><span data-stu-id="16244-p101">The simple upload API allows you to provide the contents of a new file or update the contents of an existing file in a single API call. This method only supports files up to 4MB in size.</span></span>

<span data-ttu-id="16244-104">大きなファイルをアップロードする場合は、「[アップロード セッションを使ってサイズの大きなファイルをアップロードする](item_createuploadsession.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="16244-104">To upload large files see [Upload large files with an upload session](item_createuploadsession.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="16244-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="16244-105">Permissions</span></span>
<span data-ttu-id="16244-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="16244-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="16244-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="16244-108">Permission type</span></span>      | <span data-ttu-id="16244-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="16244-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16244-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="16244-110">Delegated (work or school account)</span></span> | <span data-ttu-id="16244-111">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16244-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="16244-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="16244-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16244-113">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16244-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="16244-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="16244-114">Application</span></span> | <span data-ttu-id="16244-115">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16244-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="16244-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="16244-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /me/drive/items/{parent-id}:/{filename}:/content
PUT /me/drive/root:/{parent-path}/{filename}:/content
PUT /me/drive/items/{parent-id}/children/{filename}/content
PUT /groups/{id}/drive/items/{parent-id}/children/{filename}/content
```

## <a name="request-body"></a><span data-ttu-id="16244-117">要求本文</span><span class="sxs-lookup"><span data-stu-id="16244-117">Request body</span></span>
<span data-ttu-id="16244-118">要求の本文の内容は、アップロードするファイルのバイナリ ストリームである必要があります。</span><span class="sxs-lookup"><span data-stu-id="16244-118">The contents of the request body should be the binary stream of the file to be uploaded.</span></span>

## <a name="response"></a><span data-ttu-id="16244-119">応答</span><span class="sxs-lookup"><span data-stu-id="16244-119">Response</span></span>

<span data-ttu-id="16244-120">成功した場合、このメソッドは新しく作成されたファイルの応答本文で [driveItem](../resources/driveitem.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="16244-120">If successful, this method returns a [driveItem](../resources/driveitem.md) object in the response body for the newly created file.</span></span>

## <a name="example"></a><span data-ttu-id="16244-121">例</span><span class="sxs-lookup"><span data-stu-id="16244-121">Example</span></span>
<span data-ttu-id="16244-122">次の例は、サインインしているユーザーの OneDrive へのパスを使用してファイルをアップロードします。</span><span class="sxs-lookup"><span data-stu-id="16244-122">This example uploads a file by path to the signed-in user's OneDrive.</span></span>

<!-- {
  "blockType": "request",
  "name": "upload_item"
}-->
```http
PUT /me/drive/root:/{item-path}:/content
Content-type: text/plain

The contents of the file goes here.
```

##### <a name="response"></a><span data-ttu-id="16244-123">応答</span><span class="sxs-lookup"><span data-stu-id="16244-123">Response</span></span>

<span data-ttu-id="16244-124">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="16244-124">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "0123456789abc",
  "name": "myfile.jpg",
  "size": 10191,
  "file": { }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Upload item",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
