---
title: governanceRuleSetting リソースの種類
description: ロール設定が構成されているルールを表します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: bfc3bb7895a3ec66a32456b48901fc456d3c3b2e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971873"
---
# <a name="governancerulesetting-resource-type"></a><span data-ttu-id="68614-103">governanceRuleSetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="68614-103">governanceRuleSetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68614-104">ロール設定が構成されているルールを表します。</span><span class="sxs-lookup"><span data-stu-id="68614-104">Represents the rules that the role settings are composed of.</span></span>


## <a name="properties"></a><span data-ttu-id="68614-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="68614-105">Properties</span></span>
|<span data-ttu-id="68614-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="68614-106">Property</span></span>      | <span data-ttu-id="68614-107">型</span><span class="sxs-lookup"><span data-stu-id="68614-107">Type</span></span>         |<span data-ttu-id="68614-108">説明</span><span class="sxs-lookup"><span data-stu-id="68614-108">Description</span></span>|
|:-------------|:-------------|:----------|
|<span data-ttu-id="68614-109">ruleIdentifier</span><span class="sxs-lookup"><span data-stu-id="68614-109">ruleIdentifier</span></span>|<span data-ttu-id="68614-110">String</span><span class="sxs-lookup"><span data-stu-id="68614-110">String</span></span>        |<span data-ttu-id="68614-111">ルールの id。</span><span class="sxs-lookup"><span data-stu-id="68614-111">The id of the rule.</span></span> <span data-ttu-id="68614-112">たとえば、 ``ExpirationRule``と``MfaRule``のようになります。</span><span class="sxs-lookup"><span data-stu-id="68614-112">For example, ``ExpirationRule`` and ``MfaRule``.</span></span>|
|<span data-ttu-id="68614-113">setting</span><span class="sxs-lookup"><span data-stu-id="68614-113">setting</span></span>       |<span data-ttu-id="68614-114">String</span><span class="sxs-lookup"><span data-stu-id="68614-114">String</span></span>        |<span data-ttu-id="68614-115">ルールの設定。</span><span class="sxs-lookup"><span data-stu-id="68614-115">The settings of the rule.</span></span> <span data-ttu-id="68614-116">この値は、Parameter_Name: Parameter_Value という形式のペアのリストを含む JSON 文字列です。</span><span class="sxs-lookup"><span data-stu-id="68614-116">The value is a JSON string with a list of pairs in the format of Parameter_Name:Parameter_Value.</span></span> <span data-ttu-id="68614-117">たとえば、`{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}` のように指定します。</span><span class="sxs-lookup"><span data-stu-id="68614-117">For example, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="68614-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="68614-118">JSON representation</span></span>

<span data-ttu-id="68614-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="68614-119">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
