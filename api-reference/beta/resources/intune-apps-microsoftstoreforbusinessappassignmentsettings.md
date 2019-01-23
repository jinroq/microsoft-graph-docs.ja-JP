---
title: microsoftStoreForBusinessAppAssignmentSettings リソースの種類
description: グループに、ビジネス向け Microsoft Store モバイル アプリを割り当てるためのプロパティが含まれます。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f5f566a04169be20777b9f0fb5a7aa911ad3e864
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393250"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="ef3aa-103">microsoftStoreForBusinessAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ef3aa-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="ef3aa-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ef3aa-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ef3aa-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ef3aa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ef3aa-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ef3aa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef3aa-107">グループに、ビジネス向け Microsoft Store モバイル アプリを割り当てるためのプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="ef3aa-107">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>


<span data-ttu-id="ef3aa-108">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="ef3aa-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ef3aa-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ef3aa-109">Properties</span></span>
|<span data-ttu-id="ef3aa-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ef3aa-110">Property</span></span>|<span data-ttu-id="ef3aa-111">型</span><span class="sxs-lookup"><span data-stu-id="ef3aa-111">Type</span></span>|<span data-ttu-id="ef3aa-112">説明</span><span class="sxs-lookup"><span data-stu-id="ef3aa-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef3aa-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="ef3aa-113">useDeviceContext</span></span>|<span data-ttu-id="ef3aa-114">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="ef3aa-114">Boolean</span></span>|<span data-ttu-id="ef3aa-115">ビジネス向け Microsoft Store モバイル アプリのデバイス実行コンテキストを使用するかどうか。</span><span class="sxs-lookup"><span data-stu-id="ef3aa-115">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ef3aa-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ef3aa-116">Relationships</span></span>
<span data-ttu-id="ef3aa-117">なし</span><span class="sxs-lookup"><span data-stu-id="ef3aa-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ef3aa-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ef3aa-118">JSON Representation</span></span>
<span data-ttu-id="ef3aa-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ef3aa-119">Here is a JSON representation of the resource.</span></span>
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




