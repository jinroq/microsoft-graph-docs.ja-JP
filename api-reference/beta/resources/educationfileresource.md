---
title: educationFileResource リソースの種類
description: 送信または割り当てに関連付けられているファイル オブジェクトを表す educationResource のサブクラスです。  この例では、ファイルは特別なファイル (Word、Excel、およびなど) のいずれかがファイル システム内で特別な処理がないです。 このリソースに接続されている送信または割り当てに関連付けられている**resourceFolder**では、ファイル リソースを格納してください。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 15ca31576618f15e64b85d860077785160c25989
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520796"
---
# <a name="educationfileresource-resource-type"></a><span data-ttu-id="9ece7-105">educationFileResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9ece7-105">educationFileResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ece7-106">送信または割り当てに関連付けられているファイル オブジェクトを表す[educationResource](educationresource.md)のサブクラスです。</span><span class="sxs-lookup"><span data-stu-id="9ece7-106">A subclass of [educationResource](educationresource.md) that represents a file object that is associated with the assignment or submission.</span></span>  <span data-ttu-id="9ece7-107">この例では、ファイルは特別なファイル (Word、Excel、およびなど) のいずれかがファイル システム内で特別な処理がないです。</span><span class="sxs-lookup"><span data-stu-id="9ece7-107">In this case, the file is not one of the special files (Word, Excel, and so on) but is a file that does not have special handling within the system.</span></span> <span data-ttu-id="9ece7-108">このリソースに接続されている送信または割り当てに関連付けられている**resourceFolder**では、ファイル リソースを格納してください。</span><span class="sxs-lookup"><span data-stu-id="9ece7-108">The file resource must be stored in the **resourceFolder** that is associated with the assignment or submission this resource is attached to.</span></span>

## <a name="properties"></a><span data-ttu-id="9ece7-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9ece7-109">Properties</span></span>
| <span data-ttu-id="9ece7-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9ece7-110">Property</span></span>     | <span data-ttu-id="9ece7-111">型</span><span class="sxs-lookup"><span data-stu-id="9ece7-111">Type</span></span>   |<span data-ttu-id="9ece7-112">説明</span><span class="sxs-lookup"><span data-stu-id="9ece7-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9ece7-113">FileURL</span><span class="sxs-lookup"><span data-stu-id="9ece7-113">fileUrl</span></span>|<span data-ttu-id="9ece7-114">String</span><span class="sxs-lookup"><span data-stu-id="9ece7-114">String</span></span>|<span data-ttu-id="9ece7-115">ファイル リソースのディスク上の場所です。</span><span class="sxs-lookup"><span data-stu-id="9ece7-115">Location on disk of the file resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9ece7-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9ece7-116">JSON representation</span></span>

<span data-ttu-id="9ece7-117">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9ece7-117">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/educationfileresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
