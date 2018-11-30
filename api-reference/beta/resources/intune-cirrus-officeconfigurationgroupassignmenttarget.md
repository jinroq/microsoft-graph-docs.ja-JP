---
title: officeConfigurationGroupAssignmentTarget リソースの種類
description: AAD Office クライアントの構成は、ターゲットの割り当てをグループ化します。
ms.openlocfilehash: 263e48bfc5800231a9f36159e802f65294e6ac02
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072326"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a><span data-ttu-id="f0566-103">officeConfigurationGroupAssignmentTarget リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f0566-103">officeConfigurationGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="f0566-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f0566-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f0566-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0566-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f0566-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f0566-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f0566-107">AAD Office クライアントの構成は、ターゲットの割り当てをグループ化します。</span><span class="sxs-lookup"><span data-stu-id="f0566-107">Office client configuration AAD group assignment target.</span></span>

<span data-ttu-id="f0566-108">[OfficeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="f0566-108">Inherits from [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f0566-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f0566-109">Properties</span></span>
|<span data-ttu-id="f0566-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f0566-110">Property</span></span>|<span data-ttu-id="f0566-111">型</span><span class="sxs-lookup"><span data-stu-id="f0566-111">Type</span></span>|<span data-ttu-id="f0566-112">説明</span><span class="sxs-lookup"><span data-stu-id="f0566-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0566-113">groupId</span><span class="sxs-lookup"><span data-stu-id="f0566-113">groupId</span></span>|<span data-ttu-id="f0566-114">String</span><span class="sxs-lookup"><span data-stu-id="f0566-114">String</span></span>|<span data-ttu-id="f0566-115">AAD グループの Id は、対象としてデバイスを構成します。</span><span class="sxs-lookup"><span data-stu-id="f0566-115">The Id of the AAD group we are targeting the device configuration to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0566-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f0566-116">Relationships</span></span>
<span data-ttu-id="f0566-117">なし</span><span class="sxs-lookup"><span data-stu-id="f0566-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f0566-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f0566-118">JSON Representation</span></span>
<span data-ttu-id="f0566-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f0566-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeConfigurationGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeConfigurationGroupAssignmentTarget",
  "groupId": "String"
}
```



