---
title: deviceAndAppManagementAssignedRoleIds リソースの種類
description: まだ文書化されていません
ms.openlocfilehash: 9d9fbf9bc6dcfa422316a236dfd890369d069c2f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070808"
---
# <a name="deviceandappmanagementassignedroleids-resource-type"></a><span data-ttu-id="8b22b-103">deviceAndAppManagementAssignedRoleIds リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8b22b-103">deviceAndAppManagementAssignedRoleIds resource type</span></span>

> <span data-ttu-id="8b22b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8b22b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8b22b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8b22b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8b22b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8b22b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8b22b-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="8b22b-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="8b22b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8b22b-108">Properties</span></span>
|<span data-ttu-id="8b22b-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8b22b-109">Property</span></span>|<span data-ttu-id="8b22b-110">型</span><span class="sxs-lookup"><span data-stu-id="8b22b-110">Type</span></span>|<span data-ttu-id="8b22b-111">説明</span><span class="sxs-lookup"><span data-stu-id="8b22b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b22b-112">roleDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="8b22b-112">roleDefinitionIds</span></span>|<span data-ttu-id="8b22b-113">Guid コレクション</span><span class="sxs-lookup"><span data-stu-id="8b22b-113">Guid collection</span></span>|<span data-ttu-id="8b22b-114">特定ユーザーに割り当てられているロールの定義のロール定義の Id。</span><span class="sxs-lookup"><span data-stu-id="8b22b-114">Role Definition IDs for the specifc Role Definitions assigned to a user.</span></span>|
|<span data-ttu-id="8b22b-115">roleAssignmentIds</span><span class="sxs-lookup"><span data-stu-id="8b22b-115">roleAssignmentIds</span></span>|<span data-ttu-id="8b22b-116">Guid コレクション</span><span class="sxs-lookup"><span data-stu-id="8b22b-116">Guid collection</span></span>|<span data-ttu-id="8b22b-117">ロールの割り当てがユーザーに割り当て、特定のロールの割り当ての Id です。</span><span class="sxs-lookup"><span data-stu-id="8b22b-117">Role Assignment IDs for the specifc Role Assignments assigned to a user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b22b-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8b22b-118">Relationships</span></span>
<span data-ttu-id="8b22b-119">なし</span><span class="sxs-lookup"><span data-stu-id="8b22b-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8b22b-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8b22b-120">JSON Representation</span></span>
<span data-ttu-id="8b22b-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8b22b-121">Here is a JSON representation of the resource.</span></span>
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





