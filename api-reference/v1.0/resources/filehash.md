---
title: filehash リソースの種類
description: ファイルハッシュ (暗号化と場所に依存) に関するステートフルな情報を含みます。
localization_priority: Normal
ms.openlocfilehash: 9d72812d1ad43999ea3ed5b28251d629b9380d47
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564772"
---
# <a name="filehash-resource-type"></a><span data-ttu-id="ddb3f-103">filehash リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ddb3f-103">fileHash resource type</span></span>

<span data-ttu-id="ddb3f-104">ファイルハッシュ (暗号化と場所に依存) に関するステートフルな情報を含みます。</span><span class="sxs-lookup"><span data-stu-id="ddb3f-104">Contains stateful information about file hashes (cryptographic and location-sensitive).</span></span>

## <a name="properties"></a><span data-ttu-id="ddb3f-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ddb3f-105">Properties</span></span>

| <span data-ttu-id="ddb3f-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ddb3f-106">Property</span></span>     | <span data-ttu-id="ddb3f-107">型</span><span class="sxs-lookup"><span data-stu-id="ddb3f-107">Type</span></span>        | <span data-ttu-id="ddb3f-108">説明</span><span class="sxs-lookup"><span data-stu-id="ddb3f-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ddb3f-109">hashtype</span><span class="sxs-lookup"><span data-stu-id="ddb3f-109">hashType</span></span>|<span data-ttu-id="ddb3f-110">fileHashType</span><span class="sxs-lookup"><span data-stu-id="ddb3f-110">fileHashType</span></span>|<span data-ttu-id="ddb3f-111">ファイルハッシュの種類。</span><span class="sxs-lookup"><span data-stu-id="ddb3f-111">File hash type.</span></span> <span data-ttu-id="ddb3f-112">可能な値は、`unknown`、`sha1`、`sha256`、`md5`、`authenticodeHash256`、`lsHash`、`ctph`、`peSha1`、`peSha256` です。</span><span class="sxs-lookup"><span data-stu-id="ddb3f-112">Possible values are: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span></span>|
|<span data-ttu-id="ddb3f-113">hashvalue</span><span class="sxs-lookup"><span data-stu-id="ddb3f-113">hashValue</span></span>|<span data-ttu-id="ddb3f-114">String</span><span class="sxs-lookup"><span data-stu-id="ddb3f-114">String</span></span>|<span data-ttu-id="ddb3f-115">ファイルハッシュの値。</span><span class="sxs-lookup"><span data-stu-id="ddb3f-115">Value of the file hash.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ddb3f-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ddb3f-116">JSON representation</span></span>

<span data-ttu-id="ddb3f-117">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ddb3f-117">The following is a JSON representation of the resource.</span></span>

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
