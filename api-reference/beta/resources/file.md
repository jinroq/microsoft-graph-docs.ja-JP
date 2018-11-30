---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: File
ms.openlocfilehash: bd0cd6ea5f5ee2225392aa61c2dda9b30e2ffbca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072530"
---
# <a name="file-resource-type"></a><span data-ttu-id="9ed68-102">ファイル リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9ed68-102">File resource type</span></span>

> <span data-ttu-id="9ed68-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9ed68-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9ed68-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ed68-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9ed68-105">**ファイル** リソースは、ファイル関連のデータ項目を 1 つの構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="9ed68-105">The **File** resource groups file-related data items into a single structure.</span></span>

<span data-ttu-id="9ed68-p102">[**DriveItem**](driveitem.md) に null 以外の**ファイル** ファセットがある場合は、項目はファイルを表します。他のプロパティに加えて、ファイルにはファイルのバイト ストリームを含む**コンテンツ**関係があります。</span><span class="sxs-lookup"><span data-stu-id="9ed68-p102">If a [**DriveItem**](driveitem.md) has a non-null **file** facet, the item represents an file. In addition to other properties, files have a **content** relationship which contains the byte stream of the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9ed68-108">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9ed68-108">JSON representation</span></span>

<span data-ttu-id="9ed68-109">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9ed68-109">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="9ed68-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9ed68-110">Properties</span></span>

| <span data-ttu-id="9ed68-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9ed68-111">Property</span></span> | <span data-ttu-id="9ed68-112">型</span><span class="sxs-lookup"><span data-stu-id="9ed68-112">Type</span></span>                    | <span data-ttu-id="9ed68-113">説明</span><span class="sxs-lookup"><span data-stu-id="9ed68-113">Description</span></span>                                                                                                                                      |
|:---------|:------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="9ed68-114">hashes</span><span class="sxs-lookup"><span data-stu-id="9ed68-114">hashes</span></span>   | [<span data-ttu-id="9ed68-115">HashesType</span><span class="sxs-lookup"><span data-stu-id="9ed68-115">HashesType</span></span>](hashes.md) | <span data-ttu-id="9ed68-p103">ファイルのバイナリ コンテンツのハッシュ (利用可能な場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9ed68-p103">Hashes of the file's binary content, if available. Read-only.</span></span>                                                                                    |
| <span data-ttu-id="9ed68-118">mimeType</span><span class="sxs-lookup"><span data-stu-id="9ed68-118">mimeType</span></span> | <span data-ttu-id="9ed68-119">文字列</span><span class="sxs-lookup"><span data-stu-id="9ed68-119">string</span></span>                  | <span data-ttu-id="9ed68-p104">ファイルの MIME の種類。これはサーバーのロジックによって決定されます。またファイルのアップロード時に指定された値でない場合があります。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9ed68-p104">The MIME type for the file. This is determined by logic on the server and might not be the value provided when the file was uploaded. Read-only.</span></span> |

## <a name="remarks"></a><span data-ttu-id="9ed68-123">注釈</span><span class="sxs-lookup"><span data-stu-id="9ed68-123">Remarks</span></span> 

<span data-ttu-id="9ed68-124">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ed68-124">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The file facet describes properties of a file",
  "keywords": "file,item,facet",
  "section": "documentation",
  "tocPath": "Facets/File"
} -->
