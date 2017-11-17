# <a name="working-with-files-in-microsoft-graph"></a><span data-ttu-id="b23d2-101">Microsoft Graph でのファイルの作業</span><span class="sxs-lookup"><span data-stu-id="b23d2-101">Working with files in Microsoft Graph</span></span>

<span data-ttu-id="b23d2-p101">Microsoft Graph を使用して、OneDrive、OneDrive for Business、および SharePoint のドキュメント ライブラリに配置されるファイルに接続するアプリケーションを作成できます。Microsoft Graph を使用することで、ユーザーのドキュメントを単に格納することから、複雑なファイル共有の複雑なシナリオまで、Office 365 に格納されるファイルに関するさまざまなエクスペリエンスを構築できます。</span><span class="sxs-lookup"><span data-stu-id="b23d2-p101">You can use Microsoft Graph to create an app that connects with files across OneDrive, OneDrive for Business, and SharePoint document libraries. With Microsoft Graph, you can build a variety of experiences with files stored in Office 365, from simply storing user documents to complex file sharing scenarios.</span></span>

<span data-ttu-id="b23d2-104">Microsoft Graph では、ファイルを操作するための 2 種類のリソースが公開されています。</span><span class="sxs-lookup"><span data-stu-id="b23d2-104">Microsoft Graph exposes two resource types for working with files:</span></span>

* <span data-ttu-id="b23d2-105">[Drive](drive.md) - ドキュメント ライブラリやユーザーの OneDrive など、ファイルの論理コンテナーを表します。</span><span class="sxs-lookup"><span data-stu-id="b23d2-105">[Drive](drive.md) - Represents a logical container of files, like a document library or a user's OneDrive.</span></span>
* <span data-ttu-id="b23d2-106">[DriveItem](driveitem.md) -ドキュメント、写真、ビデオ、フォルダーなど、ドライブ内のアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="b23d2-106">[DriveItem](driveitem.md) - Represents an item within a drive, like a document, photo, video, or folder.</span></span>

<span data-ttu-id="b23d2-107">ファイル間での相互作用のほとんどは、**DriveItem** リソース間での相互作用によって発生します。</span><span class="sxs-lookup"><span data-stu-id="b23d2-107">Most of the interaction with files occurs through interaction with **DriveItem** resources. The following is an example of a DriveItem resource:</span></span> <span data-ttu-id="b23d2-108">次に、DriveItem リソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="b23d2-108">The following is an example of a driveItem resource.</span></span>

```json
{
  "@content.downloadUrl":"http://public-sn3302.files.1drv.com/y2pcT7OaUEExF7EHOlpTjCE55mIUoiX7H3sx1ff6I-nP35XUTBqZlnkh9FJhWb_pf9sZ7LEpEchvDznIbQig0hWBeidpwFkOqSKCwQylisarN6T0ecAeMvantizBUzM2PA1",
  "createdDateTime": "2016-09-16T03:37:04.72Z",
  "cTag": "aYzpENDY0OEYwNkM5MUQ5RDNEITU0OTI3LjI1Ng",
  "eTag": "aRDQ2NDhGMDZDOTFEOUQzRCE1NDkyNy4w",
  "id":"D4648F06C91D9D3D!54927",
  "lastModifiedBy": {
    "user": {
      "displayName": "Daron Spektor",
      "id": "d4648f06c91d9d3d"
    }
  },
  "name":"BritishShorthair.jpg",
  "size":35212,
  "image":{
    "height":398,
    "width":273
  },
  "file": {
    "hashes":{
      "sha1Hash":"wmgPQ6jrSeMX7JP1XmstQEGM2fc="
    }
  }
}
```

<span data-ttu-id="b23d2-109">**Drive** リソースと **DriveItem** リソースでは、次の異なる 3 つの方法でデータを公開します。</span><span class="sxs-lookup"><span data-stu-id="b23d2-109">**Drive** and **DriveItem** resources expose data in three different ways:</span></span>

