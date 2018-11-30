---
title: windowsKioskAzureADGroup リソースの種類
description: キオスクの構成の AzureAD グループを識別するに使用するクラス
ms.openlocfilehash: 4853013c9c1e9d4c276ee5e2ba83cb8b36afd06c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066950"
---
# <a name="windowskioskazureadgroup-resource-type"></a><span data-ttu-id="3a341-103">windowsKioskAzureADGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3a341-103">windowsKioskAzureADGroup resource type</span></span>

> <span data-ttu-id="3a341-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3a341-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3a341-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3a341-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3a341-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3a341-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3a341-107">キオスクの構成の AzureAD グループを識別するに使用するクラス</span><span class="sxs-lookup"><span data-stu-id="3a341-107">The class used to identify an AzureAD group for the kiosk configuration</span></span>

<span data-ttu-id="3a341-108">[WindowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="3a341-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3a341-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3a341-109">Properties</span></span>
|<span data-ttu-id="3a341-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3a341-110">Property</span></span>|<span data-ttu-id="3a341-111">型</span><span class="sxs-lookup"><span data-stu-id="3a341-111">Type</span></span>|<span data-ttu-id="3a341-112">説明</span><span class="sxs-lookup"><span data-stu-id="3a341-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a341-113">displayName</span><span class="sxs-lookup"><span data-stu-id="3a341-113">displayName</span></span>|<span data-ttu-id="3a341-114">String</span><span class="sxs-lookup"><span data-stu-id="3a341-114">String</span></span>|<span data-ttu-id="3a341-115">この構成にキオスクがロックアウトされている AzureAD グループの表示名</span><span class="sxs-lookup"><span data-stu-id="3a341-115">The display name of the AzureAD group that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="3a341-116">グループ Id</span><span class="sxs-lookup"><span data-stu-id="3a341-116">groupId</span></span>|<span data-ttu-id="3a341-117">String</span><span class="sxs-lookup"><span data-stu-id="3a341-117">String</span></span>|<span data-ttu-id="3a341-118">この構成にキオスクがロックアウトされている AzureAD グループの ID</span><span class="sxs-lookup"><span data-stu-id="3a341-118">The ID of the AzureAD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a341-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3a341-119">Relationships</span></span>
<span data-ttu-id="3a341-120">なし</span><span class="sxs-lookup"><span data-stu-id="3a341-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3a341-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3a341-121">JSON Representation</span></span>
<span data-ttu-id="3a341-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3a341-122">Here is a JSON representation of the resource.</span></span>
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





