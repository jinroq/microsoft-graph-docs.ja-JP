---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: File
localization_priority: Normal
ms.openlocfilehash: 7478ba064b5193ce7ddcd8685fc571a72d4b0057
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564786"
---
# <a name="file-resource-type"></a><span data-ttu-id="79490-102">ファイル リソースの種類</span><span class="sxs-lookup"><span data-stu-id="79490-102">File resource type</span></span>

<span data-ttu-id="79490-103">**ファイル** リソースは、ファイル関連のデータ項目を 1 つの構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="79490-103">The **File** resource groups file-related data items into a single structure.</span></span>

<span data-ttu-id="79490-p101">[**DriveItem**](driveitem.md) に null 以外の**ファイル** ファセットがある場合は、項目はファイルを表します。他のプロパティに加えて、ファイルにはファイルのバイト ストリームを含む**コンテンツ**関係があります。</span><span class="sxs-lookup"><span data-stu-id="79490-p101">If a [**DriveItem**](driveitem.md) has a non-null **file** facet, the item represents an file. In addition to other properties, files have a **content** relationship which contains the byte stream of the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="79490-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="79490-106">JSON representation</span></span>

<span data-ttu-id="79490-107">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="79490-107">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="79490-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="79490-108">Properties</span></span>

| <span data-ttu-id="79490-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="79490-109">Property</span></span> | <span data-ttu-id="79490-110">型</span><span class="sxs-lookup"><span data-stu-id="79490-110">Type</span></span>                    | <span data-ttu-id="79490-111">説明</span><span class="sxs-lookup"><span data-stu-id="79490-111">Description</span></span>                                                                                                                                      |
|:---------|:------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="79490-112">hashes</span><span class="sxs-lookup"><span data-stu-id="79490-112">hashes</span></span>   | [<span data-ttu-id="79490-113">方向性</span><span class="sxs-lookup"><span data-stu-id="79490-113">Hashes</span></span>](hashes.md) | <span data-ttu-id="79490-p102">ファイルのバイナリ コンテンツのハッシュ (利用可能な場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="79490-p102">Hashes of the file's binary content, if available. Read-only.</span></span>                                                                                    |
| <span data-ttu-id="79490-116">mimeType</span><span class="sxs-lookup"><span data-stu-id="79490-116">mimeType</span></span> | <span data-ttu-id="79490-117">string</span><span class="sxs-lookup"><span data-stu-id="79490-117">string</span></span>                  | <span data-ttu-id="79490-p103">ファイルの MIME の種類。これはサーバーのロジックによって決定されます。またファイルのアップロード時に指定された値でない場合があります。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="79490-p103">The MIME type for the file. This is determined by logic on the server and might not be the value provided when the file was uploaded. Read-only.</span></span> |

## <a name="remarks"></a><span data-ttu-id="79490-121">注釈</span><span class="sxs-lookup"><span data-stu-id="79490-121">Remarks</span></span> 

<span data-ttu-id="79490-122">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="79490-122">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The file facet describes properties of a file",
  "keywords": "file,item,facet",
  "section": "documentation",
  "tocPath": "Facets/File"
} -->
