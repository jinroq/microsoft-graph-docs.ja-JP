---
title: adminConsent リソースの種類
description: 管理者の同意情報。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7f13e8abbaf20f57e94923918a4e5c2bb5bcf9b9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968611"
---
# <a name="adminconsent-resource-type"></a><span data-ttu-id="1d3bd-103">adminConsent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1d3bd-103">adminConsent resource type</span></span>

> <span data-ttu-id="1d3bd-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d3bd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d3bd-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1d3bd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d3bd-106">管理者の同意情報。</span><span class="sxs-lookup"><span data-stu-id="1d3bd-106">Admin consent information.</span></span>

## <a name="properties"></a><span data-ttu-id="1d3bd-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d3bd-107">Properties</span></span>
|<span data-ttu-id="1d3bd-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d3bd-108">Property</span></span>|<span data-ttu-id="1d3bd-109">型</span><span class="sxs-lookup"><span data-stu-id="1d3bd-109">Type</span></span>|<span data-ttu-id="1d3bd-110">説明</span><span class="sxs-lookup"><span data-stu-id="1d3bd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d3bd-111">/Sharepoint データの編集</span><span class="sxs-lookup"><span data-stu-id="1d3bd-111">shareAPNSData</span></span>|[<span data-ttu-id="1d3bd-112">Adminconの状態</span><span class="sxs-lookup"><span data-stu-id="1d3bd-112">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="1d3bd-113">ユーザーとデバイスのデータを Apple に共有するための管理者の同意状態。</span><span class="sxs-lookup"><span data-stu-id="1d3bd-113">The admin consent state of sharing user and device data to Apple.</span></span> <span data-ttu-id="1d3bd-114">可能な値は、`notConfigured`、`granted`、`notGranted` です。</span><span class="sxs-lookup"><span data-stu-id="1d3bd-114">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d3bd-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1d3bd-115">Relationships</span></span>
<span data-ttu-id="1d3bd-116">なし</span><span class="sxs-lookup"><span data-stu-id="1d3bd-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d3bd-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1d3bd-117">JSON Representation</span></span>
<span data-ttu-id="1d3bd-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1d3bd-118">Here is a JSON representation of the resource.</span></span>
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





