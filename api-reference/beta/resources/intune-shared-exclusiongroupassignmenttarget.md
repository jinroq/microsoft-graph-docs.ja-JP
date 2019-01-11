---
title: exclusionGroupAssignmentTarget リソースの種類
description: 割り当てから除外するグループを表します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ce17f38b3ab604a11710c64992a046f6d71a6659
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870708"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="153aa-103">exclusionGroupAssignmentTarget リソースの種類</span><span class="sxs-lookup"><span data-stu-id="153aa-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="153aa-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="153aa-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="153aa-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="153aa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="153aa-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="153aa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="153aa-107">割り当てから除外するグループを表します。</span><span class="sxs-lookup"><span data-stu-id="153aa-107">Represents a group that should be excluded from an assignment.</span></span>

<span data-ttu-id="153aa-108">[groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="153aa-108">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="153aa-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="153aa-109">Properties</span></span>
|<span data-ttu-id="153aa-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="153aa-110">Property</span></span>|<span data-ttu-id="153aa-111">種類</span><span class="sxs-lookup"><span data-stu-id="153aa-111">Type</span></span>|<span data-ttu-id="153aa-112">説明</span><span class="sxs-lookup"><span data-stu-id="153aa-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="153aa-113">groupId</span><span class="sxs-lookup"><span data-stu-id="153aa-113">groupId</span></span>|<span data-ttu-id="153aa-114">文字列</span><span class="sxs-lookup"><span data-stu-id="153aa-114">String</span></span>|<span data-ttu-id="153aa-115">割り当てのターゲットとなるグループ ID です。</span><span class="sxs-lookup"><span data-stu-id="153aa-115">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="153aa-116">[groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="153aa-116">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="153aa-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="153aa-117">Relationships</span></span>
<span data-ttu-id="153aa-118">なし</span><span class="sxs-lookup"><span data-stu-id="153aa-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="153aa-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="153aa-119">JSON Representation</span></span>
<span data-ttu-id="153aa-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="153aa-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.exclusionGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.exclusionGroupAssignmentTarget",
  "groupId": "String"
}
```





