# <a name="list-recent-files"></a><span data-ttu-id="db5ab-101">最近使用したファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="db5ab-101">List recent files</span></span>

<span data-ttu-id="db5ab-p101">サインインしたユーザーによって最近使用されたアイテムのセットを一覧表示します。このコレクションには、ユーザーのドライブにあるアイテムと、他のドライブとの間でアクセス可能なアイテムが含まれています。</span><span class="sxs-lookup"><span data-stu-id="db5ab-p101">List a set of items that have been recently used by the signed in user. This collection includes items that are in the user's drive as well as items they have access to from other drives.</span></span>

## <a name="permissions"></a><span data-ttu-id="db5ab-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="db5ab-104">Permissions</span></span>
<span data-ttu-id="db5ab-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="db5ab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="db5ab-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="db5ab-107">Permission type</span></span>      | <span data-ttu-id="db5ab-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="db5ab-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db5ab-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="db5ab-109">Delegated (work or school account)</span></span> | <span data-ttu-id="db5ab-110">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db5ab-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="db5ab-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="db5ab-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db5ab-112">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db5ab-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="db5ab-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="db5ab-113">Application</span></span> | <span data-ttu-id="db5ab-114">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db5ab-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db5ab-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="db5ab-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```
GET /me/drive/recent
```

## <a name="request-body"></a><span data-ttu-id="db5ab-116">要求本文</span><span class="sxs-lookup"><span data-stu-id="db5ab-116">Request body</span></span>
<span data-ttu-id="db5ab-117">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="db5ab-117">Do not supply a request body for this method.</span></span>

## <a name="example"></a><span data-ttu-id="db5ab-118">例</span><span class="sxs-lookup"><span data-stu-id="db5ab-118">Example</span></span>

<!-- { "blockType": "request", "name": "drive-recent", "scopes": "files.read" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/recent
```

## <a name="response"></a><span data-ttu-id="db5ab-119">応答</span><span class="sxs-lookup"><span data-stu-id="db5ab-119">Response</span></span>

<span data-ttu-id="db5ab-p103">これは、ドライブの所有者が最近アクセスしたアイテムの [DriveItem](../resources/driveitem.md) リソースのコレクションを返します。ユーザーのドライブ以外のアイテムには、共有アイテムにアクセスするための情報を提供する [RemoteItem](../resources/remoteitem.md) ファセットが含まれます。</span><span class="sxs-lookup"><span data-stu-id="db5ab-p103">This returns a collection of [DriveItem](../resources/driveitem.md) resources for items which the owner of the drive has recently accessed. Items outside of the user's drive will include the [RemoteItem](../resources/remoteitem.md) facet, which provides information to access the shared item.</span></span>


<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "isCollection": true, "truncated": true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1312abc!1231",
      "remoteItem":
      {
        "id": "1991210caf!192",
        "name": "March Proposal.docx",
        "file": { },
        "size": 19121,
        "parentReference": {
          "driveId": "1991210caf",
          "id": "1991210caf!104"
        }
      }
    },
    {
      "id": "1312def!9943",
      "name": "Vacation.jpg",
      "file": { },
      "size": 37810,
      "parentReference": {
        "driveId": "1312def",
        "id": "1312def!123"
      }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="db5ab-122">注釈</span><span class="sxs-lookup"><span data-stu-id="db5ab-122">Remarks</span></span>

<span data-ttu-id="db5ab-p104">**recent** アクションから返された DriveItems の中には、それらが異なるドライブからのアイテムであることを示す **remoteItem** ファセットが含まれるものがあります。元の DriveItem オブジェクトにアクセスするには、**remoteItem** で提供された情報を使用して、以下に示す書式で要求を作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="db5ab-p104">Some driveItems returned from the **recent** action will include the **remoteItem** facet which indicates they are items from another drive. To access the original driveItem object, you will need to make a request using the information provided in **remoteItem** in the following format:</span></span>

<!-- {"blockType": "ignored"} -->
```http
GET https://graph.microsoft.com/v1.0/drives/{remoteItem.driveId}/items/{remoteItem.id}
```

<!-- {
  "type": "#page.annotation",
  "description": "Retrieve a list of files shared with the signed-in user.",
  "keywords": "sharedWithMe onedrive shared files",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Shared with me"
} -->
