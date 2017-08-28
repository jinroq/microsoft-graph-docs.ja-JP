# <a name="copy-a-driveitem"></a><span data-ttu-id="f7d67-101">DriveItem をコピーする</span><span class="sxs-lookup"><span data-stu-id="f7d67-101">Copy a DriveItem</span></span>

<span data-ttu-id="f7d67-102">新しい親の下の、または新しい名前を指定した [driveItem](../resources/driveitem.md) (すべての子を含む) のコピーを作成します。</span><span class="sxs-lookup"><span data-stu-id="f7d67-102">Creates a copy of a [driveItem](../resources/driveitem.md) (including any children) under a new parent or with a new name.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7d67-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f7d67-103">Permissions</span></span>
<span data-ttu-id="f7d67-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f7d67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f7d67-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f7d67-106">Permission type</span></span>      | <span data-ttu-id="f7d67-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f7d67-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7d67-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f7d67-108">Delegated (work or school account)</span></span> | <span data-ttu-id="f7d67-109">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7d67-109">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f7d67-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f7d67-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7d67-111">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7d67-111">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="f7d67-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f7d67-112">Application</span></span> | <span data-ttu-id="f7d67-113">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7d67-113">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7d67-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f7d67-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```
POST /me/drive/items/{item-id}/copy
POST /me/drive/root:/{path}:/copy
POST /groups/{group-id}/drive/items/{item-id}/copy
```

## <a name="request-body"></a><span data-ttu-id="f7d67-115">要求本文</span><span class="sxs-lookup"><span data-stu-id="f7d67-115">Request body</span></span>
<span data-ttu-id="f7d67-116">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="f7d67-116">In the request body, provide a JSON object with the following parameters.</span></span>


| <span data-ttu-id="f7d67-117">名前</span><span class="sxs-lookup"><span data-stu-id="f7d67-117">Name</span></span>            | <span data-ttu-id="f7d67-118">値</span><span class="sxs-lookup"><span data-stu-id="f7d67-118">Value</span></span>                                          | <span data-ttu-id="f7d67-119">説明</span><span class="sxs-lookup"><span data-stu-id="f7d67-119">Description</span></span>                                                                                                 |
|:----------------|:-----------------------------------------------|:------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="f7d67-120">parentReference</span><span class="sxs-lookup"><span data-stu-id="f7d67-120">parentReference</span></span> | [<span data-ttu-id="f7d67-121">ItemReference</span><span class="sxs-lookup"><span data-stu-id="f7d67-121">ItemReference</span></span>](../resources/itemreference.md) | <span data-ttu-id="f7d67-p102">省略可能。コピーが作成される親アイテムへの参照。</span><span class="sxs-lookup"><span data-stu-id="f7d67-p102">Optional. Reference to the parent item the copy will be created in.</span></span>                                         |
| <span data-ttu-id="f7d67-124">name</span><span class="sxs-lookup"><span data-stu-id="f7d67-124">name</span></span>            | <span data-ttu-id="f7d67-125">string</span><span class="sxs-lookup"><span data-stu-id="f7d67-125">string</span></span>                                         | <span data-ttu-id="f7d67-p103">省略可能。コピーの新しい名前。これを指定しない場合は、元の名前と同じ名前が使用されます。</span><span class="sxs-lookup"><span data-stu-id="f7d67-p103">Optional. The new name for the copy. If this isn't provided, the same name will be used as the original.</span></span>    |

<span data-ttu-id="f7d67-p104">**注:**_parentReference_ には `id` か `path` のいずれかを含める必要がありますが、両方を含める必要はありません。両方が含まれる場合は、それらが同じアイテムを参照する必要があります。そうでないと、エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="f7d67-p104">**Note:** The _parentReference_ should include either an `id` or `path` but not both. If both are included, they need to reference the same item or an error will occur.</span></span>

## <a name="example"></a><span data-ttu-id="f7d67-131">例</span><span class="sxs-lookup"><span data-stu-id="f7d67-131">Example</span></span>

<!-- { "blockType": "request", "name": "copy-item", "scopes": "files.readwrite" } -->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/copy
Content-Type: application/json

{
  "parentReference": {
    "path": "/drive/root:/Documents"
  },
  "name": "contoso plan.docx"
}
```

## <a name="response"></a><span data-ttu-id="f7d67-132">応答</span><span class="sxs-lookup"><span data-stu-id="f7d67-132">Response</span></span>

<span data-ttu-id="f7d67-133">要求の受け入れ時に、コピーの進行状況を監視する方法についての詳細を返します。</span><span class="sxs-lookup"><span data-stu-id="f7d67-133">Returns details about how to monitor the progress of the copy, upon accepting the request.</span></span>

<!-- { "blockType": "response" } -->
```http
HTTP/1.1 202 Accepted
```

## <a name="remarks"></a><span data-ttu-id="f7d67-134">注釈</span><span class="sxs-lookup"><span data-stu-id="f7d67-134">Remarks</span></span>

<span data-ttu-id="f7d67-p105">多くの場合、コピー操作は非同期で実行されます。API からの応答は、コピー操作が受け入れられたか、コピー先のファイル名が既に使用中のためという理由で拒否されたことのみを示します。</span><span class="sxs-lookup"><span data-stu-id="f7d67-p105">In many cases the copy action is performed asynchronously. The response from the API will only indicate that the copy operation was accepted or rejected, say due to the destination filename already being in use.</span></span>

<span data-ttu-id="f7d67-137">**注:**API は、コピーが成功したかどうかを知るためのメソッドは提供しません。</span><span class="sxs-lookup"><span data-stu-id="f7d67-137">**Note:** The API does not provide a method to know if the copy was successful.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Copy"
} -->
