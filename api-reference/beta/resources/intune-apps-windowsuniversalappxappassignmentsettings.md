---
title: windowsUniversalAppXAppAssignmentSettings リソースの種類
description: Windows Universal AppX モバイルアプリをグループに割り当てるときに使用されるプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f04f8207eab8bea01fd164eb1fdd7b34baf605a7
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34985648"
---
# <a name="windowsuniversalappxappassignmentsettings-resource-type"></a><span data-ttu-id="0b96f-103">windowsUniversalAppXAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0b96f-103">windowsUniversalAppXAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="0b96f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0b96f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b96f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0b96f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b96f-106">Windows Universal AppX モバイルアプリをグループに割り当てるときに使用されるプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="0b96f-106">Contains properties used when assigning a Windows Universal AppX mobile app to a group.</span></span>


<span data-ttu-id="0b96f-107">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="0b96f-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0b96f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0b96f-108">Properties</span></span>
|<span data-ttu-id="0b96f-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0b96f-109">Property</span></span>|<span data-ttu-id="0b96f-110">型</span><span class="sxs-lookup"><span data-stu-id="0b96f-110">Type</span></span>|<span data-ttu-id="0b96f-111">説明</span><span class="sxs-lookup"><span data-stu-id="0b96f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b96f-112">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="0b96f-112">useDeviceContext</span></span>|<span data-ttu-id="0b96f-113">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="0b96f-113">Boolean</span></span>|<span data-ttu-id="0b96f-114">Windows Universal AppX モバイルアプリのデバイス実行コンテキストを使用するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="0b96f-114">Whether or not to use device execution context for Windows Universal AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b96f-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0b96f-115">Relationships</span></span>
<span data-ttu-id="0b96f-116">なし</span><span class="sxs-lookup"><span data-stu-id="0b96f-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0b96f-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0b96f-117">JSON Representation</span></span>
<span data-ttu-id="0b96f-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0b96f-118">Here is a JSON representation of the resource.</span></span>
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





