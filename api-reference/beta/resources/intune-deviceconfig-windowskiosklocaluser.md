---
title: windowsKioskLocalUser リソースの種類
description: キオスクの構成にローカル ・ アカウントの識別に使用するクラス
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2dc1e54f7bc4e9fbbef3113abce90cab00825be8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934633"
---
# <a name="windowskiosklocaluser-resource-type"></a><span data-ttu-id="dba4f-103">windowsKioskLocalUser リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dba4f-103">windowsKioskLocalUser resource type</span></span>

> <span data-ttu-id="dba4f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="dba4f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dba4f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dba4f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dba4f-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="dba4f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dba4f-107">キオスクの構成にローカル ・ アカウントの識別に使用するクラス</span><span class="sxs-lookup"><span data-stu-id="dba4f-107">The class used to identify a local account for the kiosk configuration</span></span>

<span data-ttu-id="dba4f-108">[WindowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="dba4f-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dba4f-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dba4f-109">Properties</span></span>
|<span data-ttu-id="dba4f-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dba4f-110">Property</span></span>|<span data-ttu-id="dba4f-111">種類</span><span class="sxs-lookup"><span data-stu-id="dba4f-111">Type</span></span>|<span data-ttu-id="dba4f-112">説明</span><span class="sxs-lookup"><span data-stu-id="dba4f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dba4f-113">userName</span><span class="sxs-lookup"><span data-stu-id="dba4f-113">userName</span></span>|<span data-ttu-id="dba4f-114">String</span><span class="sxs-lookup"><span data-stu-id="dba4f-114">String</span></span>|<span data-ttu-id="dba4f-115">この構成にキオスクがロックアウトされているローカル ユーザー</span><span class="sxs-lookup"><span data-stu-id="dba4f-115">The local user that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="dba4f-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dba4f-116">Relationships</span></span>
<span data-ttu-id="dba4f-117">なし</span><span class="sxs-lookup"><span data-stu-id="dba4f-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dba4f-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dba4f-118">JSON Representation</span></span>
<span data-ttu-id="dba4f-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dba4f-119">Here is a JSON representation of the resource.</span></span>
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





