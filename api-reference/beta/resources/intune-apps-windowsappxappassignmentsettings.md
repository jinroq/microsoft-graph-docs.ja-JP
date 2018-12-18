---
title: windowsAppXAppAssignmentSettings リソースの種類
description: Windows AppX のモバイル アプリケーションをグループに割り当てるときに使用するプロパティが含まれています。
author: tfitzmac
ms.openlocfilehash: 84103a91c3c670ef3da8a0ea2a2e38a95cff79a6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311621"
---
# <a name="windowsappxappassignmentsettings-resource-type"></a><span data-ttu-id="4c360-103">windowsAppXAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4c360-103">windowsAppXAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="4c360-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4c360-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4c360-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c360-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4c360-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4c360-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4c360-107">Windows AppX のモバイル アプリケーションをグループに割り当てるときに使用するプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="4c360-107">Contains properties used when assigning a Windows AppX mobile app to a group.</span></span>

<span data-ttu-id="4c360-108">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="4c360-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4c360-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c360-109">Properties</span></span>
|<span data-ttu-id="4c360-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c360-110">Property</span></span>|<span data-ttu-id="4c360-111">種類</span><span class="sxs-lookup"><span data-stu-id="4c360-111">Type</span></span>|<span data-ttu-id="4c360-112">説明</span><span class="sxs-lookup"><span data-stu-id="4c360-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c360-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="4c360-113">useDeviceContext</span></span>|<span data-ttu-id="4c360-114">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="4c360-114">Boolean</span></span>|<span data-ttu-id="4c360-115">Windows AppX のモバイル アプリケーションの実行コンテキストのデバイスを使用するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="4c360-115">Whether or not to use device execution context for Windows AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c360-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4c360-116">Relationships</span></span>
<span data-ttu-id="4c360-117">なし</span><span class="sxs-lookup"><span data-stu-id="4c360-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4c360-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4c360-118">JSON Representation</span></span>
<span data-ttu-id="4c360-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4c360-119">Here is a JSON representation of the resource.</span></span>
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





