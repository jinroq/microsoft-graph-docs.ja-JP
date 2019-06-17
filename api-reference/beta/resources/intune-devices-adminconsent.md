---
title: adminConsent リソースの種類
description: 管理者の同意情報。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a25dd46c8f1f8efdc3149472dae88910774e44a9
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983373"
---
# <a name="adminconsent-resource-type"></a><span data-ttu-id="15667-103">adminConsent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="15667-103">adminConsent resource type</span></span>

> <span data-ttu-id="15667-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15667-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15667-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="15667-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15667-106">管理者の同意情報。</span><span class="sxs-lookup"><span data-stu-id="15667-106">Admin consent information.</span></span>

## <a name="properties"></a><span data-ttu-id="15667-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="15667-107">Properties</span></span>
|<span data-ttu-id="15667-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="15667-108">Property</span></span>|<span data-ttu-id="15667-109">型</span><span class="sxs-lookup"><span data-stu-id="15667-109">Type</span></span>|<span data-ttu-id="15667-110">説明</span><span class="sxs-lookup"><span data-stu-id="15667-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15667-111">/Sharepoint データの編集</span><span class="sxs-lookup"><span data-stu-id="15667-111">shareAPNSData</span></span>|[<span data-ttu-id="15667-112">Adminconの状態</span><span class="sxs-lookup"><span data-stu-id="15667-112">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="15667-113">ユーザーとデバイスのデータを Apple に共有するための管理者の同意状態。</span><span class="sxs-lookup"><span data-stu-id="15667-113">The admin consent state of sharing user and device data to Apple.</span></span> <span data-ttu-id="15667-114">可能な値は、`notConfigured`、`granted`、`notGranted` です。</span><span class="sxs-lookup"><span data-stu-id="15667-114">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="15667-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="15667-115">Relationships</span></span>
<span data-ttu-id="15667-116">なし</span><span class="sxs-lookup"><span data-stu-id="15667-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="15667-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="15667-117">JSON Representation</span></span>
<span data-ttu-id="15667-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="15667-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.adminConsent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.adminConsent",
  "shareAPNSData": "String"
}
```





