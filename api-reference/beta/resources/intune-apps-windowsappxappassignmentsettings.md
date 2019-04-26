---
title: windowsAppXAppAssignmentSettings リソースの種類
description: Windows AppX モバイルアプリをグループに割り当てるときに使用されるプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f15af8bf60dae2b40473eb23a1093f9e73bda7b6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32557860"
---
# <a name="windowsappxappassignmentsettings-resource-type"></a><span data-ttu-id="2e62c-103">windowsAppXAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2e62c-103">windowsAppXAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="2e62c-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2e62c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2e62c-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2e62c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e62c-106">Windows AppX モバイルアプリをグループに割り当てるときに使用されるプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="2e62c-106">Contains properties used when assigning a Windows AppX mobile app to a group.</span></span>


<span data-ttu-id="2e62c-107">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="2e62c-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2e62c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2e62c-108">Properties</span></span>
|<span data-ttu-id="2e62c-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2e62c-109">Property</span></span>|<span data-ttu-id="2e62c-110">型</span><span class="sxs-lookup"><span data-stu-id="2e62c-110">Type</span></span>|<span data-ttu-id="2e62c-111">説明</span><span class="sxs-lookup"><span data-stu-id="2e62c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e62c-112">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="2e62c-112">useDeviceContext</span></span>|<span data-ttu-id="2e62c-113">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="2e62c-113">Boolean</span></span>|<span data-ttu-id="2e62c-114">Windows AppX モバイルアプリのデバイス実行コンテキストを使用するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="2e62c-114">Whether or not to use device execution context for Windows AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2e62c-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2e62c-115">Relationships</span></span>
<span data-ttu-id="2e62c-116">なし</span><span class="sxs-lookup"><span data-stu-id="2e62c-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2e62c-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2e62c-117">JSON Representation</span></span>
<span data-ttu-id="2e62c-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2e62c-118">Here is a JSON representation of the resource.</span></span>
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





