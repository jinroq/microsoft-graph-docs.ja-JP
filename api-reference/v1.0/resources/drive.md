# <a name="drive-resource-type"></a><span data-ttu-id="4895f-101">ドライブ リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4895f-101">Drive resource type</span></span>

<span data-ttu-id="4895f-102">ドライブ リソースは、ユーザーの OneDrive または SharePoint のドキュメント ライブラリを表す、最上位のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="4895f-102">The drive resource is the top level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="4895f-p101">OneDrive のユーザーは、少なくとも 1 つのドライブ (そのユーザーの既定のドライブ) を常に使用できます。OneDrive のライセンスが付与されていないユーザーには、使用可能な既定のドライブがないことがあります。</span><span class="sxs-lookup"><span data-stu-id="4895f-p101">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4895f-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4895f-105">JSON representation</span></span>

<span data-ttu-id="4895f-106">以下は、**ドライブ** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4895f-106">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="4895f-107">**drive** リソースは [**baseItem**](baseitem.md) から派生し、そのリソースからプロパティを継承します。</span><span class="sxs-lookup"><span data-stu-id="4895f-107">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "items", "root", "special", "owner", "description" ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.drive"
}-->

```json
{
  "id": "string (identifier)",
  "driveType": "string",
  "owner": {"@odata.type": "microsoft.graph.identitySet"},
  "quota": {"@odata.type": "microsoft.graph.quota"},
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },

  /* relationships */
  "root": {"@odata.type": "microsoft.graph.driveItem" },
  "items": [ {"@odata.type": "microsoft.graph.driveItem" }],
  "special": [ {"@odata.type": "microsoft.graph.driveItem" }],

  /* inherited from baseItem */
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "datetime",
  "description": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "datetime",
  "name": "string",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="4895f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4895f-108">Properties</span></span>

| <span data-ttu-id="4895f-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4895f-109">Property</span></span>             | <span data-ttu-id="4895f-110">型</span><span class="sxs-lookup"><span data-stu-id="4895f-110">Type</span></span>                          | <span data-ttu-id="4895f-111">説明</span><span class="sxs-lookup"><span data-stu-id="4895f-111">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="4895f-112">id</span><span class="sxs-lookup"><span data-stu-id="4895f-112">id</span></span>                   | <span data-ttu-id="4895f-113">String</span><span class="sxs-lookup"><span data-stu-id="4895f-113">String</span></span>                        | <span data-ttu-id="4895f-p102">ドライブの一意識別子。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="4895f-p102">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="4895f-116">createdBy</span><span class="sxs-lookup"><span data-stu-id="4895f-116">createdBy</span></span>            | <span data-ttu-id="4895f-117">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="4895f-117">[identitySet][]</span></span>               | <span data-ttu-id="4895f-p103">アイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4895f-p103">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="4895f-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4895f-120">createdDateTime</span></span>      | <span data-ttu-id="4895f-121">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4895f-121">dateTimeOffset</span></span>                | <span data-ttu-id="4895f-p104">アイテム作成の日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4895f-p104">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="4895f-124">driveType</span><span class="sxs-lookup"><span data-stu-id="4895f-124">driveType</span></span>            | <span data-ttu-id="4895f-125">String</span><span class="sxs-lookup"><span data-stu-id="4895f-125">String</span></span>                        | <span data-ttu-id="4895f-p105">このリソースで表されるドライブの種類についての説明。OneDrive 個人用のドライブは `personal` を返します。OneDrive for Business は `business` を返します。SharePoint ドキュメント ライブラリは `documentLibrary` を返します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="4895f-p105">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="4895f-131">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="4895f-131">lastModifiedBy</span></span>       | <span data-ttu-id="4895f-132">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="4895f-132">[identitySet][]</span></span>               | <span data-ttu-id="4895f-p106">アイテムを最終更新したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4895f-p106">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="4895f-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4895f-135">lastModifiedDateTime</span></span> | <span data-ttu-id="4895f-136">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4895f-136">dateTimeOffset</span></span>                | <span data-ttu-id="4895f-p107">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4895f-p107">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="4895f-139">name</span><span class="sxs-lookup"><span data-stu-id="4895f-139">name</span></span>                 | <span data-ttu-id="4895f-140">string</span><span class="sxs-lookup"><span data-stu-id="4895f-140">string</span></span>                        | <span data-ttu-id="4895f-p108">アイテムの名前。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="4895f-p108">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="4895f-143">owner</span><span class="sxs-lookup"><span data-stu-id="4895f-143">owner</span></span>                | [<span data-ttu-id="4895f-144">identitySet</span><span class="sxs-lookup"><span data-stu-id="4895f-144">identitySet</span></span>](identityset.md) | <span data-ttu-id="4895f-p109">省略可能。ドライブを所有しているユーザー アカウント。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4895f-p109">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="4895f-148">クォータ</span><span class="sxs-lookup"><span data-stu-id="4895f-148">quota</span></span>                | [<span data-ttu-id="4895f-149">quota</span><span class="sxs-lookup"><span data-stu-id="4895f-149">quota</span></span>](quota.md)             | <span data-ttu-id="4895f-p110">省略可能。ドライブの記憶領域クォータに関する情報。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4895f-p110">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="4895f-153">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="4895f-153">sharepointIds</span></span>        | <span data-ttu-id="4895f-154">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="4895f-154">[sharepointIds][]</span></span>             | <span data-ttu-id="4895f-p111">SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4895f-p111">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="4895f-157">webUrl</span><span class="sxs-lookup"><span data-stu-id="4895f-157">webUrl</span></span>               | <span data-ttu-id="4895f-158">string (URL)</span><span class="sxs-lookup"><span data-stu-id="4895f-158">string (url)</span></span>                  | <span data-ttu-id="4895f-p112">ブラウザーでリソースを表示するための URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4895f-p112">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

<span data-ttu-id="4895f-161">[identitySet]: identityset.md</span><span class="sxs-lookup"><span data-stu-id="4895f-161">[identitySet]: identityset.md</span></span>
<span data-ttu-id="4895f-162">[sharepointIds]: sharepointids.md</span><span class="sxs-lookup"><span data-stu-id="4895f-162">[sharepointIds]: sharepointids.md</span></span>

## <a name="relationships"></a><span data-ttu-id="4895f-163">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4895f-163">Relationships</span></span>

| <span data-ttu-id="4895f-164">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4895f-164">Relationship</span></span> | <span data-ttu-id="4895f-165">型</span><span class="sxs-lookup"><span data-stu-id="4895f-165">Type</span></span>                                 | <span data-ttu-id="4895f-166">説明</span><span class="sxs-lookup"><span data-stu-id="4895f-166">Description</span></span>                                                              |
| :----------- | :----------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="4895f-167">items</span><span class="sxs-lookup"><span data-stu-id="4895f-167">items</span></span>        | <span data-ttu-id="4895f-168">[driveitem](driveitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4895f-168">[driveitem](driveitem.md) collection</span></span> | <span data-ttu-id="4895f-p113">ドライブに含まれているすべてのアイテム。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="4895f-p113">All items contained in the drive. Read-only. Nullable.</span></span>                   |
| <span data-ttu-id="4895f-172">root</span><span class="sxs-lookup"><span data-stu-id="4895f-172">root</span></span>         | [<span data-ttu-id="4895f-173">driveitem</span><span class="sxs-lookup"><span data-stu-id="4895f-173">driveitem</span></span>](driveitem.md)            | <span data-ttu-id="4895f-p114">ドライブのルート フォルダー。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="4895f-p114">The root folder of the drive. Read-only.</span></span>                                 |
| <span data-ttu-id="4895f-176">special</span><span class="sxs-lookup"><span data-stu-id="4895f-176">special</span></span>      | <span data-ttu-id="4895f-177">[driveitem](driveitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4895f-177">[driveitem](driveitem.md) collection</span></span> | <span data-ttu-id="4895f-p115">OneDrive で使用可能な共通フォルダーのコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="4895f-p115">Collection of common folders available in OneDrive. Read-only. Nullable.</span></span> |

## <a name="methods"></a><span data-ttu-id="4895f-181">メソッド</span><span class="sxs-lookup"><span data-stu-id="4895f-181">Methods</span></span>

<span data-ttu-id="4895f-182">次に、ドライブ リソースで使用可能なメソッドを示します。</span><span class="sxs-lookup"><span data-stu-id="4895f-182">The following methods are available for drive resources.</span></span>

| <span data-ttu-id="4895f-183">メソッド</span><span class="sxs-lookup"><span data-stu-id="4895f-183">Method</span></span>                                                | <span data-ttu-id="4895f-184">REST パス</span><span class="sxs-lookup"><span data-stu-id="4895f-184">REST Path</span></span>                        |
| :---------------------------------------------------- | :------------------------------- |
| [<span data-ttu-id="4895f-185">ユーザーの既定のドライブの取得</span><span class="sxs-lookup"><span data-stu-id="4895f-185">Get user's default drive</span></span>](../api/drive_get.md)       | `GET /me/drive`                  |
| [<span data-ttu-id="4895f-186">別のユーザーのドライブの取得</span><span class="sxs-lookup"><span data-stu-id="4895f-186">Get another user's drive</span></span>](../api/drive_get.md)       | `GET /users/{user-id}/drive`     |
| [<span data-ttu-id="4895f-187">ドライブのルート フォルダーの取得</span><span class="sxs-lookup"><span data-stu-id="4895f-187">Get root folder for a drive</span></span>](../api/item_get.md)     | `GET /drives/{drive-id}/root`    |
| [<span data-ttu-id="4895f-188">ドライブ内のアイテムの一覧</span><span class="sxs-lookup"><span data-stu-id="4895f-188">List items in a drive</span></span>](../api/item_list_children.md) | `GET /me/drive/root/children`    |
| [<span data-ttu-id="4895f-189">ドライブ内の変更内容の一覧</span><span class="sxs-lookup"><span data-stu-id="4895f-189">List changes in a drive</span></span>](../api/item_delta.md)       | `GET /me/drive/root/delta`       |
| [<span data-ttu-id="4895f-190">ドライブ内のアイテムの検索</span><span class="sxs-lookup"><span data-stu-id="4895f-190">Search items in a drive</span></span>](../api/item_search.md)      | `GET /me/drive/search(q='text')` |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "drive resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Drive"
}-->
