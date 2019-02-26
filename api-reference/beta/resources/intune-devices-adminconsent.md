---
title: adminconsent リソースの種類
description: 管理者の同意情報。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8f46e379a47bd7b08be1427115c785452543dfbf
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157940"
---
# <a name="adminconsent-resource-type"></a><span data-ttu-id="ffef5-103">adminconsent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ffef5-103">adminConsent resource type</span></span>

> <span data-ttu-id="ffef5-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ffef5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ffef5-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ffef5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ffef5-106">管理者の同意情報。</span><span class="sxs-lookup"><span data-stu-id="ffef5-106">Admin consent information.</span></span>

## <a name="properties"></a><span data-ttu-id="ffef5-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ffef5-107">Properties</span></span>
|<span data-ttu-id="ffef5-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ffef5-108">Property</span></span>|<span data-ttu-id="ffef5-109">型</span><span class="sxs-lookup"><span data-stu-id="ffef5-109">Type</span></span>|<span data-ttu-id="ffef5-110">説明</span><span class="sxs-lookup"><span data-stu-id="ffef5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffef5-111">/sharepoint データの編集</span><span class="sxs-lookup"><span data-stu-id="ffef5-111">shareAPNSData</span></span>|[<span data-ttu-id="ffef5-112">adminconの状態</span><span class="sxs-lookup"><span data-stu-id="ffef5-112">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="ffef5-113">ユーザーとデバイスのデータを Apple に共有するための管理者の同意状態。</span><span class="sxs-lookup"><span data-stu-id="ffef5-113">The admin consent state of sharing user and device data to Apple.</span></span> <span data-ttu-id="ffef5-114">可能な値は、`notConfigured`、`granted`、`notGranted` です。</span><span class="sxs-lookup"><span data-stu-id="ffef5-114">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ffef5-115">関係</span><span class="sxs-lookup"><span data-stu-id="ffef5-115">Relationships</span></span>
<span data-ttu-id="ffef5-116">なし</span><span class="sxs-lookup"><span data-stu-id="ffef5-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ffef5-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ffef5-117">JSON Representation</span></span>
<span data-ttu-id="ffef5-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ffef5-118">Here is a JSON representation of the resource.</span></span>
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




