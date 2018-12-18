---
title: windowsKioskLocalGroup リソースの種類
description: キオスクの構成にローカル グループを識別するために使用するクラス
author: tfitzmac
ms.openlocfilehash: bb2e0cddd1c9b2530e1f146e966d707466c737d1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306847"
---
# <a name="windowskiosklocalgroup-resource-type"></a><span data-ttu-id="c0f08-103">windowsKioskLocalGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c0f08-103">windowsKioskLocalGroup resource type</span></span>

> <span data-ttu-id="c0f08-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c0f08-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0f08-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0f08-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c0f08-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c0f08-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c0f08-107">キオスクの構成にローカル グループを識別するために使用するクラス</span><span class="sxs-lookup"><span data-stu-id="c0f08-107">The class used to identify a local group for the kiosk configuration</span></span>

<span data-ttu-id="c0f08-108">[WindowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="c0f08-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c0f08-109">Properties</span><span class="sxs-lookup"><span data-stu-id="c0f08-109">Properties</span></span>
|<span data-ttu-id="c0f08-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c0f08-110">Property</span></span>|<span data-ttu-id="c0f08-111">種類</span><span class="sxs-lookup"><span data-stu-id="c0f08-111">Type</span></span>|<span data-ttu-id="c0f08-112">説明</span><span class="sxs-lookup"><span data-stu-id="c0f08-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0f08-113">グループ名</span><span class="sxs-lookup"><span data-stu-id="c0f08-113">groupName</span></span>|<span data-ttu-id="c0f08-114">String</span><span class="sxs-lookup"><span data-stu-id="c0f08-114">String</span></span>|<span data-ttu-id="c0f08-115">この構成にキオスクがロックアウトされているローカル グループの名前</span><span class="sxs-lookup"><span data-stu-id="c0f08-115">The name of the local group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0f08-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c0f08-116">Relationships</span></span>
<span data-ttu-id="c0f08-117">なし</span><span class="sxs-lookup"><span data-stu-id="c0f08-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c0f08-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c0f08-118">JSON Representation</span></span>
<span data-ttu-id="c0f08-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c0f08-119">Here is a JSON representation of the resource.</span></span>
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





