---
title: windowsKioskAzureADGroup リソースの種類
description: キオスクの構成の AzureAD グループを識別するに使用するクラス
author: tfitzmac
ms.openlocfilehash: 3c4cdd8388c71b5f051ea8338e82123c241ec429
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339523"
---
# <a name="windowskioskazureadgroup-resource-type"></a><span data-ttu-id="78cf1-103">windowsKioskAzureADGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="78cf1-103">windowsKioskAzureADGroup resource type</span></span>

> <span data-ttu-id="78cf1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="78cf1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="78cf1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="78cf1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="78cf1-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="78cf1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="78cf1-107">キオスクの構成の AzureAD グループを識別するに使用するクラス</span><span class="sxs-lookup"><span data-stu-id="78cf1-107">The class used to identify an AzureAD group for the kiosk configuration</span></span>

<span data-ttu-id="78cf1-108">[WindowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="78cf1-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="78cf1-109">Properties</span><span class="sxs-lookup"><span data-stu-id="78cf1-109">Properties</span></span>
|<span data-ttu-id="78cf1-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="78cf1-110">Property</span></span>|<span data-ttu-id="78cf1-111">種類</span><span class="sxs-lookup"><span data-stu-id="78cf1-111">Type</span></span>|<span data-ttu-id="78cf1-112">説明</span><span class="sxs-lookup"><span data-stu-id="78cf1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78cf1-113">displayName</span><span class="sxs-lookup"><span data-stu-id="78cf1-113">displayName</span></span>|<span data-ttu-id="78cf1-114">String</span><span class="sxs-lookup"><span data-stu-id="78cf1-114">String</span></span>|<span data-ttu-id="78cf1-115">この構成にキオスクがロックアウトされている AzureAD グループの表示名</span><span class="sxs-lookup"><span data-stu-id="78cf1-115">The display name of the AzureAD group that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="78cf1-116">グループ Id</span><span class="sxs-lookup"><span data-stu-id="78cf1-116">groupId</span></span>|<span data-ttu-id="78cf1-117">String</span><span class="sxs-lookup"><span data-stu-id="78cf1-117">String</span></span>|<span data-ttu-id="78cf1-118">この構成にキオスクがロックアウトされている AzureAD グループの ID</span><span class="sxs-lookup"><span data-stu-id="78cf1-118">The ID of the AzureAD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="78cf1-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="78cf1-119">Relationships</span></span>
<span data-ttu-id="78cf1-120">なし</span><span class="sxs-lookup"><span data-stu-id="78cf1-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="78cf1-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="78cf1-121">JSON Representation</span></span>
<span data-ttu-id="78cf1-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="78cf1-122">Here is a JSON representation of the resource.</span></span>
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





