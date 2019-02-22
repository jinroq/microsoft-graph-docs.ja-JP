---
title: windowsUniversalAppXAppAssignmentSettings リソースの種類
description: Windows Universal AppX モバイルアプリをグループに割り当てるときに使用されるプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 58e0c656464d962d1a16a7c4651c4379876bf6ae
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153733"
---
# <a name="windowsuniversalappxappassignmentsettings-resource-type"></a><span data-ttu-id="4e3b7-103">windowsUniversalAppXAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4e3b7-103">windowsUniversalAppXAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="4e3b7-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4e3b7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e3b7-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4e3b7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e3b7-106">Windows Universal AppX モバイルアプリをグループに割り当てるときに使用されるプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="4e3b7-106">Contains properties used when assigning a Windows Universal AppX mobile app to a group.</span></span>


<span data-ttu-id="4e3b7-107">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="4e3b7-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4e3b7-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4e3b7-108">Properties</span></span>
|<span data-ttu-id="4e3b7-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4e3b7-109">Property</span></span>|<span data-ttu-id="4e3b7-110">型</span><span class="sxs-lookup"><span data-stu-id="4e3b7-110">Type</span></span>|<span data-ttu-id="4e3b7-111">説明</span><span class="sxs-lookup"><span data-stu-id="4e3b7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e3b7-112">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="4e3b7-112">useDeviceContext</span></span>|<span data-ttu-id="4e3b7-113">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="4e3b7-113">Boolean</span></span>|<span data-ttu-id="4e3b7-114">Windows Universal AppX モバイルアプリのデバイス実行コンテキストを使用するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="4e3b7-114">Whether or not to use device execution context for Windows Universal AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e3b7-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4e3b7-115">Relationships</span></span>
<span data-ttu-id="4e3b7-116">なし</span><span class="sxs-lookup"><span data-stu-id="4e3b7-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e3b7-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4e3b7-117">JSON Representation</span></span>
<span data-ttu-id="4e3b7-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4e3b7-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUniversalAppXAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXAppAssignmentSettings",
  "useDeviceContext": true
}
```




