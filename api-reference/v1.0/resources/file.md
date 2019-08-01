---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: File
localization_priority: Normal
description: ファイル リソースは、ファイル関連のデータ項目を 1 つの構造にグループ化します。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 51ec91a635db2ca259ba84cea29304e4e6ac7cbb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030374"
---
# <a name="file-resource-type"></a><span data-ttu-id="214f7-103">ファイル リソースの種類</span><span class="sxs-lookup"><span data-stu-id="214f7-103">File resource type</span></span>

<span data-ttu-id="214f7-104">**ファイル** リソースは、ファイル関連のデータ項目を 1 つの構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="214f7-104">The **File** resource groups file-related data items into a single structure.</span></span>

<span data-ttu-id="214f7-p101">[**DriveItem**](driveitem.md) に null 以外の**ファイル** ファセットがある場合は、項目はファイルを表します。他のプロパティに加えて、ファイルにはファイルのバイト ストリームを含む**コンテンツ**関係があります。</span><span class="sxs-lookup"><span data-stu-id="214f7-p101">If a [**DriveItem**](driveitem.md) has a non-null **file** facet, the item represents an file. In addition to other properties, files have a **content** relationship which contains the byte stream of the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="214f7-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="214f7-107">JSON representation</span></span>

<span data-ttu-id="214f7-108">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="214f7-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.file"
}-->

```json
{
  "hashes": {"@odata.type": "microsoft.graph.hashes"},
  "mimeType": "string"
}
```

## <a name="properties"></a><span data-ttu-id="214f7-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="214f7-109">Properties</span></span>

| <span data-ttu-id="214f7-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="214f7-110">Property</span></span> | <span data-ttu-id="214f7-111">型</span><span class="sxs-lookup"><span data-stu-id="214f7-111">Type</span></span>                    | <span data-ttu-id="214f7-112">説明</span><span class="sxs-lookup"><span data-stu-id="214f7-112">Description</span></span>                                                                                                                                      |
|:---------|:------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="214f7-113">hashes</span><span class="sxs-lookup"><span data-stu-id="214f7-113">hashes</span></span>   | [<span data-ttu-id="214f7-114">方向性</span><span class="sxs-lookup"><span data-stu-id="214f7-114">Hashes</span></span>](hashes.md) | <span data-ttu-id="214f7-p102">ファイルのバイナリ コンテンツのハッシュ (利用可能な場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="214f7-p102">Hashes of the file's binary content, if available. Read-only.</span></span>                                                                                    |
| <span data-ttu-id="214f7-117">mimeType</span><span class="sxs-lookup"><span data-stu-id="214f7-117">mimeType</span></span> | <span data-ttu-id="214f7-118">string</span><span class="sxs-lookup"><span data-stu-id="214f7-118">string</span></span>                  | <span data-ttu-id="214f7-p103">ファイルの MIME の種類。これはサーバーのロジックによって決定されます。またファイルのアップロード時に指定された値でない場合があります。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="214f7-p103">The MIME type for the file. This is determined by logic on the server and might not be the value provided when the file was uploaded. Read-only.</span></span> |

## <a name="remarks"></a><span data-ttu-id="214f7-122">注釈</span><span class="sxs-lookup"><span data-stu-id="214f7-122">Remarks</span></span> 

<span data-ttu-id="214f7-123">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="214f7-123">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The file facet describes properties of a file",
  "keywords": "file,item,facet",
  "section": "documentation",
  "tocPath": "Facets/File"
} -->
