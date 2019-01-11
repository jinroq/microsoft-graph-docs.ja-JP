---
title: governanceRuleSetting リソースの種類
description: ロールの設定で構成されたルールを表します。
localization_priority: Normal
ms.openlocfilehash: 7554c96daec70a95cde5ab0c3faedfba74764cff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894258"
---
# <a name="governancerulesetting-resource-type"></a><span data-ttu-id="0fafb-103">governanceRuleSetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0fafb-103">governanceRuleSetting resource type</span></span>

> <span data-ttu-id="0fafb-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0fafb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0fafb-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0fafb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0fafb-106">ロールの設定で構成されたルールを表します。</span><span class="sxs-lookup"><span data-stu-id="0fafb-106">Represents the rules that the role settings are composed of.</span></span>


## <a name="properties"></a><span data-ttu-id="0fafb-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0fafb-107">Properties</span></span>
|<span data-ttu-id="0fafb-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0fafb-108">Property</span></span>      | <span data-ttu-id="0fafb-109">種類</span><span class="sxs-lookup"><span data-stu-id="0fafb-109">Type</span></span>         |<span data-ttu-id="0fafb-110">説明</span><span class="sxs-lookup"><span data-stu-id="0fafb-110">Description</span></span>|
|:-------------|:-------------|:----------|
|<span data-ttu-id="0fafb-111">ruleIdentifier</span><span class="sxs-lookup"><span data-stu-id="0fafb-111">ruleIdentifier</span></span>|<span data-ttu-id="0fafb-112">String</span><span class="sxs-lookup"><span data-stu-id="0fafb-112">String</span></span>        |<span data-ttu-id="0fafb-113">ルールの id です。</span><span class="sxs-lookup"><span data-stu-id="0fafb-113">The id of the rule.</span></span> <span data-ttu-id="0fafb-114">たとえば、``ExpirationRule``と``MfaRule``。</span><span class="sxs-lookup"><span data-stu-id="0fafb-114">For example, ``ExpirationRule`` and ``MfaRule``.</span></span>|
|<span data-ttu-id="0fafb-115">setting</span><span class="sxs-lookup"><span data-stu-id="0fafb-115">setting</span></span>       |<span data-ttu-id="0fafb-116">String</span><span class="sxs-lookup"><span data-stu-id="0fafb-116">String</span></span>        |<span data-ttu-id="0fafb-117">ルールの設定をします。</span><span class="sxs-lookup"><span data-stu-id="0fafb-117">The settings of the rule.</span></span> <span data-ttu-id="0fafb-118">値は、Parameter_Name:Parameter_Value の形式でのペアの一覧を JSON 文字列です。</span><span class="sxs-lookup"><span data-stu-id="0fafb-118">The value is a JSON string with a list of pairs in the format of Parameter_Name:Parameter_Value.</span></span> <span data-ttu-id="0fafb-119">たとえば、`{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}` では、</span><span class="sxs-lookup"><span data-stu-id="0fafb-119">For example, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0fafb-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0fafb-120">JSON representation</span></span>

<span data-ttu-id="0fafb-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0fafb-121">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "governanceRuleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
