---
title: auditResource リソースの種類
description: 監査のリソースのプロパティが含まれるクラス。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ac7da99203631696b8c93fbde62db906143ffe38
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952245"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="f3bc5-103">auditResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f3bc5-103">auditResource resource type</span></span>

> <span data-ttu-id="f3bc5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f3bc5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f3bc5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3bc5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f3bc5-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f3bc5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f3bc5-107">監査のリソースのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="f3bc5-107">A class containing the properties for Audit Resource.</span></span>
## <a name="properties"></a><span data-ttu-id="f3bc5-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3bc5-108">Properties</span></span>
|<span data-ttu-id="f3bc5-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3bc5-109">Property</span></span>|<span data-ttu-id="f3bc5-110">種類</span><span class="sxs-lookup"><span data-stu-id="f3bc5-110">Type</span></span>|<span data-ttu-id="f3bc5-111">説明</span><span class="sxs-lookup"><span data-stu-id="f3bc5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3bc5-112">displayName</span><span class="sxs-lookup"><span data-stu-id="f3bc5-112">displayName</span></span>|<span data-ttu-id="f3bc5-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f3bc5-113">String</span></span>|<span data-ttu-id="f3bc5-114">表示名。</span><span class="sxs-lookup"><span data-stu-id="f3bc5-114">Display name.</span></span>|
|<span data-ttu-id="f3bc5-115">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="f3bc5-115">modifiedProperties</span></span>|<span data-ttu-id="f3bc5-116">[auditProperty](../resources/intune-auditing-auditproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f3bc5-116">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="f3bc5-117">変更されたプロパティの一覧。</span><span class="sxs-lookup"><span data-stu-id="f3bc5-117">List of modified properties.</span></span>|
|<span data-ttu-id="f3bc5-118">type</span><span class="sxs-lookup"><span data-stu-id="f3bc5-118">type</span></span>|<span data-ttu-id="f3bc5-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f3bc5-119">String</span></span>|<span data-ttu-id="f3bc5-120">監査のリソースの種類。</span><span class="sxs-lookup"><span data-stu-id="f3bc5-120">Audit resource's type.</span></span>|
|<span data-ttu-id="f3bc5-121">resourceId</span><span class="sxs-lookup"><span data-stu-id="f3bc5-121">resourceId</span></span>|<span data-ttu-id="f3bc5-122">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f3bc5-122">String</span></span>|<span data-ttu-id="f3bc5-123">監査のリソースの ID。</span><span class="sxs-lookup"><span data-stu-id="f3bc5-123">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3bc5-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f3bc5-124">Relationships</span></span>
<span data-ttu-id="f3bc5-125">なし</span><span class="sxs-lookup"><span data-stu-id="f3bc5-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f3bc5-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f3bc5-126">JSON Representation</span></span>
<span data-ttu-id="f3bc5-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f3bc5-127">Here is a JSON representation of the resource.</span></span>
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





