---
title: hybridAgentUpdaterConfiguration リソースの種類
description: hybridAgentUpdaterConfiguration リソースの種類。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5c3efdd55f432add28f6d13797a0f73b4458b966
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841249"
---
# <a name="hybridagentupdaterconfiguration-resource-type"></a><span data-ttu-id="341b1-103">hybridAgentUpdaterConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="341b1-103">hybridAgentUpdaterConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="341b1-104">テナント管理者は、各 onPremisesPublishingProfile に対して、エージェントが更新を受信したり、エージェントに対して更新プログラムを適用したりできる時間枠を構成できます。</span><span class="sxs-lookup"><span data-stu-id="341b1-104">A tenant admin can configure for each onPremisesPublishingProfile the time window during which agents can receive updates or defer updates to the agents.</span></span> <span data-ttu-id="341b1-105">OnPremisesPublishingProfile に対して指定された hybridAgentUpdaterConfiguration は、その onPremisesPublishingProfile 内のすべてのエージェントに適用されます。</span><span class="sxs-lookup"><span data-stu-id="341b1-105">The hybridAgentUpdaterConfiguration specified for an onPremisesPublishingProfile is applicable to all the agents within that onPremisesPublishingProfile.</span></span>

<span data-ttu-id="341b1-106">たとえば、onPremisesPublishingProfile のエージェントの種類が "プロビジョニング" の場合、手順は次のようになります。</span><span class="sxs-lookup"><span data-stu-id="341b1-106">For example, for the agents in onPremisesPublishingProfile of type "provisioning" the steps could be as below.</span></span>

1) <span data-ttu-id="341b1-107">テナント管理者は、次の n 日間、プロビジョニングエージェントの更新を受信しないように構成できます。</span><span class="sxs-lookup"><span data-stu-id="341b1-107">Tenant administrator can configure to not receive any updates to the Provisioning agents for the next n days.</span></span>
2) <span data-ttu-id="341b1-108">テナント管理者は、エージェントが更新を recive できる更新ウィンドウ (開始時刻と終了時刻) を構成できます。</span><span class="sxs-lookup"><span data-stu-id="341b1-108">Tenant administrator can configure an update window(start and end time) during which the agents can recive updates.</span></span>
3) <span data-ttu-id="341b1-109">テナント管理者は、allowUpdateConfigurationOverride をプロビジョニングするために updater configutration を上書きし、次に使用可能な更新プログラムを受信するために alows を有効にすることができます。</span><span class="sxs-lookup"><span data-stu-id="341b1-109">Tenant administrator can enable allowUpdateConfigurationOverride which overrides the updater configutration for Provisioning agents and alows them to receive the next available update.</span></span>

<span data-ttu-id="341b1-110">Updater 構成で指定された DateTime/Time 情報は、evaluvation 中にエージェントによって報告されるローカルタイムゾーンに変換されます。</span><span class="sxs-lookup"><span data-stu-id="341b1-110">The DateTime/Time information specified in the updater configuration will be converted to the local timezone reported by the agent during evaluvation.</span></span>

<span data-ttu-id="341b1-111">エージェントの更新は、以下の優先順位の一覧に従います。</span><span class="sxs-lookup"><span data-stu-id="341b1-111">The update of the agent will follow the below priority list</span></span>

1) <span data-ttu-id="341b1-112">AllowUpdateConfigurationOverride が true に設定されている場合、テナントによって設定された updater 構成はスキップされ、エージェントの次のバージョンが利用可能になったとき (優先度 1) に更新が送信されます。</span><span class="sxs-lookup"><span data-stu-id="341b1-112">If allowUpdateConfigurationOverride is set to true the updater configuration set by the tenant will be skipped and the agent will receive an update when the next version of the agent is available (priority 1).</span></span>
2) <span data-ttu-id="341b1-113">延期更新が設定されている場合は、更新日時 (優先度 2) までエージェントは更新されません。</span><span class="sxs-lookup"><span data-stu-id="341b1-113">If the defer update is set, the agent will not be updated until the defer update date time (priority 2).</span></span>
3) <span data-ttu-id="341b1-114">[更新] ウィンドウが設定されている場合、エージェントはその時間枠に1日24時間 (優先度 3) でのみ更新されます。</span><span class="sxs-lookup"><span data-stu-id="341b1-114">If the update window is set, the agent will be updated only during that time window in a 24 hour day (priority 3).</span></span>
4) <span data-ttu-id="341b1-115">有効な updater 構成がテナントによって設定されていない場合は、エージェントの次のバージョンが利用可能になったときに更新が受信されます。</span><span class="sxs-lookup"><span data-stu-id="341b1-115">If no valid updater configuration is set by the tenant, the agent will receive an update when the next version of the agent is available</span></span>

## <a name="properties"></a><span data-ttu-id="341b1-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="341b1-116">Properties</span></span>

| <span data-ttu-id="341b1-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="341b1-117">Property</span></span>     | <span data-ttu-id="341b1-118">型</span><span class="sxs-lookup"><span data-stu-id="341b1-118">Type</span></span>        | <span data-ttu-id="341b1-119">説明</span><span class="sxs-lookup"><span data-stu-id="341b1-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="341b1-120">allowUpdateConfigurationOverride</span><span class="sxs-lookup"><span data-stu-id="341b1-120">allowUpdateConfigurationOverride</span></span>|<span data-ttu-id="341b1-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="341b1-121">Boolean</span></span>|<span data-ttu-id="341b1-122">更新プログラムがスキップされ、エージェントの次のバージョンが利用可能になったときにエージェントが更新を受信するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="341b1-122">Indicates if updater configuration will be skipped and the agent will receive an update when the next version of the agent is available.</span></span>|
|<span data-ttu-id="341b1-123">deferUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="341b1-123">deferUpdateDateTime</span></span>|<span data-ttu-id="341b1-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="341b1-124">DateTimeOffset</span></span>|<span data-ttu-id="341b1-p102">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="341b1-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="341b1-127">updateWindow</span><span class="sxs-lookup"><span data-stu-id="341b1-127">updateWindow</span></span>|[<span data-ttu-id="341b1-128">updateWindow</span><span class="sxs-lookup"><span data-stu-id="341b1-128">updateWindow</span></span>](updatewindow.md)||

## <a name="json-representation"></a><span data-ttu-id="341b1-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="341b1-129">JSON representation</span></span>

<span data-ttu-id="341b1-130">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="341b1-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.hybridAgentUpdaterConfiguration",
  "baseType": null
}-->

```json
{
  "allowUpdateConfigurationOverride": true,
  "deferUpdateDateTime": "String (timestamp)",
  "updateWindow": {"@odata.type": "microsoft.graph.updateWindow"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "hybridAgentUpdaterConfiguration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
