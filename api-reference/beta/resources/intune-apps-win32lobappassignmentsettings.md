---
title: win32LobAppAssignmentSettings リソースの種類
description: Win32 の LOB のモバイル アプリケーションをグループに割り当てるために使用するプロパティが含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 215b5c7086c2336f80bc0b812a108fbe2e2c1740
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430375"
---
# <a name="win32lobappassignmentsettings-resource-type"></a><span data-ttu-id="7cfff-103">win32LobAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7cfff-103">win32LobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="7cfff-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7cfff-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7cfff-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7cfff-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7cfff-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7cfff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7cfff-107">Win32 の LOB のモバイル アプリケーションをグループに割り当てるために使用するプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="7cfff-107">Contains properties used to assign an Win32 LOB mobile app to a group.</span></span>


<span data-ttu-id="7cfff-108">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="7cfff-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7cfff-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7cfff-109">Properties</span></span>
|<span data-ttu-id="7cfff-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7cfff-110">Property</span></span>|<span data-ttu-id="7cfff-111">型</span><span class="sxs-lookup"><span data-stu-id="7cfff-111">Type</span></span>|<span data-ttu-id="7cfff-112">説明</span><span class="sxs-lookup"><span data-stu-id="7cfff-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7cfff-113">通知</span><span class="sxs-lookup"><span data-stu-id="7cfff-113">notifications</span></span>|[<span data-ttu-id="7cfff-114">win32LobAppNotification</span><span class="sxs-lookup"><span data-stu-id="7cfff-114">win32LobAppNotification</span></span>](../resources/intune-apps-win32lobappnotification.md)|<span data-ttu-id="7cfff-115">通知の状態このアプリケーションの割り当て。</span><span class="sxs-lookup"><span data-stu-id="7cfff-115">The notification status this app assignment.</span></span> <span data-ttu-id="7cfff-116">可能な値は、`showAll`、`showReboot`、`hideAll` です。</span><span class="sxs-lookup"><span data-stu-id="7cfff-116">Possible values are: `showAll`, `showReboot`, `hideAll`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7cfff-117">関係</span><span class="sxs-lookup"><span data-stu-id="7cfff-117">Relationships</span></span>
<span data-ttu-id="7cfff-118">なし</span><span class="sxs-lookup"><span data-stu-id="7cfff-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7cfff-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7cfff-119">JSON Representation</span></span>
<span data-ttu-id="7cfff-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7cfff-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppAssignmentSettings",
  "notifications": "String"
}
```




