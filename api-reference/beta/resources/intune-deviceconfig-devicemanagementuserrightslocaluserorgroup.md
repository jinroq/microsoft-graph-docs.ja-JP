---
title: deviceManagementUserRightsLocalUserOrGroup リソースの種類
description: ローカル ユーザーまたはグループのユーザー権利の設定の使用に関する情報を表します。
author: tfitzmac
ms.openlocfilehash: baabd2f3bb9e3bce44d172cd83f61f57c5c2c98d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303732"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a><span data-ttu-id="a768c-103">deviceManagementUserRightsLocalUserOrGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a768c-103">deviceManagementUserRightsLocalUserOrGroup resource type</span></span>

> <span data-ttu-id="a768c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a768c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a768c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a768c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a768c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a768c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a768c-107">ローカル ユーザーまたはグループのユーザー権利の設定の使用に関する情報を表します。</span><span class="sxs-lookup"><span data-stu-id="a768c-107">Represents information for a local user or group used for user rights setting.</span></span>
## <a name="properties"></a><span data-ttu-id="a768c-108">Properties</span><span class="sxs-lookup"><span data-stu-id="a768c-108">Properties</span></span>
|<span data-ttu-id="a768c-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a768c-109">Property</span></span>|<span data-ttu-id="a768c-110">種類</span><span class="sxs-lookup"><span data-stu-id="a768c-110">Type</span></span>|<span data-ttu-id="a768c-111">説明</span><span class="sxs-lookup"><span data-stu-id="a768c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a768c-112">名前</span><span class="sxs-lookup"><span data-stu-id="a768c-112">name</span></span>|<span data-ttu-id="a768c-113">String</span><span class="sxs-lookup"><span data-stu-id="a768c-113">String</span></span>|<span data-ttu-id="a768c-114">ローカル ユーザーまたはグループの名前です。</span><span class="sxs-lookup"><span data-stu-id="a768c-114">The name of this local user or group.</span></span>|
|<span data-ttu-id="a768c-115">説明</span><span class="sxs-lookup"><span data-stu-id="a768c-115">description</span></span>|<span data-ttu-id="a768c-116">String</span><span class="sxs-lookup"><span data-stu-id="a768c-116">String</span></span>|<span data-ttu-id="a768c-117">ローカル ユーザーまたはグループの管理の説明です。</span><span class="sxs-lookup"><span data-stu-id="a768c-117">Admin’s description of this local user or group.</span></span>|
|<span data-ttu-id="a768c-118">securityIdentifier</span><span class="sxs-lookup"><span data-stu-id="a768c-118">securityIdentifier</span></span>|<span data-ttu-id="a768c-119">String</span><span class="sxs-lookup"><span data-stu-id="a768c-119">String</span></span>|<span data-ttu-id="a768c-120">このローカル ユーザーまたはグループのセキュリティ識別子 (例: \* S-1-5-32-544)。</span><span class="sxs-lookup"><span data-stu-id="a768c-120">The security identifier of this local user or group (e.g. \*S-1-5-32-544).</span></span>|

## <a name="relationships"></a><span data-ttu-id="a768c-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a768c-121">Relationships</span></span>
<span data-ttu-id="a768c-122">なし</span><span class="sxs-lookup"><span data-stu-id="a768c-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a768c-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a768c-123">JSON Representation</span></span>
<span data-ttu-id="a768c-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a768c-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
  "name": "String",
  "description": "String",
  "securityIdentifier": "String"
}
```