* <span data-ttu-id="b23d2-110">_プロパティ_ (**ID** や**名前**など) は単純な値 (文字列、数値、ブール値) を公開します。</span><span class="sxs-lookup"><span data-stu-id="b23d2-110">_Properties_ (like **id** and **name**) expose simple values (strings, numbers, Booleans).</span></span>
* <span data-ttu-id="b23d2-111">_ファセット_ (**file** や **photo** など) は複雑な値を公開します。</span><span class="sxs-lookup"><span data-stu-id="b23d2-111">_Facets_ (like **file** and **photo**) expose complex values.</span></span> <span data-ttu-id="b23d2-112">**file** または **folder** ファセットの有無は、**DriveItem** の動作およびプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b23d2-112">Facets (like file and photo) expose complex values. The presence of **file** or **folder** facets indicates behaviors and properties of a **DriveItem**.</span></span>
* <span data-ttu-id="b23d2-113">_参照_ (**子**と**サムネイル**など) はその他のリソースのコレクションを指します。</span><span class="sxs-lookup"><span data-stu-id="b23d2-113">_References_ (like **children** and **thumbnails**) point to collections of other resources.</span></span>

## <a name="commonly-accessed-resources"></a><span data-ttu-id="b23d2-114">一般的にアクセスされるリソース</span><span class="sxs-lookup"><span data-stu-id="b23d2-114">Commonly accessed resources</span></span>

<span data-ttu-id="b23d2-115">ファイルの相互作用に関するほとんどの API 要求では、**Drive** または **DriveItem** にアクセスするために以下の基本リソースのいずれかを使用します。</span><span class="sxs-lookup"><span data-stu-id="b23d2-115">Most API requests for file interactions will use one of these base resources to access a **Drive** or **DriveItem**.</span></span>

| <span data-ttu-id="b23d2-116">パス</span><span class="sxs-lookup"><span data-stu-id="b23d2-116">Path</span></span>    | <span data-ttu-id="b23d2-117">リソース</span><span class="sxs-lookup"><span data-stu-id="b23d2-117">Resource</span></span>    |
|---------|-------------|
| `/me/drive` | <span data-ttu-id="b23d2-118">ユーザーの OneDrive。</span><span class="sxs-lookup"><span data-stu-id="b23d2-118">User's OneDrive</span></span> |
| `/me/drives` | <span data-ttu-id="b23d2-119">そのユーザーに使用できる OneDrive リソースを列挙します。</span><span class="sxs-lookup"><span data-stu-id="b23d2-119">Enumerate OneDrive resources available to the user.</span></span> |
| `/drives/{drive-id}` | <span data-ttu-id="b23d2-120">ドライブの ID を使用して特定の **Drive** にアクセスします。</span><span class="sxs-lookup"><span data-stu-id="b23d2-120">Access a specific **Drive** by the drive's ID.</span></span> |
| `/drives/{drive-id}/root/children` | <span data-ttu-id="b23d2-121">特定の **Drive** のルートにある **DriveItem** リソースを列挙します。</span><span class="sxs-lookup"><span data-stu-id="b23d2-121">Enumerate the **DriveItem** resources in the root of a specific **Drive**.</span></span> |
| `/me/drive/items/{item-id}` | <span data-ttu-id="b23d2-122">一意の ID を使用してユーザーの OneDrive にある **DriveItem** にアクセスします。</span><span class="sxs-lookup"><span data-stu-id="b23d2-122">Access a **DriveItem** in the user's OneDrive by its unique ID.</span></span> |
| `/me/drive/special/{special-id}` | <span data-ttu-id="b23d2-123">既知の名前を使用してユーザーの OneDrive にある特別な (名前付き) フォルダーにアクセスします。</span><span class="sxs-lookup"><span data-stu-id="b23d2-123">Access a special (named) folder in the user's OneDrive by its known name.</span></span> |
| `/users/{user-id}/drive` | <span data-ttu-id="b23d2-124">別のユーザーの一意の ID を使用してそのユーザーの OneDrive にアクセスします。</span><span class="sxs-lookup"><span data-stu-id="b23d2-124">Access another user's OneDrive by using the user's unique ID.</span></span> |
| `/groups/{group-id}/drive` | <span data-ttu-id="b23d2-125">グループの一意の ID を使用してグループの既定のドキュメント ライブラリにアクセスします。</span><span class="sxs-lookup"><span data-stu-id="b23d2-125">Access the default document library for a group by the group's unique ID.</span></span> |
| `/shares/{share-id}` | <span data-ttu-id="b23d2-126">**sharedId** や共有 URL を使用して **DriveItem** にアクセスします。</span><span class="sxs-lookup"><span data-stu-id="b23d2-126">Access a **DriveItem** by its **sharedId** or sharing URL.</span></span> |

