---
title: windowsKioskLocalUser リソースの種類
description: キオスク構成のローカルアカウントを識別するために使用されるクラス
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b1c375de52d9fc294a308eb7c5b2652ef13db0c4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548083"
---
# <a name="windowskiosklocaluser-resource-type"></a><span data-ttu-id="f568a-103">windowsKioskLocalUser リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f568a-103">windowsKioskLocalUser resource type</span></span>

> <span data-ttu-id="f568a-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f568a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f568a-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f568a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f568a-106">キオスク構成のローカルアカウントを識別するために使用されるクラス</span><span class="sxs-lookup"><span data-stu-id="f568a-106">The class used to identify a local account for the kiosk configuration</span></span>


<span data-ttu-id="f568a-107">[windowskioskuser](../resources/intune-deviceconfig-windowskioskuser.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="f568a-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f568a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f568a-108">Properties</span></span>
|<span data-ttu-id="f568a-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f568a-109">Property</span></span>|<span data-ttu-id="f568a-110">型</span><span class="sxs-lookup"><span data-stu-id="f568a-110">Type</span></span>|<span data-ttu-id="f568a-111">説明</span><span class="sxs-lookup"><span data-stu-id="f568a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f568a-112">userName</span><span class="sxs-lookup"><span data-stu-id="f568a-112">userName</span></span>|<span data-ttu-id="f568a-113">String</span><span class="sxs-lookup"><span data-stu-id="f568a-113">String</span></span>|<span data-ttu-id="f568a-114">このキオスク構成にロックされるローカルユーザー</span><span class="sxs-lookup"><span data-stu-id="f568a-114">The local user that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="f568a-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f568a-115">Relationships</span></span>
<span data-ttu-id="f568a-116">なし</span><span class="sxs-lookup"><span data-stu-id="f568a-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f568a-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f568a-117">JSON Representation</span></span>
<span data-ttu-id="f568a-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f568a-118">Here is a JSON representation of the resource.</span></span>
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





