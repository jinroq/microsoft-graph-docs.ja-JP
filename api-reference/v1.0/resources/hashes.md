# <a name="hashes-resource-type"></a><span data-ttu-id="391ae-101">ハッシュ リソースの種類</span><span class="sxs-lookup"><span data-stu-id="391ae-101">Hashes resource type</span></span>

<span data-ttu-id="391ae-102"> **ハッシュ** リソースは、利用可能なハッシュをアイテムの 1 つの構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="391ae-102">The **Hashes** resource groups available hashes into a single structure for an item.</span></span>

<span data-ttu-id="391ae-103">**注:**すべてのサービスで、表示されているすべてのハッシュ プロパティに対して値が指定されているわけではありません。</span><span class="sxs-lookup"><span data-stu-id="391ae-103">**Note:** Not all services provide a value for all hash properties listed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="391ae-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="391ae-104">JSON representation</span></span>

<span data-ttu-id="391ae-105">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="391ae-105">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "sha1Hash", "crc32Hash", "quickXorHash" ],
  "@odata.type": "microsoft.graph.hashes"
}-->

```json
{
  "crc32Hash": "string",
  "sha1Hash": "string",
  "quickXorHash": "string"
}
```


## <a name="properties"></a><span data-ttu-id="391ae-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="391ae-106">Properties</span></span>

| <span data-ttu-id="391ae-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="391ae-107">Property</span></span>         | <span data-ttu-id="391ae-108">型</span><span class="sxs-lookup"><span data-stu-id="391ae-108">Type</span></span>   | <span data-ttu-id="391ae-109">説明</span><span class="sxs-lookup"><span data-stu-id="391ae-109">Description</span></span>                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| <span data-ttu-id="391ae-110">**sha1Hash**</span><span class="sxs-lookup"><span data-stu-id="391ae-110">**sha1Hash**</span></span>     | <span data-ttu-id="391ae-111">文字列</span><span class="sxs-lookup"><span data-stu-id="391ae-111">String</span></span> | <span data-ttu-id="391ae-p101">ファイルの内容の SHA1 ハッシュ (使用可能な場合)。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="391ae-p101">SHA1 hash for the contents of the file (if available). Read-only.</span></span> |
| <span data-ttu-id="391ae-114">**crc32Hash**</span><span class="sxs-lookup"><span data-stu-id="391ae-114">**crc32Hash**</span></span>    | <span data-ttu-id="391ae-115">文字列</span><span class="sxs-lookup"><span data-stu-id="391ae-115">String</span></span> | <span data-ttu-id="391ae-p102">ファイルの CRC32 の値 (使用可能な場合)。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="391ae-p102">The CRC32 value of the file (if available). Read-only.</span></span>            |
| <span data-ttu-id="391ae-118">**quickXorHash**</span><span class="sxs-lookup"><span data-stu-id="391ae-118">**quickXorHash**</span></span> | <span data-ttu-id="391ae-119">文字列</span><span class="sxs-lookup"><span data-stu-id="391ae-119">String</span></span> | <span data-ttu-id="391ae-p103">ファイルの内容が変更されているかどうかの判別に使用できるファイルの専用ハッシュ (使用可能な場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="391ae-p103">A proprietary hash of the file that can be used to determine if the contents of the file have changed (if available). Read-only.</span></span> |

<span data-ttu-id="391ae-p104">**注:**ハッシュ値が使用可能ではない場合があります。その場合、アイテムのハッシュ値は、アイテムがダウンロードされた後に更新されます。</span><span class="sxs-lookup"><span data-stu-id="391ae-p104">**Note:** In some cases hash values may not be available. If this is the case, the hash values on an item will be updated after the item is downloaded.</span></span>


## <a name="remarks"></a><span data-ttu-id="391ae-124">注釈</span><span class="sxs-lookup"><span data-stu-id="391ae-124">Remarks</span></span>

<span data-ttu-id="391ae-p105">OneDrive for Business では、**sha1Hash** と **crc32Hash** は利用できません。OneDrive Personal では、**quickXorHash** は利用できません。</span><span class="sxs-lookup"><span data-stu-id="391ae-p105">In OneDrive for Business, **sha1Hash** and **crc32Hash** are not available. In OneDrive Personal, **quickXorHash** is not available.</span></span>

<span data-ttu-id="391ae-127">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="391ae-127">For more information about the facets on a [driveItem](driveitem.md), see driveItem.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "hashes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
