---
title: deviceAndAppManagementAssignedRoleIds リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2dbabca28f9ed8aa491d01f6eada5dc11b76867b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923377"
---
# <a name="deviceandappmanagementassignedroleids-resource-type"></a><span data-ttu-id="8f378-103">deviceAndAppManagementAssignedRoleIds リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8f378-103">deviceAndAppManagementAssignedRoleIds resource type</span></span>

> <span data-ttu-id="8f378-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8f378-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8f378-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8f378-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8f378-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8f378-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8f378-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="8f378-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="8f378-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8f378-108">Properties</span></span>
|<span data-ttu-id="8f378-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8f378-109">Property</span></span>|<span data-ttu-id="8f378-110">種類</span><span class="sxs-lookup"><span data-stu-id="8f378-110">Type</span></span>|<span data-ttu-id="8f378-111">説明</span><span class="sxs-lookup"><span data-stu-id="8f378-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f378-112">roleDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="8f378-112">roleDefinitionIds</span></span>|<span data-ttu-id="8f378-113">Guid コレクション</span><span class="sxs-lookup"><span data-stu-id="8f378-113">Guid collection</span></span>|<span data-ttu-id="8f378-114">特定ユーザーに割り当てられているロールの定義のロール定義の Id。</span><span class="sxs-lookup"><span data-stu-id="8f378-114">Role Definition IDs for the specifc Role Definitions assigned to a user.</span></span>|
|<span data-ttu-id="8f378-115">roleAssignmentIds</span><span class="sxs-lookup"><span data-stu-id="8f378-115">roleAssignmentIds</span></span>|<span data-ttu-id="8f378-116">Guid コレクション</span><span class="sxs-lookup"><span data-stu-id="8f378-116">Guid collection</span></span>|<span data-ttu-id="8f378-117">ロールの割り当てがユーザーに割り当て、特定のロールの割り当ての Id です。</span><span class="sxs-lookup"><span data-stu-id="8f378-117">Role Assignment IDs for the specifc Role Assignments assigned to a user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f378-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8f378-118">Relationships</span></span>
<span data-ttu-id="8f378-119">なし</span><span class="sxs-lookup"><span data-stu-id="8f378-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8f378-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8f378-120">JSON Representation</span></span>
<span data-ttu-id="8f378-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8f378-121">Here is a JSON representation of the resource.</span></span>
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





