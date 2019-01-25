---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: File
localization_priority: Normal
ms.openlocfilehash: 5812cffd4f7efbcd368cd576df0e16f4aedb7f1a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528418"
---
# <a name="file-resource-type"></a><span data-ttu-id="82463-102">ファイル リソースの種類</span><span class="sxs-lookup"><span data-stu-id="82463-102">File resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82463-103">**ファイル** リソースは、ファイル関連のデータ項目を 1 つの構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="82463-103">The **File** resource groups file-related data items into a single structure.</span></span>

<span data-ttu-id="82463-p101">DriveItem に null 以外のファイル ファセットがある場合は、項目はファイルを表します。他のプロパティに加えて、ファイルにはファイルのバイト ストリームを含むコンテンツ関係があります。</span><span class="sxs-lookup"><span data-stu-id="82463-p101">If a [**DriveItem**](driveitem.md) has a non-null **file** facet, the item represents an file. In addition to other properties, files have a **content** relationship which contains the byte stream of the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="82463-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="82463-106">JSON representation</span></span>

<span data-ttu-id="82463-107">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="82463-107">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="82463-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="82463-108">Properties</span></span>

| <span data-ttu-id="82463-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="82463-109">Property</span></span> | <span data-ttu-id="82463-110">型</span><span class="sxs-lookup"><span data-stu-id="82463-110">Type</span></span>                    | <span data-ttu-id="82463-111">説明</span><span class="sxs-lookup"><span data-stu-id="82463-111">Description</span></span>                                                                                                                                      |
|:---------|:------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="82463-112">hashes</span><span class="sxs-lookup"><span data-stu-id="82463-112">hashes</span></span>   | [<span data-ttu-id="82463-113">HashesType</span><span class="sxs-lookup"><span data-stu-id="82463-113">HashesType</span></span>](hashes.md) | <span data-ttu-id="82463-p102">ファイルのバイナリ コンテンツのハッシュ (利用可能な場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="82463-p102">Hashes of the file's binary content, if available. Read-only.</span></span>                                                                                    |
| <span data-ttu-id="82463-116">mimeType</span><span class="sxs-lookup"><span data-stu-id="82463-116">mimeType</span></span> | <span data-ttu-id="82463-117">string</span><span class="sxs-lookup"><span data-stu-id="82463-117">string</span></span>                  | <span data-ttu-id="82463-p103">ファイルの MIME の種類。これはサーバーのロジックによって決定されます。またファイルのアップロード時に指定された値でない場合があります。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="82463-p103">The MIME type for the file. This is determined by logic on the server and might not be the value provided when the file was uploaded. Read-only.</span></span> |

## <a name="remarks"></a><span data-ttu-id="82463-121">注釈</span><span class="sxs-lookup"><span data-stu-id="82463-121">Remarks</span></span> 

<span data-ttu-id="82463-122">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="82463-122">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The file facet describes properties of a file",
  "keywords": "file,item,facet",
  "section": "documentation",
  "tocPath": "Facets/File",
  "suppressions": [
    "Error: /api-reference/beta/resources/file.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
