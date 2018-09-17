# <a name="filehash-resource-type"></a><span data-ttu-id="c7e30-101">fileHash リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c7e30-101">fileHash resource type</span></span>

<span data-ttu-id="c7e30-102">ステートフルな暗号化などの場所に依存したファイルのハッシュについてを説明します。</span><span class="sxs-lookup"><span data-stu-id="c7e30-102">Contains stateful information about file hashes (cryptographic and location-sensitive).</span></span>

## <a name="properties"></a><span data-ttu-id="c7e30-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c7e30-103">Properties</span></span>

| <span data-ttu-id="c7e30-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c7e30-104">Property</span></span>     | <span data-ttu-id="c7e30-105">型</span><span class="sxs-lookup"><span data-stu-id="c7e30-105">Type</span></span>        | <span data-ttu-id="c7e30-106">説明</span><span class="sxs-lookup"><span data-stu-id="c7e30-106">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c7e30-107">hashType</span><span class="sxs-lookup"><span data-stu-id="c7e30-107">hashType</span></span>|<span data-ttu-id="c7e30-108">fileHashType</span><span class="sxs-lookup"><span data-stu-id="c7e30-108">fileHashType</span></span>|<span data-ttu-id="c7e30-109">ファイルハッシュタイプ。</span><span class="sxs-lookup"><span data-stu-id="c7e30-109">File hash type.</span></span> <span data-ttu-id="c7e30-110">可能な値は、`unknown`、`sha1`、`sha256`、`md5`、`authenticodeHash256`、`lsHash`、`ctph`、`peSha1`、`peSha256` です。</span><span class="sxs-lookup"><span data-stu-id="c7e30-110">Possible values are: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span></span>|
|<span data-ttu-id="c7e30-111">hashValue</span><span class="sxs-lookup"><span data-stu-id="c7e30-111">hashValue</span></span>|<span data-ttu-id="c7e30-112">文字列</span><span class="sxs-lookup"><span data-stu-id="c7e30-112">String</span></span>|<span data-ttu-id="c7e30-113">ファイルハッシュの値です。</span><span class="sxs-lookup"><span data-stu-id="c7e30-113">Value of the file hash.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c7e30-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c7e30-114">JSON representation</span></span>

<span data-ttu-id="c7e30-115">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c7e30-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileHash"
}-->

```json
{
  "hashType": "@odata.type: microsoft.graph.fileHashType",
  "hashValue": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileHash resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->