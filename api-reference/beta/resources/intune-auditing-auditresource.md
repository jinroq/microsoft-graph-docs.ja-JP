---
title: auditResource リソースの種類
description: 監査のリソースのプロパティが含まれるクラス。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 20c39cc5138be5c731bc34b1e13f8536e7581c40
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32558308"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="66d4c-103">auditResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="66d4c-103">auditResource resource type</span></span>

> <span data-ttu-id="66d4c-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66d4c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66d4c-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="66d4c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66d4c-106">監査のリソースのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="66d4c-106">A class containing the properties for Audit Resource.</span></span>

## <a name="properties"></a><span data-ttu-id="66d4c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="66d4c-107">Properties</span></span>
|<span data-ttu-id="66d4c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="66d4c-108">Property</span></span>|<span data-ttu-id="66d4c-109">型</span><span class="sxs-lookup"><span data-stu-id="66d4c-109">Type</span></span>|<span data-ttu-id="66d4c-110">説明</span><span class="sxs-lookup"><span data-stu-id="66d4c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66d4c-111">displayName</span><span class="sxs-lookup"><span data-stu-id="66d4c-111">displayName</span></span>|<span data-ttu-id="66d4c-112">String</span><span class="sxs-lookup"><span data-stu-id="66d4c-112">String</span></span>|<span data-ttu-id="66d4c-113">表示名。</span><span class="sxs-lookup"><span data-stu-id="66d4c-113">Display name.</span></span>|
|<span data-ttu-id="66d4c-114">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="66d4c-114">modifiedProperties</span></span>|<span data-ttu-id="66d4c-115">[auditProperty](../resources/intune-auditing-auditproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="66d4c-115">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="66d4c-116">変更されたプロパティの一覧。</span><span class="sxs-lookup"><span data-stu-id="66d4c-116">List of modified properties.</span></span>|
|<span data-ttu-id="66d4c-117">type</span><span class="sxs-lookup"><span data-stu-id="66d4c-117">type</span></span>|<span data-ttu-id="66d4c-118">String</span><span class="sxs-lookup"><span data-stu-id="66d4c-118">String</span></span>|<span data-ttu-id="66d4c-119">監査のリソースの種類。</span><span class="sxs-lookup"><span data-stu-id="66d4c-119">Audit resource's type.</span></span>|
|<span data-ttu-id="66d4c-120">resourceId</span><span class="sxs-lookup"><span data-stu-id="66d4c-120">resourceId</span></span>|<span data-ttu-id="66d4c-121">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="66d4c-121">String</span></span>|<span data-ttu-id="66d4c-122">監査のリソースの ID。</span><span class="sxs-lookup"><span data-stu-id="66d4c-122">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66d4c-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="66d4c-123">Relationships</span></span>
<span data-ttu-id="66d4c-124">なし</span><span class="sxs-lookup"><span data-stu-id="66d4c-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="66d4c-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="66d4c-125">JSON Representation</span></span>
<span data-ttu-id="66d4c-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="66d4c-126">Here is a JSON representation of the resource.</span></span>
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





