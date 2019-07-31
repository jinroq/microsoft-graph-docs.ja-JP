---
title: educationPowerPointResource リソースの種類
description: 'EducationResource のサブクラス。 これは PowerPoint リソースです。 PowerPoint ファイルは、に関連付けられた**fileResource**ディレクトリにアップロードする必要があります。 '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 72ab3435ed30602bbd9b2fadf9a6f4d0879e9198
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972605"
---
# <a name="educationpowerpointresource-resource-type"></a><span data-ttu-id="ba9f6-105">educationPowerPointResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ba9f6-105">educationPowerPointResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba9f6-106">[EducationResource](educationresource.md)のサブクラス。</span><span class="sxs-lookup"><span data-stu-id="ba9f6-106">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="ba9f6-107">これは PowerPoint リソースです。</span><span class="sxs-lookup"><span data-stu-id="ba9f6-107">This is a PowerPoint resource.</span></span> <span data-ttu-id="ba9f6-108">PowerPoint ファイルは、割り当てまたは送信に関連付けられている**fileResource**ディレクトリにアップロードする必要があります。</span><span class="sxs-lookup"><span data-stu-id="ba9f6-108">The PowerPoint file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="ba9f6-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ba9f6-109">Properties</span></span>
| <span data-ttu-id="ba9f6-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ba9f6-110">Property</span></span>     | <span data-ttu-id="ba9f6-111">型</span><span class="sxs-lookup"><span data-stu-id="ba9f6-111">Type</span></span>   |<span data-ttu-id="ba9f6-112">説明</span><span class="sxs-lookup"><span data-stu-id="ba9f6-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ba9f6-113">fileUrl</span><span class="sxs-lookup"><span data-stu-id="ba9f6-113">fileUrl</span></span>|<span data-ttu-id="ba9f6-114">String</span><span class="sxs-lookup"><span data-stu-id="ba9f6-114">String</span></span>|<span data-ttu-id="ba9f6-115">ディスク上のファイルの場所。</span><span class="sxs-lookup"><span data-stu-id="ba9f6-115">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ba9f6-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ba9f6-116">JSON representation</span></span>

<span data-ttu-id="ba9f6-117">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ba9f6-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationPowerPointResource"
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
  "description": "educationPowerPointResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
