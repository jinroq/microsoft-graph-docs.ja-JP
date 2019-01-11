---
title: windowsKioskAzureADGroup リソースの種類
description: キオスクの構成の AzureAD グループを識別するに使用するクラス
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 16c2b17220a92f9f230b786238b1195e2af48d6b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849869"
---
# <a name="windowskioskazureadgroup-resource-type"></a><span data-ttu-id="cee70-103">windowsKioskAzureADGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cee70-103">windowsKioskAzureADGroup resource type</span></span>

> <span data-ttu-id="cee70-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cee70-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cee70-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cee70-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cee70-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cee70-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cee70-107">キオスクの構成の AzureAD グループを識別するに使用するクラス</span><span class="sxs-lookup"><span data-stu-id="cee70-107">The class used to identify an AzureAD group for the kiosk configuration</span></span>

<span data-ttu-id="cee70-108">[WindowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="cee70-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cee70-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cee70-109">Properties</span></span>
|<span data-ttu-id="cee70-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cee70-110">Property</span></span>|<span data-ttu-id="cee70-111">種類</span><span class="sxs-lookup"><span data-stu-id="cee70-111">Type</span></span>|<span data-ttu-id="cee70-112">説明</span><span class="sxs-lookup"><span data-stu-id="cee70-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cee70-113">displayName</span><span class="sxs-lookup"><span data-stu-id="cee70-113">displayName</span></span>|<span data-ttu-id="cee70-114">String</span><span class="sxs-lookup"><span data-stu-id="cee70-114">String</span></span>|<span data-ttu-id="cee70-115">この構成にキオスクがロックアウトされている AzureAD グループの表示名</span><span class="sxs-lookup"><span data-stu-id="cee70-115">The display name of the AzureAD group that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="cee70-116">グループ Id</span><span class="sxs-lookup"><span data-stu-id="cee70-116">groupId</span></span>|<span data-ttu-id="cee70-117">String</span><span class="sxs-lookup"><span data-stu-id="cee70-117">String</span></span>|<span data-ttu-id="cee70-118">この構成にキオスクがロックアウトされている AzureAD グループの ID</span><span class="sxs-lookup"><span data-stu-id="cee70-118">The ID of the AzureAD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="cee70-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cee70-119">Relationships</span></span>
<span data-ttu-id="cee70-120">なし</span><span class="sxs-lookup"><span data-stu-id="cee70-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cee70-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cee70-121">JSON Representation</span></span>
<span data-ttu-id="cee70-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cee70-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAzureADGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAzureADGroup",
  "displayName": "String",
  "groupId": "String"
}
```





