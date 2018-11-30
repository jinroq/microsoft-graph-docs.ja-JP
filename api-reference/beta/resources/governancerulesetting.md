---
title: governanceRuleSetting リソースの種類
description: ロールの設定で構成されたルールを表します。
ms.openlocfilehash: 486b5163c59772c971cfc1d61a98817b7f0c16f5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070678"
---
# <a name="governancerulesetting-resource-type"></a><span data-ttu-id="b0126-103">governanceRuleSetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b0126-103">governanceRuleSetting resource type</span></span>

> <span data-ttu-id="b0126-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b0126-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b0126-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b0126-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b0126-106">ロールの設定で構成されたルールを表します。</span><span class="sxs-lookup"><span data-stu-id="b0126-106">Represents the rules that the role settings are composed of.</span></span>


## <a name="properties"></a><span data-ttu-id="b0126-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b0126-107">Properties</span></span>
|<span data-ttu-id="b0126-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b0126-108">Property</span></span>      | <span data-ttu-id="b0126-109">型</span><span class="sxs-lookup"><span data-stu-id="b0126-109">Type</span></span>         |<span data-ttu-id="b0126-110">説明</span><span class="sxs-lookup"><span data-stu-id="b0126-110">Description</span></span>|
|:-------------|:-------------|:----------|
|<span data-ttu-id="b0126-111">ruleIdentifier</span><span class="sxs-lookup"><span data-stu-id="b0126-111">ruleIdentifier</span></span>|<span data-ttu-id="b0126-112">String</span><span class="sxs-lookup"><span data-stu-id="b0126-112">String</span></span>        |<span data-ttu-id="b0126-113">ルールの id です。</span><span class="sxs-lookup"><span data-stu-id="b0126-113">The id of the rule.</span></span> <span data-ttu-id="b0126-114">たとえば、``ExpirationRule``と``MfaRule``。</span><span class="sxs-lookup"><span data-stu-id="b0126-114">For example, ``ExpirationRule`` and ``MfaRule``.</span></span>|
|<span data-ttu-id="b0126-115">setting</span><span class="sxs-lookup"><span data-stu-id="b0126-115">setting</span></span>       |<span data-ttu-id="b0126-116">String</span><span class="sxs-lookup"><span data-stu-id="b0126-116">String</span></span>        |<span data-ttu-id="b0126-117">ルールの設定をします。</span><span class="sxs-lookup"><span data-stu-id="b0126-117">The settings of the rule.</span></span> <span data-ttu-id="b0126-118">値は、Parameter_Name:Parameter_Value の形式でのペアの一覧を JSON 文字列です。</span><span class="sxs-lookup"><span data-stu-id="b0126-118">The value is a JSON string with a list of pairs in the format of Parameter_Name:Parameter_Value.</span></span> <span data-ttu-id="b0126-119">たとえば、`{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}` では、</span><span class="sxs-lookup"><span data-stu-id="b0126-119">For example, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b0126-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b0126-120">JSON representation</span></span>

<span data-ttu-id="b0126-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b0126-121">Here is a JSON representation of the resource.</span></span>

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