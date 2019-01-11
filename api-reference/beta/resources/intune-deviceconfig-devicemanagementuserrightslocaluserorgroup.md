---
title: deviceManagementUserRightsLocalUserOrGroup リソースの種類
description: ローカル ユーザーまたはグループのユーザー権利の設定の使用に関する情報を表します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d795e2b259c71612b1d0720796b6ad76145bb36d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885744"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a><span data-ttu-id="5e868-103">deviceManagementUserRightsLocalUserOrGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5e868-103">deviceManagementUserRightsLocalUserOrGroup resource type</span></span>

> <span data-ttu-id="5e868-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5e868-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5e868-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5e868-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5e868-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5e868-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5e868-107">ローカル ユーザーまたはグループのユーザー権利の設定の使用に関する情報を表します。</span><span class="sxs-lookup"><span data-stu-id="5e868-107">Represents information for a local user or group used for user rights setting.</span></span>
## <a name="properties"></a><span data-ttu-id="5e868-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5e868-108">Properties</span></span>
|<span data-ttu-id="5e868-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5e868-109">Property</span></span>|<span data-ttu-id="5e868-110">種類</span><span class="sxs-lookup"><span data-stu-id="5e868-110">Type</span></span>|<span data-ttu-id="5e868-111">説明</span><span class="sxs-lookup"><span data-stu-id="5e868-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e868-112">名前</span><span class="sxs-lookup"><span data-stu-id="5e868-112">name</span></span>|<span data-ttu-id="5e868-113">String</span><span class="sxs-lookup"><span data-stu-id="5e868-113">String</span></span>|<span data-ttu-id="5e868-114">ローカル ユーザーまたはグループの名前です。</span><span class="sxs-lookup"><span data-stu-id="5e868-114">The name of this local user or group.</span></span>|
|<span data-ttu-id="5e868-115">説明</span><span class="sxs-lookup"><span data-stu-id="5e868-115">description</span></span>|<span data-ttu-id="5e868-116">String</span><span class="sxs-lookup"><span data-stu-id="5e868-116">String</span></span>|<span data-ttu-id="5e868-117">ローカル ユーザーまたはグループの管理の説明です。</span><span class="sxs-lookup"><span data-stu-id="5e868-117">Admin’s description of this local user or group.</span></span>|
|<span data-ttu-id="5e868-118">securityIdentifier</span><span class="sxs-lookup"><span data-stu-id="5e868-118">securityIdentifier</span></span>|<span data-ttu-id="5e868-119">String</span><span class="sxs-lookup"><span data-stu-id="5e868-119">String</span></span>|<span data-ttu-id="5e868-120">このローカル ユーザーまたはグループのセキュリティ識別子 (例: \* S-1-5-32-544)。</span><span class="sxs-lookup"><span data-stu-id="5e868-120">The security identifier of this local user or group (e.g. \*S-1-5-32-544).</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e868-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5e868-121">Relationships</span></span>
<span data-ttu-id="5e868-122">なし</span><span class="sxs-lookup"><span data-stu-id="5e868-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5e868-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5e868-123">JSON Representation</span></span>
<span data-ttu-id="5e868-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5e868-124">Here is a JSON representation of the resource.</span></span>
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





