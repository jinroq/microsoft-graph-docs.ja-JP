# <a name="list-items-shared-with-the-signed-in-user"></a><span data-ttu-id="2cf4a-101">サインインしているユーザーと共有しているアイテムを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="2cf4a-101">List items shared with the signed-in user</span></span>

<span data-ttu-id="2cf4a-102">[ドライブ](../resources/drive.md) の所有者と共有されている、[DriveItem](../resources/driveitem.md) リソースのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="2cf4a-102">Retrieve a collection of [DriveItem](../resources/driveitem.md) resources that have been shared with the owner of the [Drive](../resources/drive.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2cf4a-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2cf4a-103">Permissions</span></span>
<span data-ttu-id="2cf4a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2cf4a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2cf4a-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2cf4a-106">Permission type</span></span>      | <span data-ttu-id="2cf4a-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2cf4a-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2cf4a-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2cf4a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="2cf4a-109">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cf4a-109">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="2cf4a-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2cf4a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2cf4a-111">Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cf4a-111">Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="2cf4a-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2cf4a-112">Application</span></span> | <span data-ttu-id="2cf4a-113">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cf4a-113">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

<span data-ttu-id="2cf4a-114">さらに、**すべて**のアクセス許可のうちの一つがなければ、この API から返された共有項目はアクセスできません。</span><span class="sxs-lookup"><span data-stu-id="2cf4a-114">Additionally, without one of the  **All** scopes, shared items returned from this API will not be accessible.</span></span>

## <a name="http-request"></a><span data-ttu-id="2cf4a-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2cf4a-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```
GET /me/drive/sharedWithMe
```

## <a name="request-body"></a><span data-ttu-id="2cf4a-116">要求本文</span><span class="sxs-lookup"><span data-stu-id="2cf4a-116">Request body</span></span>
<span data-ttu-id="2cf4a-117">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2cf4a-117">Do not supply a request body for this method.</span></span>

## <a name="example"></a><span data-ttu-id="2cf4a-118">例</span><span class="sxs-lookup"><span data-stu-id="2cf4a-118">Example</span></span>

<!-- { "blockType": "request", "name": "drive-sharedwithme", "scopes": "files.read" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/sharedWithMe
```

## <a name="response"></a><span data-ttu-id="2cf4a-119">応答</span><span class="sxs-lookup"><span data-stu-id="2cf4a-119">Response</span></span>

<span data-ttu-id="2cf4a-p102">これは、ドライブの所有者を共有している DriveItem リソースを含む、[DriveItem](../resources/driveitem.md) リソースのコレクションを返します。この例では、ドライブはユーザーの既定のドライブです。そのため、これはサインインしているユーザーと共有しているアイテムを返します。</span><span class="sxs-lookup"><span data-stu-id="2cf4a-p102">This returns a collection of [DriveItem](../resources/driveitem.md) resources which contain the DriveItem resources shared with the owner of the drive. In this example, since the drive is the user's default drive, this returns items shared with the signed in user.</span></span>


<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "isCollection": true, "truncated": true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1312abc",
      "remoteItem": {
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
      "id": "1312def",
      "remoteItem": {
        "id": "1991210caf!1991",
        "name": "Team Roster.xlsx",
        "file": { },
        "size": 37619,
        "parentReference": {
          "driveId": "1991210caf",
          "id": "1991210caf!104"
        }
      }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="2cf4a-122">注釈</span><span class="sxs-lookup"><span data-stu-id="2cf4a-122">Remarks</span></span>

<span data-ttu-id="2cf4a-p103">**sharedWithMe** アクションから返された DriveItems には、それらが異なるドライブからのアイテムであることを示す [**remoteItem**](../resources/remoteitem.md) ファセットが必ず含まれます。共有された DriveItem リソースにアクセスするには、**remoteItem** で提供された情報を使用して、以下に示す書式で要求を作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2cf4a-p103">DriveItems returned from the **sharedWithMe** action will always include the [**remoteItem**](../resources/remoteitem.md) facet which indicates they are items from a different drive. To access the shared DriveItem resource, you will need to make a request using the information provided in **remoteItem** in the following format:</span></span>

<!-- {"blockType": "ignored"} -->
```http
GET https://graph.microsoft.com/v1.0/drives/{remoteItem.parentReference.driveId}/items/{remoteItem.id}
```

<!-- {
  "type": "#page.annotation",
  "description": "Retrieve a list of files shared with the signed-in user.",
  "keywords": "sharedWithMe onedrive shared files",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Shared with me"
} -->
