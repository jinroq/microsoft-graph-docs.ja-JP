---
title: educationFileResource リソースの種類
description: EducationResource のサブクラスで、割り当てまたは送信に関連付けられているファイルオブジェクトを表します。  この例では、ファイルは特別なファイル (Word、Excel など) の1つではなく、システム内で特別な処理を行わないファイルです。 ファイルリソースは、このリソースが添付されている割り当てまたは送信に関連付けられている**Resourcefolder**に格納されている必要があります。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 678591d4c9662f1ab3fc68f7d35a0ec525c6e74f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972744"
---
# <a name="educationfileresource-resource-type"></a><span data-ttu-id="f32a6-105">educationFileResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f32a6-105">educationFileResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f32a6-106">[EducationResource](educationresource.md)のサブクラスで、割り当てまたは送信に関連付けられているファイルオブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="f32a6-106">A subclass of [educationResource](educationresource.md) that represents a file object that is associated with the assignment or submission.</span></span>  <span data-ttu-id="f32a6-107">この例では、ファイルは特別なファイル (Word、Excel など) の1つではなく、システム内で特別な処理を行わないファイルです。</span><span class="sxs-lookup"><span data-stu-id="f32a6-107">In this case, the file is not one of the special files (Word, Excel, and so on) but is a file that does not have special handling within the system.</span></span> <span data-ttu-id="f32a6-108">ファイルリソースは、このリソースが添付されている割り当てまたは送信に関連付けられている**Resourcefolder**に格納されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f32a6-108">The file resource must be stored in the **resourceFolder** that is associated with the assignment or submission this resource is attached to.</span></span>

## <a name="properties"></a><span data-ttu-id="f32a6-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f32a6-109">Properties</span></span>
| <span data-ttu-id="f32a6-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f32a6-110">Property</span></span>     | <span data-ttu-id="f32a6-111">型</span><span class="sxs-lookup"><span data-stu-id="f32a6-111">Type</span></span>   |<span data-ttu-id="f32a6-112">説明</span><span class="sxs-lookup"><span data-stu-id="f32a6-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f32a6-113">fileUrl</span><span class="sxs-lookup"><span data-stu-id="f32a6-113">fileUrl</span></span>|<span data-ttu-id="f32a6-114">String</span><span class="sxs-lookup"><span data-stu-id="f32a6-114">String</span></span>|<span data-ttu-id="f32a6-115">ファイルリソースのディスク上の場所です。</span><span class="sxs-lookup"><span data-stu-id="f32a6-115">Location on disk of the file resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f32a6-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f32a6-116">JSON representation</span></span>

<span data-ttu-id="f32a6-117">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f32a6-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFileResource"
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
  "description": "educationFileResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
