---
title: windowsUniversalAppXAppAssignmentSettings リソースの種類
description: Windows ユニバーサル AppX のモバイル アプリケーションをグループに割り当てるときに使用するプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ebb9649460fbfa6da717ba099786eb7d4c2807da
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987007"
---
# <a name="windowsuniversalappxappassignmentsettings-resource-type"></a><span data-ttu-id="1be5b-103">windowsUniversalAppXAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1be5b-103">windowsUniversalAppXAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="1be5b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1be5b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1be5b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1be5b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1be5b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1be5b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1be5b-107">Windows ユニバーサル AppX のモバイル アプリケーションをグループに割り当てるときに使用するプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="1be5b-107">Contains properties used when assigning a Windows Universal AppX mobile app to a group.</span></span>

<span data-ttu-id="1be5b-108">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="1be5b-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1be5b-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1be5b-109">Properties</span></span>
|<span data-ttu-id="1be5b-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1be5b-110">Property</span></span>|<span data-ttu-id="1be5b-111">種類</span><span class="sxs-lookup"><span data-stu-id="1be5b-111">Type</span></span>|<span data-ttu-id="1be5b-112">説明</span><span class="sxs-lookup"><span data-stu-id="1be5b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1be5b-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="1be5b-113">useDeviceContext</span></span>|<span data-ttu-id="1be5b-114">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="1be5b-114">Boolean</span></span>|<span data-ttu-id="1be5b-115">Windows ユニバーサル AppX のモバイル アプリケーションの実行コンテキストのデバイスを使用するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="1be5b-115">Whether or not to use device execution context for Windows Universal AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1be5b-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1be5b-116">Relationships</span></span>
<span data-ttu-id="1be5b-117">なし</span><span class="sxs-lookup"><span data-stu-id="1be5b-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1be5b-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1be5b-118">JSON Representation</span></span>
<span data-ttu-id="1be5b-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1be5b-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUniversalAppXAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXAppAssignmentSettings",
  "useDeviceContext": true
}
```





