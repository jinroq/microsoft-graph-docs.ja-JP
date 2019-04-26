---
title: macosvppapp割り当て設定リソースの種類
description: グループへの Mac VPP モバイルアプリの割り当てに使用されるプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b55e203e58197d4b3e29d4a6a8567769d9196e0c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553086"
---
# <a name="macosvppappassignmentsettings-resource-type"></a><span data-ttu-id="fef9e-103">macosvppapp割り当て設定リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fef9e-103">macOsVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="fef9e-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fef9e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fef9e-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fef9e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fef9e-106">グループへの Mac VPP モバイルアプリの割り当てに使用されるプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="fef9e-106">Contains properties used to assign an Mac VPP mobile app to a group.</span></span>


<span data-ttu-id="fef9e-107">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="fef9e-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fef9e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fef9e-108">Properties</span></span>
|<span data-ttu-id="fef9e-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fef9e-109">Property</span></span>|<span data-ttu-id="fef9e-110">型</span><span class="sxs-lookup"><span data-stu-id="fef9e-110">Type</span></span>|<span data-ttu-id="fef9e-111">説明</span><span class="sxs-lookup"><span data-stu-id="fef9e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fef9e-112">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="fef9e-112">useDeviceLicensing</span></span>|<span data-ttu-id="fef9e-113">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="fef9e-113">Boolean</span></span>|<span data-ttu-id="fef9e-114">デバイスのライセンスを使用するかどうか。</span><span class="sxs-lookup"><span data-stu-id="fef9e-114">Whether or not to use device licensing.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fef9e-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fef9e-115">Relationships</span></span>
<span data-ttu-id="fef9e-116">なし</span><span class="sxs-lookup"><span data-stu-id="fef9e-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fef9e-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fef9e-117">JSON Representation</span></span>
<span data-ttu-id="fef9e-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fef9e-118">Here is a JSON representation of the resource.</span></span>
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





