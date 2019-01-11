---
title: deviceAndAppManagementAssignedRoleIds リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1ae87f1a8430ef2539fe10e813390b0fbd68b267
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846341"
---
# <a name="deviceandappmanagementassignedroleids-resource-type"></a><span data-ttu-id="26278-103">deviceAndAppManagementAssignedRoleIds リソースの種類</span><span class="sxs-lookup"><span data-stu-id="26278-103">deviceAndAppManagementAssignedRoleIds resource type</span></span>

> <span data-ttu-id="26278-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="26278-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="26278-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="26278-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="26278-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="26278-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="26278-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="26278-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="26278-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="26278-108">Properties</span></span>
|<span data-ttu-id="26278-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="26278-109">Property</span></span>|<span data-ttu-id="26278-110">種類</span><span class="sxs-lookup"><span data-stu-id="26278-110">Type</span></span>|<span data-ttu-id="26278-111">説明</span><span class="sxs-lookup"><span data-stu-id="26278-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26278-112">roleDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="26278-112">roleDefinitionIds</span></span>|<span data-ttu-id="26278-113">Guid コレクション</span><span class="sxs-lookup"><span data-stu-id="26278-113">Guid collection</span></span>|<span data-ttu-id="26278-114">特定ユーザーに割り当てられているロールの定義のロール定義の Id。</span><span class="sxs-lookup"><span data-stu-id="26278-114">Role Definition IDs for the specifc Role Definitions assigned to a user.</span></span>|
|<span data-ttu-id="26278-115">roleAssignmentIds</span><span class="sxs-lookup"><span data-stu-id="26278-115">roleAssignmentIds</span></span>|<span data-ttu-id="26278-116">Guid コレクション</span><span class="sxs-lookup"><span data-stu-id="26278-116">Guid collection</span></span>|<span data-ttu-id="26278-117">ロールの割り当てがユーザーに割り当て、特定のロールの割り当ての Id です。</span><span class="sxs-lookup"><span data-stu-id="26278-117">Role Assignment IDs for the specifc Role Assignments assigned to a user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="26278-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="26278-118">Relationships</span></span>
<span data-ttu-id="26278-119">なし</span><span class="sxs-lookup"><span data-stu-id="26278-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="26278-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="26278-120">JSON Representation</span></span>
<span data-ttu-id="26278-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="26278-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceAndAppManagementAssignedRoleIds"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignedRoleIds",
  "roleDefinitionIds": [
    "Guid"
  ],
  "roleAssignmentIds": [
    "Guid"
  ]
}
```





