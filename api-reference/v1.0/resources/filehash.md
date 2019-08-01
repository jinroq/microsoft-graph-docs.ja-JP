---
title: fileHash リソースの種類
description: ファイルハッシュ (暗号化と場所に依存) に関するステートフルな情報を含みます。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: aabe56237ea44285c93f802268bd68688f16aa05
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030381"
---
# <a name="filehash-resource-type"></a><span data-ttu-id="b81e8-103">fileHash リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b81e8-103">fileHash resource type</span></span>

<span data-ttu-id="b81e8-104">ファイルハッシュ (暗号化と場所に依存) に関するステートフルな情報を含みます。</span><span class="sxs-lookup"><span data-stu-id="b81e8-104">Contains stateful information about file hashes (cryptographic and location-sensitive).</span></span>

## <a name="properties"></a><span data-ttu-id="b81e8-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b81e8-105">Properties</span></span>

| <span data-ttu-id="b81e8-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b81e8-106">Property</span></span>     | <span data-ttu-id="b81e8-107">型</span><span class="sxs-lookup"><span data-stu-id="b81e8-107">Type</span></span>        | <span data-ttu-id="b81e8-108">説明</span><span class="sxs-lookup"><span data-stu-id="b81e8-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b81e8-109">hashType</span><span class="sxs-lookup"><span data-stu-id="b81e8-109">hashType</span></span>|<span data-ttu-id="b81e8-110">fileHashType</span><span class="sxs-lookup"><span data-stu-id="b81e8-110">fileHashType</span></span>|<span data-ttu-id="b81e8-111">ファイルハッシュの種類。</span><span class="sxs-lookup"><span data-stu-id="b81e8-111">File hash type.</span></span> <span data-ttu-id="b81e8-112">可能な値は、`unknown`、`sha1`、`sha256`、`md5`、`authenticodeHash256`、`lsHash`、`ctph`、`peSha1`、`peSha256` です。</span><span class="sxs-lookup"><span data-stu-id="b81e8-112">Possible values are: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span></span>|
|<span data-ttu-id="b81e8-113">hashValue</span><span class="sxs-lookup"><span data-stu-id="b81e8-113">hashValue</span></span>|<span data-ttu-id="b81e8-114">String</span><span class="sxs-lookup"><span data-stu-id="b81e8-114">String</span></span>|<span data-ttu-id="b81e8-115">ファイルハッシュの値。</span><span class="sxs-lookup"><span data-stu-id="b81e8-115">Value of the file hash.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b81e8-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b81e8-116">JSON representation</span></span>

<span data-ttu-id="b81e8-117">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b81e8-117">The following is a JSON representation of the resource.</span></span>

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
