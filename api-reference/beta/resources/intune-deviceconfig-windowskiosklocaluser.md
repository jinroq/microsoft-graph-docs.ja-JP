---
title: windowsKioskLocalUser リソースの種類
description: キオスク構成のローカルアカウントを識別するために使用されるクラス
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b1c375de52d9fc294a308eb7c5b2652ef13db0c4
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31777110"
---
# <a name="windowskiosklocaluser-resource-type"></a><span data-ttu-id="0565d-103">windowsKioskLocalUser リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0565d-103">windowsKioskLocalUser resource type</span></span>

> <span data-ttu-id="0565d-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0565d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0565d-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0565d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0565d-106">キオスク構成のローカルアカウントを識別するために使用されるクラス</span><span class="sxs-lookup"><span data-stu-id="0565d-106">The class used to identify a local account for the kiosk configuration</span></span>


<span data-ttu-id="0565d-107">[windowskioskuser](../resources/intune-deviceconfig-windowskioskuser.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="0565d-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0565d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0565d-108">Properties</span></span>
|<span data-ttu-id="0565d-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0565d-109">Property</span></span>|<span data-ttu-id="0565d-110">型</span><span class="sxs-lookup"><span data-stu-id="0565d-110">Type</span></span>|<span data-ttu-id="0565d-111">説明</span><span class="sxs-lookup"><span data-stu-id="0565d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0565d-112">userName</span><span class="sxs-lookup"><span data-stu-id="0565d-112">userName</span></span>|<span data-ttu-id="0565d-113">String</span><span class="sxs-lookup"><span data-stu-id="0565d-113">String</span></span>|<span data-ttu-id="0565d-114">このキオスク構成にロックされるローカルユーザー</span><span class="sxs-lookup"><span data-stu-id="0565d-114">The local user that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="0565d-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0565d-115">Relationships</span></span>
<span data-ttu-id="0565d-116">なし</span><span class="sxs-lookup"><span data-stu-id="0565d-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0565d-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0565d-117">JSON Representation</span></span>
<span data-ttu-id="0565d-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0565d-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskLocalUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskLocalUser",
  "userName": "String"
}
```





