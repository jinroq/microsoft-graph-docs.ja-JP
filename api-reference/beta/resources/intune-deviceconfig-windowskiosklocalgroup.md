---
title: windowsKioskLocalGroup リソースの種類
description: キオスク構成のローカルグループを識別するために使用されるクラス
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 661b1a4a6dd06fe44754232f967ebf8ec9c1ab55
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969003"
---
# <a name="windowskiosklocalgroup-resource-type"></a><span data-ttu-id="caaea-103">windowsKioskLocalGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="caaea-103">windowsKioskLocalGroup resource type</span></span>

> <span data-ttu-id="caaea-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="caaea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="caaea-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="caaea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="caaea-106">キオスク構成のローカルグループを識別するために使用されるクラス</span><span class="sxs-lookup"><span data-stu-id="caaea-106">The class used to identify a local group for the kiosk configuration</span></span>


<span data-ttu-id="caaea-107">[Windowskioskuser](../resources/intune-deviceconfig-windowskioskuser.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="caaea-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="caaea-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="caaea-108">Properties</span></span>
|<span data-ttu-id="caaea-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="caaea-109">Property</span></span>|<span data-ttu-id="caaea-110">型</span><span class="sxs-lookup"><span data-stu-id="caaea-110">Type</span></span>|<span data-ttu-id="caaea-111">説明</span><span class="sxs-lookup"><span data-stu-id="caaea-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="caaea-112">groupName</span><span class="sxs-lookup"><span data-stu-id="caaea-112">groupName</span></span>|<span data-ttu-id="caaea-113">String</span><span class="sxs-lookup"><span data-stu-id="caaea-113">String</span></span>|<span data-ttu-id="caaea-114">このキオスク構成にロックされるローカルグループの名前</span><span class="sxs-lookup"><span data-stu-id="caaea-114">The name of the local group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="caaea-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="caaea-115">Relationships</span></span>
<span data-ttu-id="caaea-116">なし</span><span class="sxs-lookup"><span data-stu-id="caaea-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="caaea-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="caaea-117">JSON Representation</span></span>
<span data-ttu-id="caaea-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="caaea-118">Here is a JSON representation of the resource.</span></span>
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





