---
title: auditResource リソースの種類
description: 監査のリソースのプロパティが含まれるクラス。
ms.openlocfilehash: a3825418c1406bbe9fcce7feeba96217342c735e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072074"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="11bef-103">auditResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="11bef-103">auditResource resource type</span></span>

> <span data-ttu-id="11bef-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="11bef-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="11bef-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="11bef-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="11bef-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="11bef-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="11bef-107">監査のリソースのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="11bef-107">A class containing the properties for Audit Resource.</span></span>
## <a name="properties"></a><span data-ttu-id="11bef-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="11bef-108">Properties</span></span>
|<span data-ttu-id="11bef-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="11bef-109">Property</span></span>|<span data-ttu-id="11bef-110">型</span><span class="sxs-lookup"><span data-stu-id="11bef-110">Type</span></span>|<span data-ttu-id="11bef-111">説明</span><span class="sxs-lookup"><span data-stu-id="11bef-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11bef-112">displayName</span><span class="sxs-lookup"><span data-stu-id="11bef-112">displayName</span></span>|<span data-ttu-id="11bef-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="11bef-113">String</span></span>|<span data-ttu-id="11bef-114">表示名。</span><span class="sxs-lookup"><span data-stu-id="11bef-114">Display name.</span></span>|
|<span data-ttu-id="11bef-115">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="11bef-115">modifiedProperties</span></span>|<span data-ttu-id="11bef-116">[auditProperty](../resources/intune-auditing-auditproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="11bef-116">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="11bef-117">変更されたプロパティの一覧。</span><span class="sxs-lookup"><span data-stu-id="11bef-117">List of modified properties.</span></span>|
|<span data-ttu-id="11bef-118">type</span><span class="sxs-lookup"><span data-stu-id="11bef-118">type</span></span>|<span data-ttu-id="11bef-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="11bef-119">String</span></span>|<span data-ttu-id="11bef-120">監査のリソースの種類。</span><span class="sxs-lookup"><span data-stu-id="11bef-120">Audit resource's type.</span></span>|
|<span data-ttu-id="11bef-121">resourceId</span><span class="sxs-lookup"><span data-stu-id="11bef-121">resourceId</span></span>|<span data-ttu-id="11bef-122">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="11bef-122">String</span></span>|<span data-ttu-id="11bef-123">監査のリソースの ID。</span><span class="sxs-lookup"><span data-stu-id="11bef-123">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="11bef-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="11bef-124">Relationships</span></span>
<span data-ttu-id="11bef-125">なし</span><span class="sxs-lookup"><span data-stu-id="11bef-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="11bef-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="11bef-126">JSON Representation</span></span>
<span data-ttu-id="11bef-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="11bef-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditResource",
  "displayName": "String",
  "modifiedProperties": [
    {
      "@odata.type": "microsoft.graph.auditProperty",
      "displayName": "String",
      "oldValue": "String",
      "newValue": "String"
    }
  ],
  "type": "String",
  "resourceId": "String"
}
```





