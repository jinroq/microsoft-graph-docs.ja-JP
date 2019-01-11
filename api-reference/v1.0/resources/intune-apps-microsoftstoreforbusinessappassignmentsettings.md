---
title: microsoftStoreForBusinessAppAssignmentSettings リソースの種類
description: グループに、ビジネス向け Microsoft Store モバイル アプリを割り当てるためのプロパティが含まれます。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 86922fa8b9ca587f0c777bbaed4b479620e6af21
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876371"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="05808-103">microsoftStoreForBusinessAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="05808-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="05808-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="05808-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="05808-105">グループに、ビジネス向け Microsoft Store モバイル アプリを割り当てるためのプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="05808-105">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>

<span data-ttu-id="05808-106">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="05808-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="05808-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="05808-107">Properties</span></span>
|<span data-ttu-id="05808-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="05808-108">Property</span></span>|<span data-ttu-id="05808-109">種類</span><span class="sxs-lookup"><span data-stu-id="05808-109">Type</span></span>|<span data-ttu-id="05808-110">説明</span><span class="sxs-lookup"><span data-stu-id="05808-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05808-111">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="05808-111">useDeviceContext</span></span>|<span data-ttu-id="05808-112">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="05808-112">Boolean</span></span>|<span data-ttu-id="05808-113">ビジネス向け Microsoft Store モバイル アプリのデバイス実行コンテキストを使用するかどうか。</span><span class="sxs-lookup"><span data-stu-id="05808-113">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="05808-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="05808-114">Relationships</span></span>
<span data-ttu-id="05808-115">なし</span><span class="sxs-lookup"><span data-stu-id="05808-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="05808-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="05808-116">JSON Representation</span></span>
<span data-ttu-id="05808-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="05808-117">Here is a JSON representation of the resource.</span></span>
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



