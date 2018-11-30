---
title: microsoftStoreForBusinessAppAssignmentSettings リソースの種類
description: グループに、ビジネス向け Microsoft Store モバイル アプリを割り当てるためのプロパティが含まれます。
ms.openlocfilehash: 53dc4e9887147253047df67db865c45488b51009
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068508"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="31736-103">microsoftStoreForBusinessAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="31736-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="31736-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="31736-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="31736-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31736-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="31736-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="31736-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="31736-107">グループに、ビジネス向け Microsoft Store モバイル アプリを割り当てるためのプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="31736-107">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>

<span data-ttu-id="31736-108">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="31736-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="31736-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31736-109">Properties</span></span>
|<span data-ttu-id="31736-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31736-110">Property</span></span>|<span data-ttu-id="31736-111">型</span><span class="sxs-lookup"><span data-stu-id="31736-111">Type</span></span>|<span data-ttu-id="31736-112">説明</span><span class="sxs-lookup"><span data-stu-id="31736-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31736-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="31736-113">useDeviceContext</span></span>|<span data-ttu-id="31736-114">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="31736-114">Boolean</span></span>|<span data-ttu-id="31736-115">ビジネス向け Microsoft Store モバイル アプリのデバイス実行コンテキストを使用するかどうか。</span><span class="sxs-lookup"><span data-stu-id="31736-115">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="31736-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="31736-116">Relationships</span></span>
<span data-ttu-id="31736-117">なし</span><span class="sxs-lookup"><span data-stu-id="31736-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="31736-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="31736-118">JSON Representation</span></span>
<span data-ttu-id="31736-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="31736-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.microsoftStoreForBusinessAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessAppAssignmentSettings",
  "useDeviceContext": true
}
```





