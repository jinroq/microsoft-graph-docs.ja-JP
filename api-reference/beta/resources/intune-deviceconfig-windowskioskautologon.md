---
title: windowsKioskAutologon リソースの種類
description: キオスクは、自動ログオンの構成を識別するために使用するクラス
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 33f3e2abe3d01a012a26161121be2d3d9f898435
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932449"
---
# <a name="windowskioskautologon-resource-type"></a><span data-ttu-id="09b6f-103">windowsKioskAutologon リソースの種類</span><span class="sxs-lookup"><span data-stu-id="09b6f-103">windowsKioskAutologon resource type</span></span>

> <span data-ttu-id="09b6f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="09b6f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="09b6f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="09b6f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="09b6f-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="09b6f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="09b6f-107">キオスクは、自動ログオンの構成を識別するために使用するクラス</span><span class="sxs-lookup"><span data-stu-id="09b6f-107">The class used to identify an autologon kiosk configuration</span></span>

<span data-ttu-id="09b6f-108">[WindowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="09b6f-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="09b6f-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09b6f-109">Properties</span></span>
|<span data-ttu-id="09b6f-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09b6f-110">Property</span></span>|<span data-ttu-id="09b6f-111">種類</span><span class="sxs-lookup"><span data-stu-id="09b6f-111">Type</span></span>|<span data-ttu-id="09b6f-112">説明</span><span class="sxs-lookup"><span data-stu-id="09b6f-112">Description</span></span>|
|:---|:---|:---|

## <a name="relationships"></a><span data-ttu-id="09b6f-113">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="09b6f-113">Relationships</span></span>
<span data-ttu-id="09b6f-114">なし</span><span class="sxs-lookup"><span data-stu-id="09b6f-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="09b6f-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="09b6f-115">JSON Representation</span></span>
<span data-ttu-id="09b6f-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="09b6f-116">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAutologon"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAutologon"
}
```





