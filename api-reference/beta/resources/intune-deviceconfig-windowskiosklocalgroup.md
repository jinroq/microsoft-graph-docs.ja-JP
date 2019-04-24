---
title: windowsKioskLocalGroup リソースの種類
description: キオスク構成のローカルグループを識別するために使用されるクラス
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 54a4686282e4c13f657adf010a3e0272025eb249
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453972"
---
# <a name="windowskiosklocalgroup-resource-type"></a><span data-ttu-id="92943-103">windowsKioskLocalGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="92943-103">windowsKioskLocalGroup resource type</span></span>

> <span data-ttu-id="92943-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92943-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92943-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="92943-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92943-106">キオスク構成のローカルグループを識別するために使用されるクラス</span><span class="sxs-lookup"><span data-stu-id="92943-106">The class used to identify a local group for the kiosk configuration</span></span>


<span data-ttu-id="92943-107">[windowskioskuser](../resources/intune-deviceconfig-windowskioskuser.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="92943-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="92943-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92943-108">Properties</span></span>
|<span data-ttu-id="92943-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92943-109">Property</span></span>|<span data-ttu-id="92943-110">型</span><span class="sxs-lookup"><span data-stu-id="92943-110">Type</span></span>|<span data-ttu-id="92943-111">説明</span><span class="sxs-lookup"><span data-stu-id="92943-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92943-112">groupName</span><span class="sxs-lookup"><span data-stu-id="92943-112">groupName</span></span>|<span data-ttu-id="92943-113">String</span><span class="sxs-lookup"><span data-stu-id="92943-113">String</span></span>|<span data-ttu-id="92943-114">このキオスク構成にロックされるローカルグループの名前</span><span class="sxs-lookup"><span data-stu-id="92943-114">The name of the local group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="92943-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="92943-115">Relationships</span></span>
<span data-ttu-id="92943-116">なし</span><span class="sxs-lookup"><span data-stu-id="92943-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="92943-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="92943-117">JSON Representation</span></span>
<span data-ttu-id="92943-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="92943-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskLocalGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskLocalGroup",
  "groupName": "String"
}
```





