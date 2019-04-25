---
title: governanceRuleSetting リソースの種類
description: ロール設定が構成されているルールを表します。
localization_priority: Normal
ms.openlocfilehash: bbb44760cf4b7377e5e5cc6dd312c2caee9897fa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547460"
---
# <a name="governancerulesetting-resource-type"></a><span data-ttu-id="777c8-103">governanceRuleSetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="777c8-103">governanceRuleSetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="777c8-104">ロール設定が構成されているルールを表します。</span><span class="sxs-lookup"><span data-stu-id="777c8-104">Represents the rules that the role settings are composed of.</span></span>


## <a name="properties"></a><span data-ttu-id="777c8-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="777c8-105">Properties</span></span>
|<span data-ttu-id="777c8-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="777c8-106">Property</span></span>      | <span data-ttu-id="777c8-107">型</span><span class="sxs-lookup"><span data-stu-id="777c8-107">Type</span></span>         |<span data-ttu-id="777c8-108">説明</span><span class="sxs-lookup"><span data-stu-id="777c8-108">Description</span></span>|
|:-------------|:-------------|:----------|
|<span data-ttu-id="777c8-109">ruleIdentifier</span><span class="sxs-lookup"><span data-stu-id="777c8-109">ruleIdentifier</span></span>|<span data-ttu-id="777c8-110">String</span><span class="sxs-lookup"><span data-stu-id="777c8-110">String</span></span>        |<span data-ttu-id="777c8-111">ルールの id。</span><span class="sxs-lookup"><span data-stu-id="777c8-111">The id of the rule.</span></span> <span data-ttu-id="777c8-112">たとえば、 ``ExpirationRule``と``MfaRule``のようになります。</span><span class="sxs-lookup"><span data-stu-id="777c8-112">For example, ``ExpirationRule`` and ``MfaRule``.</span></span>|
|<span data-ttu-id="777c8-113">setting</span><span class="sxs-lookup"><span data-stu-id="777c8-113">setting</span></span>       |<span data-ttu-id="777c8-114">String</span><span class="sxs-lookup"><span data-stu-id="777c8-114">String</span></span>        |<span data-ttu-id="777c8-115">ルールの設定。</span><span class="sxs-lookup"><span data-stu-id="777c8-115">The settings of the rule.</span></span> <span data-ttu-id="777c8-116">この値は、Parameter_Name: Parameter_Value という形式のペアのリストを含む JSON 文字列です。</span><span class="sxs-lookup"><span data-stu-id="777c8-116">The value is a JSON string with a list of pairs in the format of Parameter_Name:Parameter_Value.</span></span> <span data-ttu-id="777c8-117">たとえば、`{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}` のように指定します。</span><span class="sxs-lookup"><span data-stu-id="777c8-117">For example, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="777c8-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="777c8-118">JSON representation</span></span>

<span data-ttu-id="777c8-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="777c8-119">Here is a JSON representation of the resource.</span></span>

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
