---
title: educationWordResource リソースの種類
description: 'educationResource のサブクラス。 これは Word ドキュメントリソースです。 Word ファイルは、に関連付けられた**fileResource**ディレクトリにアップロードする必要があります。 '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9bd9af22c141991efd85fc240a002b5c7a0eac3b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340204"
---
# <a name="educationwordresource-resource-type"></a><span data-ttu-id="291ed-105">educationWordResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="291ed-105">educationWordResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="291ed-106">[educationResource](educationresource.md)のサブクラス。</span><span class="sxs-lookup"><span data-stu-id="291ed-106">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="291ed-107">これは Word ドキュメントリソースです。</span><span class="sxs-lookup"><span data-stu-id="291ed-107">This is a Word document resource.</span></span> <span data-ttu-id="291ed-108">Word ファイルは、割り当てまたは送信に関連付けられている**fileResource**ディレクトリにアップロードする必要があります。</span><span class="sxs-lookup"><span data-stu-id="291ed-108">The Word file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="291ed-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="291ed-109">Properties</span></span>
| <span data-ttu-id="291ed-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="291ed-110">Property</span></span>     | <span data-ttu-id="291ed-111">型</span><span class="sxs-lookup"><span data-stu-id="291ed-111">Type</span></span>   |<span data-ttu-id="291ed-112">説明</span><span class="sxs-lookup"><span data-stu-id="291ed-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="291ed-113">fileUrl</span><span class="sxs-lookup"><span data-stu-id="291ed-113">fileUrl</span></span>|<span data-ttu-id="291ed-114">String</span><span class="sxs-lookup"><span data-stu-id="291ed-114">String</span></span>|<span data-ttu-id="291ed-115">ディスク上のファイルの場所。</span><span class="sxs-lookup"><span data-stu-id="291ed-115">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="291ed-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="291ed-116">JSON representation</span></span>

<span data-ttu-id="291ed-117">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="291ed-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationWordResource"
}-->

```json
{
  "fileUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationWordResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
