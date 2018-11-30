---
title: windowsKioskAzureADUser リソースの種類
description: キオスクの構成の AzureAD ユーザー アカウントの識別に使用するクラス
ms.openlocfilehash: 22e71ab10ac7fb755050e8d6e5d19568bef2fae8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069659"
---
# <a name="windowskioskazureaduser-resource-type"></a><span data-ttu-id="79007-103">windowsKioskAzureADUser リソースの種類</span><span class="sxs-lookup"><span data-stu-id="79007-103">windowsKioskAzureADUser resource type</span></span>

> <span data-ttu-id="79007-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="79007-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="79007-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79007-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="79007-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="79007-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="79007-107">キオスクの構成の AzureAD ユーザー アカウントの識別に使用するクラス</span><span class="sxs-lookup"><span data-stu-id="79007-107">The class used to identify an AzureAD user account for the kiosk configuration</span></span>

<span data-ttu-id="79007-108">[WindowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="79007-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="79007-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="79007-109">Properties</span></span>
|<span data-ttu-id="79007-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="79007-110">Property</span></span>|<span data-ttu-id="79007-111">型</span><span class="sxs-lookup"><span data-stu-id="79007-111">Type</span></span>|<span data-ttu-id="79007-112">説明</span><span class="sxs-lookup"><span data-stu-id="79007-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79007-113">userId</span><span class="sxs-lookup"><span data-stu-id="79007-113">userId</span></span>|<span data-ttu-id="79007-114">String</span><span class="sxs-lookup"><span data-stu-id="79007-114">String</span></span>|<span data-ttu-id="79007-115">この構成にキオスクがロックアウトされている AzureAD のユーザーの ID</span><span class="sxs-lookup"><span data-stu-id="79007-115">The ID of the AzureAD user that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="79007-116">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="79007-116">userPrincipalName</span></span>|<span data-ttu-id="79007-117">String</span><span class="sxs-lookup"><span data-stu-id="79007-117">String</span></span>|<span data-ttu-id="79007-118">この構成にキオスクがロックアウトされているユーザー アカウント</span><span class="sxs-lookup"><span data-stu-id="79007-118">The user accounts that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="79007-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="79007-119">Relationships</span></span>
<span data-ttu-id="79007-120">なし</span><span class="sxs-lookup"><span data-stu-id="79007-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="79007-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="79007-121">JSON Representation</span></span>
<span data-ttu-id="79007-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="79007-122">Here is a JSON representation of the resource.</span></span>
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





