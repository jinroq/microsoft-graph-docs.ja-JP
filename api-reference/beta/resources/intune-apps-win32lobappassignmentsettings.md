---
title: win32LobAppAssignmentSettings リソースの種類
description: グループへの Win32 LOB モバイルアプリの割り当てに使用されるプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f8b6588c270c9b7977ddd7b3c7eb239f3b0432cb
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993236"
---
# <a name="win32lobappassignmentsettings-resource-type"></a><span data-ttu-id="69409-103">win32LobAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="69409-103">win32LobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="69409-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="69409-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69409-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="69409-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69409-106">グループへの Win32 LOB モバイルアプリの割り当てに使用されるプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="69409-106">Contains properties used to assign an Win32 LOB mobile app to a group.</span></span>


<span data-ttu-id="69409-107">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="69409-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="69409-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="69409-108">Properties</span></span>
|<span data-ttu-id="69409-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="69409-109">Property</span></span>|<span data-ttu-id="69409-110">型</span><span class="sxs-lookup"><span data-stu-id="69409-110">Type</span></span>|<span data-ttu-id="69409-111">説明</span><span class="sxs-lookup"><span data-stu-id="69409-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69409-112">受け取る</span><span class="sxs-lookup"><span data-stu-id="69409-112">notifications</span></span>|[<span data-ttu-id="69409-113">win32LobAppNotification</span><span class="sxs-lookup"><span data-stu-id="69409-113">win32LobAppNotification</span></span>](../resources/intune-apps-win32lobappnotification.md)|<span data-ttu-id="69409-114">このアプリの割り当ての通知状態。</span><span class="sxs-lookup"><span data-stu-id="69409-114">The notification status this app assignment.</span></span> <span data-ttu-id="69409-115">可能な値は、`showAll`、`showReboot`、`hideAll` です。</span><span class="sxs-lookup"><span data-stu-id="69409-115">Possible values are: `showAll`, `showReboot`, `hideAll`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="69409-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="69409-116">Relationships</span></span>
<span data-ttu-id="69409-117">なし</span><span class="sxs-lookup"><span data-stu-id="69409-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="69409-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="69409-118">JSON Representation</span></span>
<span data-ttu-id="69409-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="69409-119">Here is a JSON representation of the resource.</span></span>
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





