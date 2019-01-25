---
title: educationWordResource リソースの種類
description: 'EducationResource のサブクラスです。 これは、Word ドキュメント リソースです。 関連付けられている**fileResource**ディレクトリに Word ファイルをアップロードする必要があります、 '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9d92b993ab920a894590346bf5fde0ff86c73e8d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529671"
---
# <a name="educationwordresource-resource-type"></a><span data-ttu-id="d40b1-105">educationWordResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d40b1-105">educationWordResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d40b1-106">[EducationResource](educationresource.md)のサブクラスです。</span><span class="sxs-lookup"><span data-stu-id="d40b1-106">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="d40b1-107">これは、Word ドキュメント リソースです。</span><span class="sxs-lookup"><span data-stu-id="d40b1-107">This is a Word document resource.</span></span> <span data-ttu-id="d40b1-108">Word ファイルを送信または割り当てに関連付けられている**fileResource**ディレクトリにアップロードする必要があります。</span><span class="sxs-lookup"><span data-stu-id="d40b1-108">The Word file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="d40b1-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d40b1-109">Properties</span></span>
| <span data-ttu-id="d40b1-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d40b1-110">Property</span></span>     | <span data-ttu-id="d40b1-111">型</span><span class="sxs-lookup"><span data-stu-id="d40b1-111">Type</span></span>   |<span data-ttu-id="d40b1-112">説明</span><span class="sxs-lookup"><span data-stu-id="d40b1-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d40b1-113">FileURL</span><span class="sxs-lookup"><span data-stu-id="d40b1-113">fileUrl</span></span>|<span data-ttu-id="d40b1-114">String</span><span class="sxs-lookup"><span data-stu-id="d40b1-114">String</span></span>|<span data-ttu-id="d40b1-115">ディスク上のファイルの場所です。</span><span class="sxs-lookup"><span data-stu-id="d40b1-115">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d40b1-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d40b1-116">JSON representation</span></span>

<span data-ttu-id="d40b1-117">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d40b1-117">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/educationwordresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
