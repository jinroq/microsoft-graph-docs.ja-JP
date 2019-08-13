---
title: adminConsent リソースの種類
description: 管理者の同意情報。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8d78333cd683501a8bf4fea0aa3a2e55944d9b5a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36319309"
---
# <a name="adminconsent-resource-type"></a><span data-ttu-id="c3a1a-103">adminConsent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c3a1a-103">adminConsent resource type</span></span>

> <span data-ttu-id="c3a1a-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3a1a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3a1a-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c3a1a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3a1a-106">管理者の同意情報。</span><span class="sxs-lookup"><span data-stu-id="c3a1a-106">Admin consent information.</span></span>

## <a name="properties"></a><span data-ttu-id="c3a1a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c3a1a-107">Properties</span></span>
|<span data-ttu-id="c3a1a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c3a1a-108">Property</span></span>|<span data-ttu-id="c3a1a-109">型</span><span class="sxs-lookup"><span data-stu-id="c3a1a-109">Type</span></span>|<span data-ttu-id="c3a1a-110">説明</span><span class="sxs-lookup"><span data-stu-id="c3a1a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3a1a-111">/Sharepoint データの編集</span><span class="sxs-lookup"><span data-stu-id="c3a1a-111">shareAPNSData</span></span>|[<span data-ttu-id="c3a1a-112">Adminconの状態</span><span class="sxs-lookup"><span data-stu-id="c3a1a-112">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="c3a1a-113">ユーザーとデバイスのデータを Apple に共有するための管理者の同意状態。</span><span class="sxs-lookup"><span data-stu-id="c3a1a-113">The admin consent state of sharing user and device data to Apple.</span></span> <span data-ttu-id="c3a1a-114">可能な値は、`notConfigured`、`granted`、`notGranted` です。</span><span class="sxs-lookup"><span data-stu-id="c3a1a-114">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|
|<span data-ttu-id="c3a1a-115">shareUserExperienceAnalyticsData</span><span class="sxs-lookup"><span data-stu-id="c3a1a-115">shareUserExperienceAnalyticsData</span></span>|[<span data-ttu-id="c3a1a-116">Adminconの状態</span><span class="sxs-lookup"><span data-stu-id="c3a1a-116">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="c3a1a-117">ユーザー環境分析データの共有に関する管理者の同意を取得または設定します。</span><span class="sxs-lookup"><span data-stu-id="c3a1a-117">Gets or sets the admin consent for sharing User experience analytics data.</span></span> <span data-ttu-id="c3a1a-118">可能な値は、`notConfigured`、`granted`、`notGranted` です。</span><span class="sxs-lookup"><span data-stu-id="c3a1a-118">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3a1a-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c3a1a-119">Relationships</span></span>
<span data-ttu-id="c3a1a-120">なし</span><span class="sxs-lookup"><span data-stu-id="c3a1a-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3a1a-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c3a1a-121">JSON Representation</span></span>
<span data-ttu-id="c3a1a-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c3a1a-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.adminConsent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.adminConsent",
  "shareAPNSData": "String",
  "shareUserExperienceAnalyticsData": "String"
}
```



