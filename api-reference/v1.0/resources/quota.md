# <a name="quota-resource-type"></a><span data-ttu-id="d5f06-101">クォータ リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d5f06-101">Quota resource type</span></span>

<span data-ttu-id="d5f06-102">**クォータ** リソースは、[ドライブ](drive.md) リソースの領域の制約に関する詳細を提供します。</span><span class="sxs-lookup"><span data-stu-id="d5f06-102">The **quota** resource provides details about space constrains on a [Drive](drive.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5f06-103">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d5f06-103">JSON representation</span></span>

<span data-ttu-id="d5f06-104">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d5f06-104">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.quota"
}-->

```json
{
  "deleted": 1024,
  "remaining": 1024,
  "state": "normal | nearing | critical | exceeded",
  "total": 1024,
  "used": 1024
}
```

## <a name="properties"></a><span data-ttu-id="d5f06-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d5f06-105">Properties</span></span>

| <span data-ttu-id="d5f06-106">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="d5f06-106">Property name</span></span> | <span data-ttu-id="d5f06-107">種類</span><span class="sxs-lookup"><span data-stu-id="d5f06-107">Type</span></span>   | <span data-ttu-id="d5f06-108">説明</span><span class="sxs-lookup"><span data-stu-id="d5f06-108">Description</span></span>                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| <span data-ttu-id="d5f06-109">total</span><span class="sxs-lookup"><span data-stu-id="d5f06-109">total</span></span>         | <span data-ttu-id="d5f06-110">Int64</span><span class="sxs-lookup"><span data-stu-id="d5f06-110">Int64</span></span>  | <span data-ttu-id="d5f06-p101">許可されている記憶域の合計 (バイト単位)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d5f06-p101">Total allowed storage space, in bytes. Read-only.</span></span>                           |
| <span data-ttu-id="d5f06-113">used</span><span class="sxs-lookup"><span data-stu-id="d5f06-113">used</span></span>          | <span data-ttu-id="d5f06-114">Int64</span><span class="sxs-lookup"><span data-stu-id="d5f06-114">Int64</span></span>  | <span data-ttu-id="d5f06-p102">使用領域の合計 (バイト単位)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d5f06-p102">Total space used, in bytes. Read-only.</span></span>                                      |
| <span data-ttu-id="d5f06-117">remaining</span><span class="sxs-lookup"><span data-stu-id="d5f06-117">remaining</span></span>     | <span data-ttu-id="d5f06-118">Int64</span><span class="sxs-lookup"><span data-stu-id="d5f06-118">Int64</span></span>  | <span data-ttu-id="d5f06-p103">クォータ制限に達するまでの残りの領域の合計 (バイト単位)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d5f06-p103">Total space remaining before reaching the quota limit, in bytes. Read-only.</span></span> |
| <span data-ttu-id="d5f06-121">deleted</span><span class="sxs-lookup"><span data-stu-id="d5f06-121">deleted</span></span>       | <span data-ttu-id="d5f06-122">Int64</span><span class="sxs-lookup"><span data-stu-id="d5f06-122">Int64</span></span>  | <span data-ttu-id="d5f06-p104">ごみ箱内のファイルによって消費されている領域の合計 (バイト単位)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d5f06-p104">Total space consumed by files in the recycle bin, in bytes. Read-only.</span></span>      |
| <span data-ttu-id="d5f06-125">state</span><span class="sxs-lookup"><span data-stu-id="d5f06-125">state</span></span>         | <span data-ttu-id="d5f06-126">string</span><span class="sxs-lookup"><span data-stu-id="d5f06-126">string</span></span> | <span data-ttu-id="d5f06-p105">記憶域の状態を示す列挙値。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d5f06-p105">Enumeration value that indicates the state of the storage space. Read-only.</span></span> |

## <a name="state-enumeration"></a><span data-ttu-id="d5f06-129">状態の列挙値</span><span class="sxs-lookup"><span data-stu-id="d5f06-129">State Enumeration</span></span>

| <span data-ttu-id="d5f06-130">値</span><span class="sxs-lookup"><span data-stu-id="d5f06-130">Value</span></span>      | <span data-ttu-id="d5f06-131">説明</span><span class="sxs-lookup"><span data-stu-id="d5f06-131">Description</span></span>                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | <span data-ttu-id="d5f06-132">ドライブに十分なクォータが残っています。</span><span class="sxs-lookup"><span data-stu-id="d5f06-132">The drive has plenty of remaining quota left.</span></span>                                                                                                                               |
| `nearing`  | <span data-ttu-id="d5f06-133">残りのクォータは、クォータ領域の合計の 10% 未満です。</span><span class="sxs-lookup"><span data-stu-id="d5f06-133">Remaining quota is less than 10% of total quota space.</span></span>                                                                                                                      |
| `critical` | <span data-ttu-id="d5f06-134">残りのクォータは、クォータ領域の合計の 1% 未満です。</span><span class="sxs-lookup"><span data-stu-id="d5f06-134">Remaining quota is less than 1% of total quota space.</span></span>                                                                                                                       |
| `exceeded` | <span data-ttu-id="d5f06-p106">クォータ使用量が、クォータの合計を超えています。クォータの合計を下回るか、追加の記憶領域を購入するまで、新しいファイルまたはフォルダーをドライブに追加することはできません。</span><span class="sxs-lookup"><span data-stu-id="d5f06-p106">The used quota has exceeded the total quota. New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "quota resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
