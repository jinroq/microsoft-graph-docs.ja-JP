---
title: windowsAppXAppAssignmentSettings リソースの種類
description: Windows AppX のモバイル アプリケーションをグループに割り当てるときに使用するプロパティが含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0f55400b0e17884a4e6ca3de0692e69d388c46e2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410925"
---
# <a name="windowsappxappassignmentsettings-resource-type"></a><span data-ttu-id="e91ea-103">windowsAppXAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e91ea-103">windowsAppXAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="e91ea-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e91ea-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e91ea-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e91ea-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e91ea-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e91ea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e91ea-107">Windows AppX のモバイル アプリケーションをグループに割り当てるときに使用するプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e91ea-107">Contains properties used when assigning a Windows AppX mobile app to a group.</span></span>


<span data-ttu-id="e91ea-108">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="e91ea-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e91ea-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e91ea-109">Properties</span></span>
|<span data-ttu-id="e91ea-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e91ea-110">Property</span></span>|<span data-ttu-id="e91ea-111">型</span><span class="sxs-lookup"><span data-stu-id="e91ea-111">Type</span></span>|<span data-ttu-id="e91ea-112">説明</span><span class="sxs-lookup"><span data-stu-id="e91ea-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e91ea-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="e91ea-113">useDeviceContext</span></span>|<span data-ttu-id="e91ea-114">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="e91ea-114">Boolean</span></span>|<span data-ttu-id="e91ea-115">Windows AppX のモバイル アプリケーションの実行コンテキストのデバイスを使用するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e91ea-115">Whether or not to use device execution context for Windows AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e91ea-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e91ea-116">Relationships</span></span>
<span data-ttu-id="e91ea-117">なし</span><span class="sxs-lookup"><span data-stu-id="e91ea-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e91ea-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e91ea-118">JSON Representation</span></span>
<span data-ttu-id="e91ea-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e91ea-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsAppXAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAppXAppAssignmentSettings",
  "useDeviceContext": true
}
```




