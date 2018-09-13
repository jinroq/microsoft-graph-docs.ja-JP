# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="97a72-101">fileSecurityState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="97a72-101">fileSecurityState resource type</span></span>

<span data-ttu-id="97a72-102">アラートに関連するファイル (プロセスではない) に関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="97a72-102">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="97a72-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="97a72-103">Properties</span></span>

| <span data-ttu-id="97a72-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="97a72-104">Property</span></span>   | <span data-ttu-id="97a72-105">型</span><span class="sxs-lookup"><span data-stu-id="97a72-105">Type</span></span>|<span data-ttu-id="97a72-106">説明</span><span class="sxs-lookup"><span data-stu-id="97a72-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97a72-107">fileHash</span><span class="sxs-lookup"><span data-stu-id="97a72-107">fileHash</span></span>|[<span data-ttu-id="97a72-108">fileHash</span><span class="sxs-lookup"><span data-stu-id="97a72-108">fileHash</span></span>](filehash.md)|<span data-ttu-id="97a72-109">複合型の暗号化などの場所に依存したファイルのハッシュが含まれています。</span><span class="sxs-lookup"><span data-stu-id="97a72-109">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="97a72-110">名前</span><span class="sxs-lookup"><span data-stu-id="97a72-110">name</span></span>|<span data-ttu-id="97a72-111">文字列</span><span class="sxs-lookup"><span data-stu-id="97a72-111">String</span></span>|<span data-ttu-id="97a72-112">ファイル名（パスなし）。</span><span class="sxs-lookup"><span data-stu-id="97a72-112">File name (without path).</span></span>|
|<span data-ttu-id="97a72-113">パス</span><span class="sxs-lookup"><span data-stu-id="97a72-113">path</span></span>|<span data-ttu-id="97a72-114">文字列</span><span class="sxs-lookup"><span data-stu-id="97a72-114">String</span></span>|<span data-ttu-id="97a72-115">ファイル/ imageFileのフルファイルパス。</span><span class="sxs-lookup"><span data-stu-id="97a72-115">Full file path of the stencil file</span></span>|
|<span data-ttu-id="97a72-116">riskScore</span><span class="sxs-lookup"><span data-stu-id="97a72-116">riskScore</span></span>|<span data-ttu-id="97a72-117">文字列</span><span class="sxs-lookup"><span data-stu-id="97a72-117">String</span></span>|<span data-ttu-id="97a72-118">プロバイダー生成された計算されるリスクの警告ファイルのスコアです。</span><span class="sxs-lookup"><span data-stu-id="97a72-118">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="97a72-119">1 パーセンテージ相当する 0 - 1 の値の範囲を推奨します。</span><span class="sxs-lookup"><span data-stu-id="97a72-119">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="97a72-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="97a72-120">JSON representation</span></span>

<span data-ttu-id="97a72-121">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="97a72-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileSecurityState"
}-->

```json
{
  "fileHash": {"@odata.type": "microsoft.graph.fileHash"},
  "name": "String",
  "path": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->