---
title: windowsAppXAppAssignmentSettings リソースの種類
description: Windows AppX モバイルアプリをグループに割り当てるときに使用されるプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3bba16c9a98bbdbf584cd7a0cba1c4634bf90b31
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949872"
---
# <a name="windowsappxappassignmentsettings-resource-type"></a><span data-ttu-id="8f885-103">windowsAppXAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8f885-103">windowsAppXAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="8f885-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8f885-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8f885-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8f885-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f885-106">Windows AppX モバイルアプリをグループに割り当てるときに使用されるプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="8f885-106">Contains properties used when assigning a Windows AppX mobile app to a group.</span></span>


<span data-ttu-id="8f885-107">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="8f885-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8f885-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8f885-108">Properties</span></span>
|<span data-ttu-id="8f885-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8f885-109">Property</span></span>|<span data-ttu-id="8f885-110">型</span><span class="sxs-lookup"><span data-stu-id="8f885-110">Type</span></span>|<span data-ttu-id="8f885-111">説明</span><span class="sxs-lookup"><span data-stu-id="8f885-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f885-112">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="8f885-112">useDeviceContext</span></span>|<span data-ttu-id="8f885-113">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="8f885-113">Boolean</span></span>|<span data-ttu-id="8f885-114">Windows AppX モバイルアプリのデバイス実行コンテキストを使用するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="8f885-114">Whether or not to use device execution context for Windows AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f885-115">関係</span><span class="sxs-lookup"><span data-stu-id="8f885-115">Relationships</span></span>
<span data-ttu-id="8f885-116">なし</span><span class="sxs-lookup"><span data-stu-id="8f885-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8f885-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8f885-117">JSON Representation</span></span>
<span data-ttu-id="8f885-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8f885-118">Here is a JSON representation of the resource.</span></span>
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