<span data-ttu-id="b23d2-127">一意の ID を使用して **Drive** 内の **DriveItem** にアドレス指定することに加え、既知のリソースからの相対パスを使用することによってアプリで **DriveItem** にアドレス指定することもできます。</span><span class="sxs-lookup"><span data-stu-id="b23d2-127">In addition to addressing a **DriveItem** within a **Drive** by unique ID, your app can also address a **DriveItem** by relative path from a known resource. To address using a path, the colon () character is used to escape the relative path. This table provides an example of different ways to use the colon character to address an item by path.</span></span>
<span data-ttu-id="b23d2-128">パスを使用してアドレス指定するには、コロン (`:`) を使用して相対パスをエスケープします。</span><span class="sxs-lookup"><span data-stu-id="b23d2-128">To address using a path, the colon (`:`) character is used to escape the relative path.</span></span>
<span data-ttu-id="b23d2-129">次の表に、コロンを使用してパスでアイテムをアドレス指定するいくつかの方法を示します。</span><span class="sxs-lookup"><span data-stu-id="b23d2-129">This table provides an example of different ways to use the colon character to address an item by path.</span></span>

| <span data-ttu-id="b23d2-130">パス</span><span class="sxs-lookup"><span data-stu-id="b23d2-130">Path</span></span> | <span data-ttu-id="b23d2-131">リソース</span><span class="sxs-lookup"><span data-stu-id="b23d2-131">Resource</span></span> |
|---|---|
| `/me/drive/root:/path/to/file` | <span data-ttu-id="b23d2-132">ユーザーの OneDrive ルート フォルダーへの相対パスを使用して **DriveItem** にアクセスします。</span><span class="sxs-lookup"><span data-stu-id="b23d2-132">Access a **DriveItem** by path relative to the user's OneDrive root folder.</span></span> |
| `/me/drive/items/{item-id}:/path/to/file` | <span data-ttu-id="b23d2-133">別のアイテム (**folder** ファセットを持つ **DriveItem**) への相対パスを使用して **DriveItem** にアクセスします。</span><span class="sxs-lookup"><span data-stu-id="b23d2-133">Access a **DriveItem** by path relative to another item (a **DriveItem** with a **folder** facet).</span></span> |
| `/me/drive/root:/path/to/folder:/children` | <span data-ttu-id="b23d2-134">ユーザーの OneDrive のルートへの相対パスを使用して **DriveItem** の子を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="b23d2-134">List the children of a **DriveItem** by path relative to the root of the user's OneDrive.</span></span> |
| `/me/drive/items/{item-id}:/path/to/folder:/children` | <span data-ttu-id="b23d2-135">別のアイテムへの相対パスを使用して **DriveItem** の子を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="b23d2-135">List the children of a **DriveItem** by path relative to another item.</span></span> |

## <a name="drive-resource"></a><span data-ttu-id="b23d2-136">ドライブ リソース</span><span class="sxs-lookup"><span data-stu-id="b23d2-136">Drive resource</span></span>

<span data-ttu-id="b23d2-137">[ドライブ リソース](drive.md)は、ユーザーの OneDrive または SharePoint ドキュメント ライブラリ内の最上位のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="b23d2-137">The [Drive resource](drive.md) is the top-level object within a user's OneDrive or a SharePoint document library. Nearly all files operations will start by addressing a specific drive resource.</span></span>
<span data-ttu-id="b23d2-138">ほぼすべてのファイル操作は、特定のドライブ リソースをアドレス指定することによって開始されます。</span><span class="sxs-lookup"><span data-stu-id="b23d2-138">The Drive resource is the top-level object within a user's OneDrive or a SharePoint document library. Nearly all files operations will start by addressing a specific drive resource.</span></span>

<span data-ttu-id="b23d2-139">ドライブの一意の ID または [User](user.md)、[Group](group.md)、組織の既定のドライブを使用して、ドライブ リソースをアドレス指定できます。</span><span class="sxs-lookup"><span data-stu-id="b23d2-139">A drive resource can be addressed either by the drive's unique ID or by the default drive for a [User](user.md), [Group](group.md), or organization.</span></span> 

## <a name="driveitem-resource"></a><span data-ttu-id="b23d2-140">DriveItem リソース</span><span class="sxs-lookup"><span data-stu-id="b23d2-140">DriveItem resource</span></span>

