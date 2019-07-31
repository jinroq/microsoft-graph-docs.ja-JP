---
title: Macosvppapp割り当て設定リソースの種類
description: グループへの Mac VPP モバイルアプリの割り当てに使用されるプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 446e46cab832609073a80ee171decbb668014338
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005409"
---
# <a name="macosvppappassignmentsettings-resource-type"></a><span data-ttu-id="68c69-103">Macosvppapp割り当て設定リソースの種類</span><span class="sxs-lookup"><span data-stu-id="68c69-103">macOsVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="68c69-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="68c69-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68c69-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="68c69-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68c69-106">グループへの Mac VPP モバイルアプリの割り当てに使用されるプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="68c69-106">Contains properties used to assign an Mac VPP mobile app to a group.</span></span>


<span data-ttu-id="68c69-107">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="68c69-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="68c69-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="68c69-108">Properties</span></span>
|<span data-ttu-id="68c69-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="68c69-109">Property</span></span>|<span data-ttu-id="68c69-110">型</span><span class="sxs-lookup"><span data-stu-id="68c69-110">Type</span></span>|<span data-ttu-id="68c69-111">説明</span><span class="sxs-lookup"><span data-stu-id="68c69-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68c69-112">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="68c69-112">useDeviceLicensing</span></span>|<span data-ttu-id="68c69-113">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="68c69-113">Boolean</span></span>|<span data-ttu-id="68c69-114">デバイスのライセンスを使用するかどうか。</span><span class="sxs-lookup"><span data-stu-id="68c69-114">Whether or not to use device licensing.</span></span>|

## <a name="relationships"></a><span data-ttu-id="68c69-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="68c69-115">Relationships</span></span>
<span data-ttu-id="68c69-116">なし</span><span class="sxs-lookup"><span data-stu-id="68c69-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="68c69-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="68c69-117">JSON Representation</span></span>
<span data-ttu-id="68c69-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="68c69-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOsVppAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOsVppAppAssignmentSettings",
  "useDeviceLicensing": true
}
```





