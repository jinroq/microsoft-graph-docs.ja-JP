---
title: auditResource リソースの種類
description: 監査のリソースのプロパティが含まれるクラス。
author: tfitzmac
ms.openlocfilehash: 5cfc23a80b2247b9f561d802ce844091c623ef62
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302661"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="e7746-103">auditResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e7746-103">auditResource resource type</span></span>

> <span data-ttu-id="e7746-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e7746-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e7746-105">監査のリソースのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="e7746-105">A class containing the properties for Audit Resource.</span></span>
## <a name="properties"></a><span data-ttu-id="e7746-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e7746-106">Properties</span></span>
|<span data-ttu-id="e7746-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e7746-107">Property</span></span>|<span data-ttu-id="e7746-108">種類</span><span class="sxs-lookup"><span data-stu-id="e7746-108">Type</span></span>|<span data-ttu-id="e7746-109">説明</span><span class="sxs-lookup"><span data-stu-id="e7746-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7746-110">displayName</span><span class="sxs-lookup"><span data-stu-id="e7746-110">displayName</span></span>|<span data-ttu-id="e7746-111">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="e7746-111">String</span></span>|<span data-ttu-id="e7746-112">表示名。</span><span class="sxs-lookup"><span data-stu-id="e7746-112">Display name.</span></span>|
|<span data-ttu-id="e7746-113">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="e7746-113">modifiedProperties</span></span>|<span data-ttu-id="e7746-114">[auditProperty](../resources/intune-auditing-auditproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e7746-114">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="e7746-115">変更されたプロパティの一覧。</span><span class="sxs-lookup"><span data-stu-id="e7746-115">List of modified properties.</span></span>|
|<span data-ttu-id="e7746-116">type</span><span class="sxs-lookup"><span data-stu-id="e7746-116">type</span></span>|<span data-ttu-id="e7746-117">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="e7746-117">String</span></span>|<span data-ttu-id="e7746-118">監査のリソースの種類。</span><span class="sxs-lookup"><span data-stu-id="e7746-118">Audit resource's type.</span></span>|
|<span data-ttu-id="e7746-119">resourceId</span><span class="sxs-lookup"><span data-stu-id="e7746-119">resourceId</span></span>|<span data-ttu-id="e7746-120">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="e7746-120">String</span></span>|<span data-ttu-id="e7746-121">監査のリソースの ID。</span><span class="sxs-lookup"><span data-stu-id="e7746-121">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7746-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e7746-122">Relationships</span></span>
<span data-ttu-id="e7746-123">なし</span><span class="sxs-lookup"><span data-stu-id="e7746-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e7746-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e7746-124">JSON Representation</span></span>
<span data-ttu-id="e7746-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e7746-125">Here is a JSON representation of the resource.</span></span>
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



