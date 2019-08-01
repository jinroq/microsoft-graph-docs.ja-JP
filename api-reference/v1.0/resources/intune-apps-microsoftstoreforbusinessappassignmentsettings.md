---
title: microsoftStoreForBusinessAppAssignmentSettings リソースの種類
description: グループに、ビジネス向け Microsoft Store モバイル アプリを割り当てるためのプロパティが含まれます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e347bc5967ccd732530cbe9fde5367d354c9a81b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028981"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="b9347-103">microsoftStoreForBusinessAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b9347-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="b9347-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b9347-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9347-105">グループに、ビジネス向け Microsoft Store モバイル アプリを割り当てるためのプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="b9347-105">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>


<span data-ttu-id="b9347-106">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="b9347-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b9347-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b9347-107">Properties</span></span>
|<span data-ttu-id="b9347-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b9347-108">Property</span></span>|<span data-ttu-id="b9347-109">型</span><span class="sxs-lookup"><span data-stu-id="b9347-109">Type</span></span>|<span data-ttu-id="b9347-110">説明</span><span class="sxs-lookup"><span data-stu-id="b9347-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9347-111">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="b9347-111">useDeviceContext</span></span>|<span data-ttu-id="b9347-112">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="b9347-112">Boolean</span></span>|<span data-ttu-id="b9347-113">ビジネス向け Microsoft Store モバイル アプリのデバイス実行コンテキストを使用するかどうか。</span><span class="sxs-lookup"><span data-stu-id="b9347-113">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9347-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b9347-114">Relationships</span></span>
<span data-ttu-id="b9347-115">なし</span><span class="sxs-lookup"><span data-stu-id="b9347-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b9347-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b9347-116">JSON Representation</span></span>
<span data-ttu-id="b9347-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b9347-117">Here is a JSON representation of the resource.</span></span>
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



