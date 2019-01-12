---
title: windowsAppXAppAssignmentSettings リソースの種類
description: Windows AppX のモバイル アプリケーションをグループに割り当てるときに使用するプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 011bef0bc4ce19028329aff7a4406aea8f918658
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975630"
---
# <a name="windowsappxappassignmentsettings-resource-type"></a><span data-ttu-id="e55e4-103">windowsAppXAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e55e4-103">windowsAppXAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="e55e4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e55e4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e55e4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e55e4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e55e4-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e55e4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e55e4-107">Windows AppX のモバイル アプリケーションをグループに割り当てるときに使用するプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e55e4-107">Contains properties used when assigning a Windows AppX mobile app to a group.</span></span>

<span data-ttu-id="e55e4-108">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="e55e4-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e55e4-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e55e4-109">Properties</span></span>
|<span data-ttu-id="e55e4-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e55e4-110">Property</span></span>|<span data-ttu-id="e55e4-111">種類</span><span class="sxs-lookup"><span data-stu-id="e55e4-111">Type</span></span>|<span data-ttu-id="e55e4-112">説明</span><span class="sxs-lookup"><span data-stu-id="e55e4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e55e4-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="e55e4-113">useDeviceContext</span></span>|<span data-ttu-id="e55e4-114">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="e55e4-114">Boolean</span></span>|<span data-ttu-id="e55e4-115">Windows AppX のモバイル アプリケーションの実行コンテキストのデバイスを使用するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e55e4-115">Whether or not to use device execution context for Windows AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e55e4-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e55e4-116">Relationships</span></span>
<span data-ttu-id="e55e4-117">なし</span><span class="sxs-lookup"><span data-stu-id="e55e4-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e55e4-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e55e4-118">JSON Representation</span></span>
<span data-ttu-id="e55e4-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e55e4-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsAppXAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAppXAppAssignmentSettings",
  "useDeviceContext": true
}
```





