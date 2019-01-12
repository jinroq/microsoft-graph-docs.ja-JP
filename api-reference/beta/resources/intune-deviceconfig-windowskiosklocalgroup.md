---
title: windowsKioskLocalGroup リソースの種類
description: キオスクの構成にローカル グループを識別するために使用するクラス
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f9c5d467e70b4e2e7f60bc4898be35a2e9fefadc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964754"
---
# <a name="windowskiosklocalgroup-resource-type"></a><span data-ttu-id="e17c7-103">windowsKioskLocalGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e17c7-103">windowsKioskLocalGroup resource type</span></span>

> <span data-ttu-id="e17c7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e17c7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e17c7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e17c7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e17c7-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e17c7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e17c7-107">キオスクの構成にローカル グループを識別するために使用するクラス</span><span class="sxs-lookup"><span data-stu-id="e17c7-107">The class used to identify a local group for the kiosk configuration</span></span>

<span data-ttu-id="e17c7-108">[WindowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="e17c7-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e17c7-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e17c7-109">Properties</span></span>
|<span data-ttu-id="e17c7-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e17c7-110">Property</span></span>|<span data-ttu-id="e17c7-111">種類</span><span class="sxs-lookup"><span data-stu-id="e17c7-111">Type</span></span>|<span data-ttu-id="e17c7-112">説明</span><span class="sxs-lookup"><span data-stu-id="e17c7-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e17c7-113">グループ名</span><span class="sxs-lookup"><span data-stu-id="e17c7-113">groupName</span></span>|<span data-ttu-id="e17c7-114">String</span><span class="sxs-lookup"><span data-stu-id="e17c7-114">String</span></span>|<span data-ttu-id="e17c7-115">この構成にキオスクがロックアウトされているローカル グループの名前</span><span class="sxs-lookup"><span data-stu-id="e17c7-115">The name of the local group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="e17c7-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e17c7-116">Relationships</span></span>
<span data-ttu-id="e17c7-117">なし</span><span class="sxs-lookup"><span data-stu-id="e17c7-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e17c7-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e17c7-118">JSON Representation</span></span>
<span data-ttu-id="e17c7-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e17c7-119">Here is a JSON representation of the resource.</span></span>
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





