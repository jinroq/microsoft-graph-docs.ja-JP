---
title: windowsKioskAzureADUser リソースの種類
description: キオスクの構成の AzureAD ユーザー アカウントの識別に使用するクラス
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 08c5b53e8e208abac2801146ff70df6023eaedff
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420186"
---
# <a name="windowskioskazureaduser-resource-type"></a><span data-ttu-id="0bbb3-103">windowsKioskAzureADUser リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0bbb3-103">windowsKioskAzureADUser resource type</span></span>

> <span data-ttu-id="0bbb3-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0bbb3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0bbb3-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0bbb3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0bbb3-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0bbb3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0bbb3-107">キオスクの構成の AzureAD ユーザー アカウントの識別に使用するクラス</span><span class="sxs-lookup"><span data-stu-id="0bbb3-107">The class used to identify an AzureAD user account for the kiosk configuration</span></span>


<span data-ttu-id="0bbb3-108">[WindowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0bbb3-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0bbb3-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0bbb3-109">Properties</span></span>
|<span data-ttu-id="0bbb3-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0bbb3-110">Property</span></span>|<span data-ttu-id="0bbb3-111">型</span><span class="sxs-lookup"><span data-stu-id="0bbb3-111">Type</span></span>|<span data-ttu-id="0bbb3-112">説明</span><span class="sxs-lookup"><span data-stu-id="0bbb3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bbb3-113">userId</span><span class="sxs-lookup"><span data-stu-id="0bbb3-113">userId</span></span>|<span data-ttu-id="0bbb3-114">String</span><span class="sxs-lookup"><span data-stu-id="0bbb3-114">String</span></span>|<span data-ttu-id="0bbb3-115">この構成にキオスクがロックアウトされている AzureAD のユーザーの ID</span><span class="sxs-lookup"><span data-stu-id="0bbb3-115">The ID of the AzureAD user that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="0bbb3-116">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0bbb3-116">userPrincipalName</span></span>|<span data-ttu-id="0bbb3-117">String</span><span class="sxs-lookup"><span data-stu-id="0bbb3-117">String</span></span>|<span data-ttu-id="0bbb3-118">この構成にキオスクがロックアウトされているユーザー アカウント</span><span class="sxs-lookup"><span data-stu-id="0bbb3-118">The user accounts that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="0bbb3-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0bbb3-119">Relationships</span></span>
<span data-ttu-id="0bbb3-120">なし</span><span class="sxs-lookup"><span data-stu-id="0bbb3-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0bbb3-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0bbb3-121">JSON Representation</span></span>
<span data-ttu-id="0bbb3-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0bbb3-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAzureADUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAzureADUser",
  "userId": "String",
  "userPrincipalName": "String"
}
```




