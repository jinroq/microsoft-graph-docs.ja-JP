---
title: microsoftStoreForBusinessAppAssignmentSettings リソースの種類
description: グループに、ビジネス向け Microsoft Store モバイル アプリを割り当てるためのプロパティが含まれます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e117e805a4fff60eb3271310f1e501413b3ebb33
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34986194"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="01bcf-103">microsoftStoreForBusinessAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="01bcf-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="01bcf-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="01bcf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01bcf-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="01bcf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01bcf-106">グループに、ビジネス向け Microsoft Store モバイル アプリを割り当てるためのプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="01bcf-106">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>


<span data-ttu-id="01bcf-107">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="01bcf-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="01bcf-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="01bcf-108">Properties</span></span>
|<span data-ttu-id="01bcf-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="01bcf-109">Property</span></span>|<span data-ttu-id="01bcf-110">型</span><span class="sxs-lookup"><span data-stu-id="01bcf-110">Type</span></span>|<span data-ttu-id="01bcf-111">説明</span><span class="sxs-lookup"><span data-stu-id="01bcf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01bcf-112">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="01bcf-112">useDeviceContext</span></span>|<span data-ttu-id="01bcf-113">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="01bcf-113">Boolean</span></span>|<span data-ttu-id="01bcf-114">ビジネス向け Microsoft Store モバイル アプリのデバイス実行コンテキストを使用するかどうか。</span><span class="sxs-lookup"><span data-stu-id="01bcf-114">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="01bcf-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="01bcf-115">Relationships</span></span>
<span data-ttu-id="01bcf-116">なし</span><span class="sxs-lookup"><span data-stu-id="01bcf-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="01bcf-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="01bcf-117">JSON Representation</span></span>
<span data-ttu-id="01bcf-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="01bcf-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.microsoftStoreForBusinessAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessAppAssignmentSettings",
  "useDeviceContext": true
}
```