<span data-ttu-id="b23d2-141">[DriveItem](driveitem.md) は、ドライブのファイル システム内のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="b23d2-141">[DriveItems](driveitem.md) are the objects inside a drive's file system.</span></span>
<span data-ttu-id="b23d2-142">`/items/{item-id}` 構文で **id** を使用して、または `/root:/path/to/item/` 構文でファイル システム パスを使用して、それらにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="b23d2-142">DriveItems are the objects inside a drive's file system. They can be accessed by their **id** by using `/items/{item-id}` syntax, or by their file system path using the `/root:/path/to/item/` syntax.</span></span>

<span data-ttu-id="b23d2-143">DriveItem には、アイテムの ID と機能に関するデータを提供する_ファセット_が存在します。</span><span class="sxs-lookup"><span data-stu-id="b23d2-143">DriveItems have _facets_ that provide data about the item's identity and capabilities.</span></span>

<span data-ttu-id="b23d2-144">**folder** ファセットを持つ DriveItem は、アイテムのコンテナーとして機能し、フォルダーの下のアイテムのコレクションを指す**子**参照を持ちます。</span><span class="sxs-lookup"><span data-stu-id="b23d2-144">DriveItems with a **folder** facet act as containers of items, and have a **children** reference, which points to a collection of items under the folder.</span></span>

## <a name="shared-folders-and-remote-items"></a><span data-ttu-id="b23d2-145">共有フォルダーおよびリモート アイテム</span><span class="sxs-lookup"><span data-stu-id="b23d2-145">Shared folders and remote items</span></span>

<span data-ttu-id="b23d2-146">OneDrive 個人ユーザーは、別のドライブから自分の OneDrive に 1 つ以上の共有アイテムを追加できます。</span><span class="sxs-lookup"><span data-stu-id="b23d2-146">OneDrive personal users can add one or more shared items from another drive to their own OneDrive. These shared items appear as a DriveItem in the children collection with a remoteItem facet.</span></span>
<span data-ttu-id="b23d2-147">これらの共有のアイテムは、[remoteItem](remoteitem.md) ファセットを持つ**子**コレクションの **DriveItem** として表示されます。</span><span class="sxs-lookup"><span data-stu-id="b23d2-147">OneDrive personal users can add one or more shared items from another drive to their own OneDrive. These shared items appear as a **DriveItem** in the **children** collection with a [remoteItem](remoteitem.md) facet.</span></span>

<span data-ttu-id="b23d2-148">共有フォルダーとリモート アイテムの操作方法の詳細については、「[リモート アイテムおよび共有フォルダー](remoteitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b23d2-148">For more information about working with shared folders and remote items, see [Remote items and shared folders](remoteitem.md).</span></span>   

## <a name="sharing-and-permissions"></a><span data-ttu-id="b23d2-149">共有とアクセス許可</span><span class="sxs-lookup"><span data-stu-id="b23d2-149">Sharing and permissions</span></span>

<span data-ttu-id="b23d2-150">OneDrive と SharePoint のドキュメント ライブラリの最も一般的な操作の 1 つは、他のユーザーとコンテンツを共有することです。</span><span class="sxs-lookup"><span data-stu-id="b23d2-150">One of the most common actions for OneDrive and SharePoint document libraries is sharing content with other people. Microsoft Graph allows your app to create sharing links, add permissions and send invitations to items in a drive.</span></span>
<span data-ttu-id="b23d2-151">Microsoft Graph を使用することによって、アプリで[共有リンク](../api/driveitem_createlink.md)を作成し、[アクセス許可を追加してドライブ内のアイテムに招待状を送信](../api/driveitem_invite.md)することができます。</span><span class="sxs-lookup"><span data-stu-id="b23d2-151">One of the most common actions for OneDrive and SharePoint document libraries is sharing content with other people. Microsoft Graph allows your app to create [sharing links](../api/driveitem_createlink.md), [add permissions and send invitations](../api/driveitem_invite.md) to items in a drive.</span></span>

<span data-ttu-id="b23d2-152">Microsoft Graph では、アプリで共有リンクから[共有コンテンツに直接アクセス](../api/shares_get.md)することもできます。</span><span class="sxs-lookup"><span data-stu-id="b23d2-152">Microsoft Graph also provides a way for your app to [access shared content](../api/shares_get.md) directly from a sharing link.</span></span>

 
