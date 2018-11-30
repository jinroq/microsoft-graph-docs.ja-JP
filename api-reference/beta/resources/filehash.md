---
title: fileHash リソースの種類
description: ステートフルな暗号化などの場所に依存したファイルのハッシュについてを説明します。
ms.openlocfilehash: 8f283046efc9b4af181cb33fb4e9ca63e4892b67
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070730"
---
# <a name="filehash-resource-type"></a><span data-ttu-id="293bf-103">fileHash リソースの種類</span><span class="sxs-lookup"><span data-stu-id="293bf-103">fileHash resource type</span></span>

<span data-ttu-id="293bf-104">ステートフルな暗号化などの場所に依存したファイルのハッシュについてを説明します。</span><span class="sxs-lookup"><span data-stu-id="293bf-104">Contains stateful information about file hashes (cryptographic and location-sensitive).</span></span>

## <a name="properties"></a><span data-ttu-id="293bf-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="293bf-105">Properties</span></span>

| <span data-ttu-id="293bf-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="293bf-106">Property</span></span>     | <span data-ttu-id="293bf-107">型</span><span class="sxs-lookup"><span data-stu-id="293bf-107">Type</span></span>        | <span data-ttu-id="293bf-108">説明</span><span class="sxs-lookup"><span data-stu-id="293bf-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="293bf-109">hashType</span><span class="sxs-lookup"><span data-stu-id="293bf-109">hashType</span></span>|<span data-ttu-id="293bf-110">[fileHashType](filehashtypeenumtype.md)列挙型</span><span class="sxs-lookup"><span data-stu-id="293bf-110">[fileHashType](filehashtypeenumtype.md) enum</span></span>|<span data-ttu-id="293bf-111">ファイル ハッシュ タイプを入力します。</span><span class="sxs-lookup"><span data-stu-id="293bf-111">File hash type.</span></span> <span data-ttu-id="293bf-112">可能な値は、`unknown`、`sha1`、`sha256`、`md5`、`authenticodeHash256`、`lsHash`、`ctph`、`peSha1`、`peSha256` です。</span><span class="sxs-lookup"><span data-stu-id="293bf-112">Possible values are: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span></span>|
|<span data-ttu-id="293bf-113">して</span><span class="sxs-lookup"><span data-stu-id="293bf-113">hashValue</span></span>|<span data-ttu-id="293bf-114">String</span><span class="sxs-lookup"><span data-stu-id="293bf-114">String</span></span>|<span data-ttu-id="293bf-115">ファイル ハッシュの値です。</span><span class="sxs-lookup"><span data-stu-id="293bf-115">Value of the file hash.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="293bf-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="293bf-116">JSON representation</span></span>

<span data-ttu-id="293bf-117">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="293bf-117">The following is a JSON representation of the resource.</span></span>

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