---
title: governanceRuleSetting リソースの種類
description: ロールの設定で構成されたルールを表します。
localization_priority: Normal
ms.openlocfilehash: bbb44760cf4b7377e5e5cc6dd312c2caee9897fa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522239"
---
# <a name="governancerulesetting-resource-type"></a><span data-ttu-id="24c12-103">governanceRuleSetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="24c12-103">governanceRuleSetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24c12-104">ロールの設定で構成されたルールを表します。</span><span class="sxs-lookup"><span data-stu-id="24c12-104">Represents the rules that the role settings are composed of.</span></span>


## <a name="properties"></a><span data-ttu-id="24c12-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24c12-105">Properties</span></span>
|<span data-ttu-id="24c12-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24c12-106">Property</span></span>      | <span data-ttu-id="24c12-107">型</span><span class="sxs-lookup"><span data-stu-id="24c12-107">Type</span></span>         |<span data-ttu-id="24c12-108">説明</span><span class="sxs-lookup"><span data-stu-id="24c12-108">Description</span></span>|
|:-------------|:-------------|:----------|
|<span data-ttu-id="24c12-109">ruleIdentifier</span><span class="sxs-lookup"><span data-stu-id="24c12-109">ruleIdentifier</span></span>|<span data-ttu-id="24c12-110">String</span><span class="sxs-lookup"><span data-stu-id="24c12-110">String</span></span>        |<span data-ttu-id="24c12-111">ルールの id です。</span><span class="sxs-lookup"><span data-stu-id="24c12-111">The id of the rule.</span></span> <span data-ttu-id="24c12-112">たとえば、``ExpirationRule``と``MfaRule``。</span><span class="sxs-lookup"><span data-stu-id="24c12-112">For example, ``ExpirationRule`` and ``MfaRule``.</span></span>|
|<span data-ttu-id="24c12-113">setting</span><span class="sxs-lookup"><span data-stu-id="24c12-113">setting</span></span>       |<span data-ttu-id="24c12-114">String</span><span class="sxs-lookup"><span data-stu-id="24c12-114">String</span></span>        |<span data-ttu-id="24c12-115">ルールの設定をします。</span><span class="sxs-lookup"><span data-stu-id="24c12-115">The settings of the rule.</span></span> <span data-ttu-id="24c12-116">値は、Parameter_Name:Parameter_Value の形式でのペアの一覧を JSON 文字列です。</span><span class="sxs-lookup"><span data-stu-id="24c12-116">The value is a JSON string with a list of pairs in the format of Parameter_Name:Parameter_Value.</span></span> <span data-ttu-id="24c12-117">たとえば、`{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}` のように指定します。</span><span class="sxs-lookup"><span data-stu-id="24c12-117">For example, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="24c12-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="24c12-118">JSON representation</span></span>

<span data-ttu-id="24c12-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="24c12-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.governanceRuleSetting"
}-->


```json
{
  "ruleIdentifier": "String",
  "setting": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRuleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governancerulesetting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
